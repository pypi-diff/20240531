# Comparing `tmp/swanlab-0.3.6.tar.gz` & `tmp/swanlab-0.3.7.tar.gz`

## Comparing `swanlab-0.3.6.tar` & `swanlab-0.3.7.tar`

### file list

```diff
@@ -1,854 +1,855 @@
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.6/.eslintrc-auto-import.json
--rw-r--r--   0        0        0    28874 2020-02-02 00:00:00.000000 swanlab-0.3.6/README.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.6/jsconfig.json
--rw-r--r--   0        0        0   236753 2020-02-02 00:00:00.000000 swanlab-0.3.6/package-lock.json
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 swanlab-0.3.6/package.json
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.6/.config/copy_frontend.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.6/.vscode/extensions.json
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 swanlab-0.3.6/.vscode/launch.json
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.6/.vscode/settings.json
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.6/.vscode/tailwind.json
--rw-r--r--   0        0        0   218889 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/.package-lock.json
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@alloc/quick-lru/package.json
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antfu/utils/package.json
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/adjust/package.json
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/adjust/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/attr/package.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/color-util/package.json
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/component/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/component/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/coord/package.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/dom-util/package.json
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/event-emitter/package.json
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-base/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-canvas/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-math/package.json
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g-svg/package.json
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g2/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/g2plot/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/scale/package.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@antv/util/package.json
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@babel/parser/package.json
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@esbuild/linux-x64/package.json
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@eslint/eslintrc/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@eslint/js/package.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@eslint-community/eslint-utils/package.json
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@eslint-community/regexpp/package.json
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@headlessui/vue/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@humanwhocodes/config-array/package.json
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@humanwhocodes/module-importer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@humanwhocodes/object-schema/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@intlify/core-base/package.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@intlify/message-compiler/package.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@intlify/shared/package.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@isaacs/cliui/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@jest/schemas/package.json
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@jridgewell/gen-mapping/package.json
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@jridgewell/resolve-uri/package.json
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@jridgewell/set-array/package.json
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@jridgewell/source-map/package.json
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@jridgewell/sourcemap-codec/package.json
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@jridgewell/trace-mapping/package.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@ljharb/resumer/package.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@ljharb/through/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@ljharb/through/tsconfig.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@nodelib/fs.scandir/package.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@nodelib/fs.stat/package.json
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@nodelib/fs.walk/package.json
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@pkgjs/parseargs/package.json
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@popperjs/core/package.json
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@rollup/pluginutils/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@rollup/pluginutils/dist/es/package.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@rollup/rollup-linux-x64-gnu/package.json
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@rollup/rollup-linux-x64-musl/package.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@sinclair/typebox/package.json
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@tanstack/virtual-core/package.json
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@tanstack/vue-virtual/package.json
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@types/d3-timer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@types/estree/package.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@ungap/structured-clone/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@ungap/structured-clone/cjs/package.json
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitejs/plugin-vue/package.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/expect/package.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/runner/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/runner/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/snapshot/package.json
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/spy/package.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/utils/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vitest/utils/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/compiler-core/package.json
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/compiler-dom/package.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/compiler-sfc/package.json
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/compiler-ssr/package.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/devtools-api/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/reactivity/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/runtime-core/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/runtime-dom/package.json
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/server-renderer/package.json
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/@vue/shared/package.json
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/acorn/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/acorn-jsx/package.json
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/acorn-walk/package.json
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ajv/package.json
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ajv/lib/refs/data.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-draft-04.json
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-draft-06.json
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-draft-07.json
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-secure.json
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/align-text/package.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/amdefine/package.json
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/any-promise/package.json
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/anymatch/package.json
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/arg/package.json
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/argparse/package.json
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/array-buffer-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/array-buffer-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/arraybuffer.prototype.slice/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/assertion-error/package.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/asynckit/package.json
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/autoprefixer/package.json
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/available-typed-arrays/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/available-typed-arrays/tsconfig.json
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/axios/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/balanced-match/package.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/base64-arraybuffer/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/binary-extensions/binary-extensions.json
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/binary-extensions/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/boolbase/package.json
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/braces/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/browserslist/package.json
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/buffer-from/package.json
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/cac/package.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/call-bind/package.json
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/callsites/package.json
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/camelcase/package.json
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/camelcase-css/package.json
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/caniuse-lite/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/center-align/package.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/chai/bower.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/chai/package.json
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/chalk/package.json
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/check-error/package.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/chokidar/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/chokidar/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/cliui/package.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/color-convert/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/color-name/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/combined-stream/package.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/commander/package-support.json
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/commander/package.json
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/concat-map/package.json
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/confbox/package.json
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/contour_plot/package.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/cross-spawn/package.json
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/css-line-break/package.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/cssesc/package.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/csstype/package.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/d3-color/package.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/d3-ease/package.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/d3-hierarchy/package.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/d3-interpolate/package.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/d3-regression/package.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/d3-timer/package.json
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/data-view-buffer/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/data-view-buffer/tsconfig.json
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/data-view-byte-length/package.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/data-view-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/data-view-byte-offset/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/data-view-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/debug/package.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/decamelize/package.json
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/deep-eql/package.json
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/deep-equal/package.json
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/deep-is/package.json
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/define-data-property/package.json
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/define-data-property/tsconfig.json
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/define-properties/package.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/defined/package.json
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/delayed-stream/package.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/detect-browser/package.json
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/didyoumean/package.json
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/diff-sequences/package.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/dlv/package.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/doctrine/package.json
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/dotignore/package.json
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eastasianwidth/package.json
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/electron-to-chromium/chromium-versions.json
--rw-r--r--   0        0        0    50514 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/electron-to-chromium/full-chromium-versions.json
--rw-r--r--   0        0        0    78988 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/electron-to-chromium/full-versions.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/electron-to-chromium/package.json
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/electron-to-chromium/versions.json
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/entities/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/entities/lib/esm/package.json
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-abstract/package.json
--rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-abstract/helpers/caseFolding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-abstract/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-abstract/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-define-property/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-define-property/tsconfig.json
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-errors/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-errors/tsconfig.json
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-object-atoms/package.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-object-atoms/tsconfig.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-set-tostringtag/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-set-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/es-to-primitive/package.json
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/esbuild/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/escalade/package.json
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint/conf/replacements.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint/conf/rule-type-list.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-config-prettier/package.json
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-prettier/package.json
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/package.json
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
--rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/math-elements.json
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-scope/package.json
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/eslint-visitor-keys/package.json
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/espree/package.json
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/esquery/package.json
--rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/esrecurse/package.json
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/estraverse/package.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/estree-walker/dist/esm/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/estree-walker/src/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/esutils/package.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/execa/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fast-deep-equal/package.json
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fast-diff/package.json
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fast-glob/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fast-glob/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fast-json-stable-stringify/package.json
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fast-json-stable-stringify/benchmark/test.json
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fast-levenshtein/package.json
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fastq/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fastq/test/tsconfig.json
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fecha/package.json
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/file-entry-cache/package.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fill-range/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/find-up/package.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/flat-cache/package.json
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/flatted/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/flatted/cjs/package.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fmin/.eslintrc.json
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fmin/package.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/follow-redirects/package.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/for-each/package.json
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/foreground-child/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/foreground-child/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/foreground-child/dist/mjs/package.json
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/form-data/package.json
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fraction.js/package.json
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/fs.realpath/package.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/function-bind/package.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/function.prototype.name/package.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/functions-have-names/package.json
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/get-func-name/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/get-intrinsic/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/get-stream/package.json
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/get-symbol-description/package.json
--rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/mat2/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/mat2d/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/mat3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/mat4/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/quat/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/quat2/package.json
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/types.d.ts/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/vec2/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/vec3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gl-matrix/vec4/package.json
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/glob/package.json
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/globals/globals.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/globals/package.json
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/globalthis/package.json
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/gopd/package.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/graphemer/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has/package.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-ansi/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-bigints/package.json
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-flag/package.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-property-descriptors/package.json
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-proto/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-proto/tsconfig.json
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-symbols/package.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-tostringtag/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/has-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/hasown/package.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/hasown/tsconfig.json
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/html2canvas/package.json
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/html2canvas/tsconfig.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/human-signals/package.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/husky/package.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ignore/package.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/immutable/package.json
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/import-fresh/package.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/imurmurhash/package.json
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/inflight/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/inherits/package.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/internal-slot/package.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-arguments/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-bigint/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-binary-path/package.json
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-boolean-object/package.json
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-buffer/package.json
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-callable/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-core-module/core.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-core-module/package.json
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-data-view/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-data-view/tsconfig.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-date-object/package.json
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-extglob/package.json
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-fullwidth-code-point/package.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-glob/package.json
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-negative-zero/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-negative-zero/tsconfig.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-number/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-number-object/package.json
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-path-inside/package.json
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-regex/package.json
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-shared-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-shared-array-buffer/tsconfig.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-stream/package.json
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-string/package.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-symbol/package.json
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-typed-array/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-typed-array/tsconfig.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/is-weakref/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/isarray/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/isexe/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/jackspeak/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/jackspeak/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/jackspeak/dist/esm/package.json
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/jiti/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/js-tokens/package.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/js-yaml/package.json
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/json-buffer/package.json
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/json-schema-traverse/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/json-stable-stringify-without-jsonify/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/json2module/package.json
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/json5/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/keyv/package.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/kind-of/package.json
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lazy-cache/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/levn/package.json
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lines-and-columns/package.json
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/locate-path/package.json
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lodash/package.json
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lodash-es/package.json
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lodash.merge/package.json
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/longest/package.json
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/loupe/package.json
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lru-cache/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lru-cache/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/lru-cache/dist/esm/package.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/magic-string/package.json
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/merge-stream/package.json
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/merge2/package.json
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/micromatch/package.json
--rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mime-db/db.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mime-db/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mime-types/package.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mimic-fn/package.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/minimatch/package.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/minimist/package.json
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/minipass/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/minipass/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/minipass/dist/esm/package.json
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mlly/package.json
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mock-property/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mockjs/bower.json
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mockjs/package.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mockjs/test/bower.json
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mockjs/test/package.json
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/moment/package.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ms/package.json
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/mz/package.json
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/nanoid/package.json
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/nanoid/async/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/nanoid/non-secure/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/nanoid/url-alphabet/package.json
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/natural-compare/package.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/node-releases/package.json
--rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/node-releases/data/processed/envs.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/node-releases/data/release-schedule/release-schedule.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/normalize-path/package.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/normalize-range/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/npm-run-path/package.json
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/npm-run-path/node_modules/path-key/package.json
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/nth-check/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/nth-check/lib/esm/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/object-assign/package.json
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/object-hash/package.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/object-is/package.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/object-keys/package.json
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/object.assign/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/once/package.json
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/onetime/package.json
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/optionator/package.json
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/p-locate/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/parent-module/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/path-exists/package.json
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/path-is-absolute/package.json
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/path-key/package.json
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/path-parse/package.json
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/path-scurry/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/path-scurry/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/path-scurry/dist/esm/package.json
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pathe/package.json
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pathval/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pdfast/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/picocolors/package.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/picomatch/package.json
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pify/package.json
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pinia/package.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pinia/node_modules/vue-demi/package.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pirates/package.json
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pkg-types/package.json
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/possible-typed-array-names/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/possible-typed-array-names/tsconfig.json
--rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss-import/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss-js/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss-load-config/package.json
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss-load-config/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss-nested/package.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss-selector-parser/package.json
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/postcss-value-parser/package.json
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/prelude-ls/package.json
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/prettier/package.json
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/prettier-linter-helpers/package.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/prettier-linter-helpers/.vscode/settings.json
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pretty-format/package.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/pretty-format/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/proxy-from-env/package.json
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/punycode/package.json
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/queue-microtask/package.json
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/react-is/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/read-cache/package.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/readdirp/package.json
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/regexp.prototype.flags/package.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/repeat-string/package.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/lib/core.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/baz/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/browser_field/package.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/dot_main/package.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/dot_slash_main/package.json
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/false_main/package.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/incorrect_main/package.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/invalid_main/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/multirepo/lerna.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/multirepo/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve/test/resolver/symlinked/package/package.json
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/resolve-from/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/reusify/package.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/right-align/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rimraf/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rollup/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rollup/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rollup/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rollup/node_modules/chalk/package.json
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rollup/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rollup/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rollup/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/run-parallel/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/rw/package.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/safe-array-concat/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/safe-array-concat/tsconfig.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/safe-regex-test/package.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sass/package.json
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/scule/package.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/semver/package.json
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/set-function-length/package.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/set-function-length/tsconfig.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/set-function-name/package.json
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/set-function-name/tsconfig.json
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/shebang-command/package.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/shebang-regex/package.json
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/side-channel/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/side-channel/tsconfig.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/side-channel/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/side-channel/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/siginfo/package.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/signal-exit/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/signal-exit/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/signal-exit/dist/mjs/package.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/size-sensor/package.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/source-map/package.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/source-map-js/package.json
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/stackback/package.json
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/std-env/package.json
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string-width/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string-width/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string-width/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string-width-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string.prototype.trim/package.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string.prototype.trimend/package.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/string.prototype.trimstart/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/strip-ansi-cjs/package.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/strip-final-newline/package.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/strip-json-comments/package.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/strip-literal/package.json
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/commander/package.json
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/glob/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/glob/dist/esm/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/supports-preserve-symlinks-flag/package.json
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tailwindcss/package.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tailwindcss/stubs/.prettierrc.json
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tape/package.json
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/terser/package.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/terser/bin/package.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/terser/dist/package.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/terser/node_modules/commander/package.json
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/terser/node_modules/source-map/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/terser/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/text-segmentation/package.json
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/text-table/package.json
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/thenify/package.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/thenify-all/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tinybench/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tinypool/package.json
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tinyspy/package.json
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tippy.js/package.json
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tippy.js/headless/package.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/to-regex-range/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ts-interface-checker/package.json
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/type-check/package.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/type-detect/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/type-fest/package.json
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-buffer/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-byte-offset/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-length/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/typed-array-length/tsconfig.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/ufo/package.json
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/uglify-js/package.json
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/uglify-js/node_modules/source-map/package.json
--rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/uglify-js/tools/domprops.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/uglify-to-browserify/package.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unbox-primitive/package.json
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unimport/package.json
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unimport/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unimport/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unimport/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin/package.json
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-auto-import/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-vue-components/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/update-browserslist-db/.devcontainer.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/update-browserslist-db/package.json
--rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/uri-js/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/util-deprecate/package.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/utrie/package.json
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vite/package.json
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vite/node_modules/rollup/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vite/node_modules/rollup/dist/es/package.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vite/types/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vite-node/package.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vite-plugin-json5/package.json
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vitest/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vitest/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue/compiler-sfc/package.json
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue/jsx-runtime/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue/server-renderer/package.json
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-eslint-parser/package.json
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-i18n/package.json
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-i18n/vetur/attributes.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-i18n/vetur/tags.json
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-router/package.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-router/vetur/attributes.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-router/vetur/tags.json
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-tippy/package.json
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-tippy/tsconfig.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-tippy/vetur/attributes.json
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/vue-tippy/vetur/tags.json
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/webpack-sources/package.json
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/webpack-virtual-modules/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/which/package.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/which-boxed-primitive/package.json
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/which-typed-array/package.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/which-typed-array/tsconfig.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/why-is-node-running/package.json
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/window-size/package.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/word-wrap/package.json
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wordwrap/package.json
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrap-ansi/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrap-ansi-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/wrappy/package.json
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/xml-name-validator/package.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/yaml/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/yaml/browser/package.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/yargs/package.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.6/node_modules/yocto-queue/package.json
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/__init__.py
--rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/env.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/error.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/package.json
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/package.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/cos.py
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/http.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/info.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/auth/__init__.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/auth/login.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/upload/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/api/upload/model.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cli/__init__.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cli/main.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cli/utils.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/__init__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/_log_collector.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/start_thread.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/task_types.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/utils.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/dog/README.md
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/dog/__init__.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/dog/log_sniffer.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/dog/metadata_handle.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/cloud/dog/sniffer_queue.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/compat/README.md
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/compat/server/controller/experiment.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/converter/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/converter/tfb/__init__.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/converter/tfb/_utils.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/converter/tfb/tfb_converter.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/converter/wb/__init__.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/converter/wb/wb_converter.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/__init__.py
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/callback_cloud.py
--rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/callback_local.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/config.py
--rw-r--r--   0        0        0    13030 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/sdk.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/settings.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/_utils.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/audio.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/base.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/chart.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/image.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/object_3d.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/text.py
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/video.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/utils_modules/__init__.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/utils_modules/bounding_boxes.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/modules/utils_modules/image_mask.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/run/__init__.py
--rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/run/callback.py
--rw-r--r--   0        0        0    16930 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/run/exp.py
--rw-r--r--   0        0        0    13553 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/run/main.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/run/operator.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/system/__init__.py
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/system/info.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/system/monitor.py
--rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/data/system/bin/apple_gpu_stats
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/__init__.py
--rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/callback.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/db_connect.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/error.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/model.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/table_config.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/docs/Errors.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/docs/README.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/migrate/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/migrate/chart.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/migrate/experiment.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/migrate/namespace.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/migrate/project.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/migrate/tag.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/__init__.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/charts.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/displays.py
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/experiments.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/namespaces.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/projects.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/sources.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/models/tags.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/utils/__init__.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/db/utils/chart.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/fastai.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/huggingface.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/mmengine.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/pytorch_lightning.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/sb3.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/ultralytics.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/integration_utils/autologging.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/integration_utils/get_modules.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/integration_utils/timer.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/openai/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/openai/openai.py
--rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/openai/resolver.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/zhipuai/__init__.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/zhipuai/resolver.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/integration/zhipuai/zhipuai.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/log/__init__.py
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/log/console.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/log/log.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/app.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/settings.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/chart.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/db.py
--rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/experiment.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/namespace.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/project.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/utils/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/utils/charts.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/controller/utils/tag.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/middleware/common.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/module/__init__.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/module/resp.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/router/chart.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/router/experiment.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/router/media.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/router/namespace.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/server/router/project.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/index.html
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/ChartPage-C2Rj7xI3.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/ChartPage-DgOOkrVh.css
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/ChartsView-DpI6U3QH.js
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvHardware-4H7mp2Bs.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvIndex-B5_l1b65.js
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvItems-B4PwmQT4.js
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvItems-BfjcRO-X.css
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/ExperimentView-BTbu21ka.js
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/ExperimentView-CCDMXo4h.css
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/FuncBar-Ct_nBdvU.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/FuncBar-DgVTuZfd.css
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/HelpView-C4wSXY1I.js
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/HomeView-BS7FyMAt.css
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/HomeView-BqTu9_fG.js
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/IndexPage-C5dvtib2.css
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/IndexPage-CrqN4Ekl.js
--rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/LogPage-B-fC6sB7.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/LogPage-DBzoauOW.css
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/NotFound-DijsQ96i.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/SLLoading-6DfF2aH0.js
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js
--rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
--rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/chart-DB312WPs.css
--rw-r--r--   0        0        0  1098521 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/chart-eW1meEc1.js
--rw-r--r--   0        0        0   393892 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/index-B5SDzoY4.js
--rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/index-B7Izi8NT.css
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/template/assets/logo-ChHf2ozk.ico
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/utils/__init__.py
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/utils/file.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/utils/font.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/utils/judgment.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/utils/key.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.6/swanlab/utils/time.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/create_error_chart.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/create_experiment.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/start_server.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/use_swanlog.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/config/config.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/config/load.yaml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/.gitignore
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/fastai/fastai_train.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/fastai/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/huggingface/requirements.txt
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/huggingface/transformers_bert_train.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/lightning/lightning_base.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/lightning/lightning_train.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/lightning/requirements.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/sb3/requirements.txt
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/sb3/sb3_PPO.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/ultralytics/requirements.txt
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/ultralytics/ultralytics_classifer.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/ultralytics/ultralytics_detection.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/ultralytics/ultralytics_pose.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/integration/ultralytics/ultralytics_segmentation.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/conftest.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/pytest_env.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/pytest_example.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/auth/pytest_login.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/data/pytest_sdk.py
--rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/data/run/pytest_main.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/log/pytest_log.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/server/controller/utils/utils.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/utils/pytest_file.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/utils/pytest_key.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 swanlab-0.3.6/test/unit/utils/pytest_package.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 swanlab-0.3.6/.gitignore
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.6/LICENSE
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    31011 2020-02-02 00:00:00.000000 swanlab-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.7/.eslintrc-auto-import.json
+-rw-r--r--   0        0        0    22389 2020-02-02 00:00:00.000000 swanlab-0.3.7/README.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.7/jsconfig.json
+-rw-r--r--   0        0        0   236756 2020-02-02 00:00:00.000000 swanlab-0.3.7/package-lock.json
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.7/package.json
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.7/.config/copy_frontend.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.7/.vscode/extensions.json
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 swanlab-0.3.7/.vscode/launch.json
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.7/.vscode/settings.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.7/.vscode/tailwind.json
+-rw-r--r--   0        0        0   218889 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/.package-lock.json
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@alloc/quick-lru/package.json
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antfu/utils/package.json
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/adjust/package.json
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/adjust/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/attr/package.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/color-util/package.json
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/component/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/component/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/coord/package.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/dom-util/package.json
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/event-emitter/package.json
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-base/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-canvas/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-math/package.json
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g-svg/package.json
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g2/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/g2plot/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/scale/package.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@antv/util/package.json
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@babel/parser/package.json
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@esbuild/linux-x64/package.json
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@eslint/eslintrc/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@eslint/js/package.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@eslint-community/eslint-utils/package.json
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@eslint-community/regexpp/package.json
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@headlessui/vue/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@humanwhocodes/config-array/package.json
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@humanwhocodes/module-importer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@humanwhocodes/object-schema/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@intlify/core-base/package.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@intlify/message-compiler/package.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@intlify/shared/package.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@isaacs/cliui/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@jest/schemas/package.json
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@jridgewell/gen-mapping/package.json
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@jridgewell/resolve-uri/package.json
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@jridgewell/set-array/package.json
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@jridgewell/source-map/package.json
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@jridgewell/sourcemap-codec/package.json
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@jridgewell/trace-mapping/package.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@ljharb/resumer/package.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@ljharb/through/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@ljharb/through/tsconfig.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@nodelib/fs.scandir/package.json
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@nodelib/fs.stat/package.json
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@nodelib/fs.walk/package.json
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@pkgjs/parseargs/package.json
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@popperjs/core/package.json
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@rollup/pluginutils/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@rollup/pluginutils/dist/es/package.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@rollup/rollup-linux-x64-gnu/package.json
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@rollup/rollup-linux-x64-musl/package.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@sinclair/typebox/package.json
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@tanstack/virtual-core/package.json
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@tanstack/vue-virtual/package.json
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@types/d3-timer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@types/estree/package.json
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@ungap/structured-clone/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@ungap/structured-clone/cjs/package.json
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitejs/plugin-vue/package.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/expect/package.json
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/runner/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/runner/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/snapshot/package.json
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/spy/package.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/utils/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vitest/utils/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/compiler-core/package.json
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/compiler-dom/package.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/compiler-ssr/package.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/devtools-api/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/reactivity/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/runtime-core/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/runtime-dom/package.json
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/server-renderer/package.json
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/@vue/shared/package.json
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/acorn/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/acorn-jsx/package.json
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/acorn-walk/package.json
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ajv/package.json
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ajv/lib/refs/data.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-draft-04.json
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-draft-06.json
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-draft-07.json
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-secure.json
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/align-text/package.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/amdefine/package.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/any-promise/package.json
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/anymatch/package.json
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/arg/package.json
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/argparse/package.json
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/array-buffer-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/array-buffer-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/arraybuffer.prototype.slice/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/assertion-error/package.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/asynckit/package.json
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/autoprefixer/package.json
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/available-typed-arrays/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/available-typed-arrays/tsconfig.json
+-rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/axios/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/balanced-match/package.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/base64-arraybuffer/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/binary-extensions/binary-extensions.json
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/binary-extensions/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/boolbase/package.json
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/braces/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/browserslist/package.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/buffer-from/package.json
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/cac/package.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/call-bind/package.json
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/callsites/package.json
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/camelcase/package.json
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/camelcase-css/package.json
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/caniuse-lite/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/center-align/package.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/chai/bower.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/chai/package.json
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/chalk/package.json
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/check-error/package.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/chokidar/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/chokidar/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/cliui/package.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/color-convert/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/color-name/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/combined-stream/package.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/commander/package-support.json
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/commander/package.json
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/concat-map/package.json
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/confbox/package.json
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/contour_plot/package.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/cross-spawn/package.json
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/css-line-break/package.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/cssesc/package.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/csstype/package.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/d3-color/package.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/d3-ease/package.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/d3-hierarchy/package.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/d3-interpolate/package.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/d3-regression/package.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/d3-timer/package.json
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/data-view-buffer/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/data-view-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/data-view-byte-length/package.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/data-view-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/data-view-byte-offset/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/data-view-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/debug/package.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/decamelize/package.json
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/deep-eql/package.json
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/deep-equal/package.json
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/deep-is/package.json
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/define-data-property/package.json
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/define-data-property/tsconfig.json
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/define-properties/package.json
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/defined/package.json
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/delayed-stream/package.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/detect-browser/package.json
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/didyoumean/package.json
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/diff-sequences/package.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/dlv/package.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/doctrine/package.json
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/dotignore/package.json
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eastasianwidth/package.json
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/electron-to-chromium/chromium-versions.json
+-rw-r--r--   0        0        0    50619 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/electron-to-chromium/full-chromium-versions.json
+-rw-r--r--   0        0        0    79153 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/electron-to-chromium/full-versions.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/electron-to-chromium/package.json
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/electron-to-chromium/versions.json
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/entities/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/entities/lib/esm/package.json
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-abstract/package.json
+-rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-abstract/helpers/caseFolding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-abstract/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-abstract/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-define-property/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-define-property/tsconfig.json
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-errors/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-errors/tsconfig.json
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-object-atoms/package.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-object-atoms/tsconfig.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-set-tostringtag/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-set-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/es-to-primitive/package.json
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/esbuild/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/escalade/package.json
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint/conf/replacements.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint/conf/rule-type-list.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-config-prettier/package.json
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-prettier/package.json
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/package.json
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
+-rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/math-elements.json
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-scope/package.json
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/eslint-visitor-keys/package.json
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/espree/package.json
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/esquery/package.json
+-rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/esrecurse/package.json
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/estraverse/package.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/estree-walker/dist/esm/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/estree-walker/src/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/esutils/package.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/execa/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fast-deep-equal/package.json
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fast-diff/package.json
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fast-glob/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fast-glob/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fast-json-stable-stringify/package.json
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fast-json-stable-stringify/benchmark/test.json
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fast-levenshtein/package.json
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fastq/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fastq/test/tsconfig.json
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fecha/package.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/file-entry-cache/package.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fill-range/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/find-up/package.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/flat-cache/package.json
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/flatted/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/flatted/cjs/package.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fmin/.eslintrc.json
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fmin/package.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/follow-redirects/package.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/for-each/package.json
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/foreground-child/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/foreground-child/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/foreground-child/dist/mjs/package.json
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/form-data/package.json
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fraction.js/package.json
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/fs.realpath/package.json
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/function-bind/package.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/function.prototype.name/package.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/functions-have-names/package.json
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/get-func-name/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/get-intrinsic/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/get-stream/package.json
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/get-symbol-description/package.json
+-rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/mat2/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/mat2d/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/mat3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/mat4/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/quat/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/quat2/package.json
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/types.d.ts/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/vec2/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/vec3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gl-matrix/vec4/package.json
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/glob/package.json
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/globals/globals.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/globals/package.json
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/globalthis/package.json
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/gopd/package.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/graphemer/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has/package.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-ansi/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-bigints/package.json
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-flag/package.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-property-descriptors/package.json
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-proto/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-proto/tsconfig.json
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-symbols/package.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-tostringtag/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/has-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/hasown/package.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/hasown/tsconfig.json
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/html2canvas/package.json
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/html2canvas/tsconfig.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/human-signals/package.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/husky/package.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ignore/package.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/immutable/package.json
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/import-fresh/package.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/imurmurhash/package.json
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/inflight/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/inherits/package.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/internal-slot/package.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-arguments/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-bigint/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-binary-path/package.json
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-boolean-object/package.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-buffer/package.json
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-callable/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-core-module/core.json
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-core-module/package.json
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-data-view/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-data-view/tsconfig.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-date-object/package.json
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-extglob/package.json
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-fullwidth-code-point/package.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-glob/package.json
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-negative-zero/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-negative-zero/tsconfig.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-number/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-number-object/package.json
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-path-inside/package.json
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-regex/package.json
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-shared-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-shared-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-stream/package.json
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-string/package.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-symbol/package.json
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-typed-array/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-typed-array/tsconfig.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/is-weakref/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/isarray/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/isexe/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/jackspeak/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/jackspeak/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/jackspeak/dist/esm/package.json
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/jiti/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/js-tokens/package.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/js-yaml/package.json
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/json-buffer/package.json
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/json-schema-traverse/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/json-stable-stringify-without-jsonify/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/json2module/package.json
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/json5/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/keyv/package.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/kind-of/package.json
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lazy-cache/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/levn/package.json
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lines-and-columns/package.json
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/locate-path/package.json
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lodash/package.json
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lodash-es/package.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lodash.merge/package.json
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/longest/package.json
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/loupe/package.json
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lru-cache/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lru-cache/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/lru-cache/dist/esm/package.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/magic-string/package.json
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/merge-stream/package.json
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/merge2/package.json
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/micromatch/package.json
+-rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mime-db/db.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mime-db/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mime-types/package.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mimic-fn/package.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/minimist/package.json
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/minipass/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/minipass/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/minipass/dist/esm/package.json
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mlly/package.json
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mock-property/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mockjs/bower.json
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mockjs/package.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mockjs/test/bower.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mockjs/test/package.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/moment/package.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ms/package.json
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/mz/package.json
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/nanoid/package.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/nanoid/async/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/nanoid/non-secure/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/nanoid/url-alphabet/package.json
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/natural-compare/package.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/node-releases/package.json
+-rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/node-releases/data/processed/envs.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/node-releases/data/release-schedule/release-schedule.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/normalize-path/package.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/normalize-range/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/npm-run-path/package.json
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/npm-run-path/node_modules/path-key/package.json
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/nth-check/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/nth-check/lib/esm/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/object-assign/package.json
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/object-hash/package.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/object-is/package.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/object-keys/package.json
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/object.assign/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/once/package.json
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/onetime/package.json
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/optionator/package.json
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/p-locate/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/parent-module/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/path-exists/package.json
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/path-is-absolute/package.json
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/path-key/package.json
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/path-parse/package.json
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/path-scurry/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/path-scurry/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/path-scurry/dist/esm/package.json
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pathe/package.json
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pathval/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pdfast/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/picocolors/package.json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/picomatch/package.json
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pify/package.json
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pinia/package.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pinia/node_modules/vue-demi/package.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pirates/package.json
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pkg-types/package.json
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/possible-typed-array-names/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/possible-typed-array-names/tsconfig.json
+-rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss-import/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss-js/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss-load-config/package.json
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss-load-config/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss-nested/package.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss-selector-parser/package.json
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/postcss-value-parser/package.json
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/prelude-ls/package.json
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/prettier/package.json
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/prettier-linter-helpers/package.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/prettier-linter-helpers/.vscode/settings.json
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pretty-format/package.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/pretty-format/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/proxy-from-env/package.json
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/punycode/package.json
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/queue-microtask/package.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/react-is/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/read-cache/package.json
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/readdirp/package.json
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/regexp.prototype.flags/package.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/repeat-string/package.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/lib/core.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/baz/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/browser_field/package.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/dot_main/package.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/dot_slash_main/package.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/false_main/package.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/incorrect_main/package.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/invalid_main/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/multirepo/lerna.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/multirepo/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve/test/resolver/symlinked/package/package.json
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/resolve-from/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/reusify/package.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/right-align/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rimraf/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rollup/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rollup/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rollup/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rollup/node_modules/chalk/package.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rollup/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rollup/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rollup/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/run-parallel/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/rw/package.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/safe-array-concat/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/safe-array-concat/tsconfig.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/safe-regex-test/package.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sass/package.json
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/scule/package.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/semver/package.json
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/set-function-length/package.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/set-function-length/tsconfig.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/set-function-name/package.json
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/set-function-name/tsconfig.json
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/shebang-command/package.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/shebang-regex/package.json
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/side-channel/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/side-channel/tsconfig.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/side-channel/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/side-channel/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/siginfo/package.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/signal-exit/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/signal-exit/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/signal-exit/dist/mjs/package.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/size-sensor/package.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/source-map/package.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/source-map-js/package.json
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/stackback/package.json
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/std-env/package.json
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string-width/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string-width/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string-width-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string.prototype.trim/package.json
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string.prototype.trimend/package.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/string.prototype.trimstart/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/strip-ansi-cjs/package.json
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/strip-final-newline/package.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/strip-json-comments/package.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/strip-literal/package.json
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/glob/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/glob/dist/esm/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/supports-preserve-symlinks-flag/package.json
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tailwindcss/package.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tailwindcss/stubs/.prettierrc.json
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tape/package.json
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/terser/package.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/terser/bin/package.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/terser/dist/package.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/terser/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/terser/node_modules/source-map/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/terser/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/text-segmentation/package.json
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/text-table/package.json
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/thenify/package.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/thenify-all/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tinybench/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tinypool/package.json
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tinyspy/package.json
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tippy.js/package.json
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tippy.js/headless/package.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/to-regex-range/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ts-interface-checker/package.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/type-check/package.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/type-detect/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/type-fest/package.json
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-buffer/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-byte-offset/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-length/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/typed-array-length/tsconfig.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/ufo/package.json
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/uglify-js/package.json
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/uglify-js/node_modules/source-map/package.json
+-rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/uglify-js/tools/domprops.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/uglify-to-browserify/package.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unbox-primitive/package.json
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unimport/package.json
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unimport/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unimport/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unimport/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin/package.json
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-auto-import/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-vue-components/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/update-browserslist-db/.devcontainer.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/update-browserslist-db/package.json
+-rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/uri-js/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/util-deprecate/package.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/utrie/package.json
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vite/package.json
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vite/node_modules/rollup/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vite/node_modules/rollup/dist/es/package.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vite/types/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vite-node/package.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vite-plugin-json5/package.json
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vitest/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vitest/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue/jsx-runtime/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue/server-renderer/package.json
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-eslint-parser/package.json
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-i18n/package.json
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-i18n/vetur/attributes.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-i18n/vetur/tags.json
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-router/package.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-router/vetur/attributes.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-router/vetur/tags.json
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-tippy/package.json
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-tippy/tsconfig.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-tippy/vetur/attributes.json
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/vue-tippy/vetur/tags.json
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/webpack-sources/package.json
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/webpack-virtual-modules/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/which/package.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/which-boxed-primitive/package.json
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/which-typed-array/package.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/which-typed-array/tsconfig.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/why-is-node-running/package.json
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/window-size/package.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/word-wrap/package.json
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wordwrap/package.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrap-ansi/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrap-ansi-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/wrappy/package.json
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/xml-name-validator/package.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/yaml/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/yaml/browser/package.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/yargs/package.json
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.7/node_modules/yocto-queue/package.json
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/__init__.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/env.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/error.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/package.json
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/package.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/__init__.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/cos.py
+-rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/http.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/info.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/auth/__init__.py
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/auth/login.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/upload/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/api/upload/model.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cli/__init__.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cli/main.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cli/utils.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/__init__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/_log_collector.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/start_thread.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/task_types.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/utils.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/dog/README.md
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/dog/__init__.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/dog/log_sniffer.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/dog/metadata_handle.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/cloud/dog/sniffer_queue.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/compat/README.md
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/compat/server/controller/experiment.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/converter/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/converter/tfb/__init__.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/converter/tfb/_utils.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/converter/tfb/tfb_converter.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/converter/wb/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/converter/wb/wb_converter.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/__init__.py
+-rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/callback_cloud.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/callback_local.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/config.py
+-rw-r--r--   0        0        0    13030 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/sdk.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/settings.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/_utils.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/audio.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/base.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/chart.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/image.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/object_3d.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/text.py
+-rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/video.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/utils_modules/__init__.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/utils_modules/bounding_boxes.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/modules/utils_modules/image_mask.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/run/__init__.py
+-rw-r--r--   0        0        0     8509 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/run/callback.py
+-rw-r--r--   0        0        0    17302 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/run/exp.py
+-rw-r--r--   0        0        0    13553 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/run/main.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/run/operator.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/system/__init__.py
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/system/info.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/system/monitor.py
+-rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/data/system/bin/apple_gpu_stats
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/__init__.py
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/callback.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/db_connect.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/error.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/model.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/table_config.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/docs/Errors.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/docs/README.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/migrate/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/migrate/chart.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/migrate/experiment.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/migrate/namespace.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/migrate/project.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/migrate/tag.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/__init__.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/charts.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/displays.py
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/experiments.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/namespaces.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/projects.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/sources.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/models/tags.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/utils/__init__.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/db/utils/chart.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/fastai.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/huggingface.py
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/mmengine.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/pytorch_lightning.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/sb3.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/ultralytics.py
+-rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/integration_utils/autologging.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/integration_utils/get_modules.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/integration_utils/timer.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/openai/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/openai/openai.py
+-rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/openai/resolver.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/zhipuai/__init__.py
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/zhipuai/resolver.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/integration/zhipuai/zhipuai.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/log/__init__.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/log/console.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/log/log.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/app.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/settings.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/chart.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/db.py
+-rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/experiment.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/namespace.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/project.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/utils/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/utils/charts.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/controller/utils/tag.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/middleware/common.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/module/__init__.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/module/resp.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/router/chart.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/router/experiment.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/router/media.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/router/namespace.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/server/router/project.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/index.html
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/ChartPage-BqfnvJQ4.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/ChartPage-DgOOkrVh.css
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/ChartsView-DKnkZV4x.js
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvHardware-Dh6G7EyN.js
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvIndex-3qdPSvC8.js
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvItems-BfjcRO-X.css
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvItems-z9WBoR8b.js
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvRequirements-B26RqDqU.js
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/EnvironmentPage-DLnE8Co5.js
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/ExperimentView-CCDMXo4h.css
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/ExperimentView-x-2IwSHi.js
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/FuncBar-Chts8yho.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/FuncBar-DgVTuZfd.css
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/HelpView-BS1FZ4Nz.js
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/HomeView-BS7FyMAt.css
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/HomeView-uDUGPxwP.js
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/IndexPage-C5dvtib2.css
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/IndexPage-Jy4F58Oh.js
+-rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/LogPage-D3SdB10-.js
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/LogPage-DBzoauOW.css
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/NotFound-Dt02Ekhs.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/SLLoading-B-49YNim.js
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/SLStatusLabel-DNkFoo89.js
+-rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/chart-B9MmDiWI.css
+-rw-r--r--   0        0        0  1098733 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/chart-Cb2YjpB3.js
+-rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/index-B7Izi8NT.css
+-rw-r--r--   0        0        0   393925 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/index-CmcaZNbV.js
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/template/assets/logo-ChHf2ozk.ico
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/utils/__init__.py
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/utils/file.py
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/utils/font.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/utils/judgment.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/utils/key.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.7/swanlab/utils/time.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/create_error_chart.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/create_experiment.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/start_server.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/use_swanlog.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/config/config.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/config/load.yaml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/.gitignore
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/fastai/fastai_train.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/fastai/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/huggingface/requirements.txt
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/huggingface/transformers_bert_train.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/lightning/lightning_base.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/lightning/lightning_train.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/lightning/requirements.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/sb3/requirements.txt
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/sb3/sb3_PPO.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/ultralytics/requirements.txt
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/ultralytics/ultralytics_classifer.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/ultralytics/ultralytics_detection.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/ultralytics/ultralytics_pose.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/integration/ultralytics/ultralytics_segmentation.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/conftest.py
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/pytest_env.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/pytest_example.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/pytest_package.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/api/pytest_http.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/api/auth/pytest_login.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/data/pytest_sdk.py
+-rw-r--r--   0        0        0    21785 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/data/run/pytest_main.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/log/pytest_log.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/server/controller/utils/utils.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/utils/pytest_file.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.7/test/unit/utils/pytest_key.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 swanlab-0.3.7/.gitignore
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.7/LICENSE
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    24526 2020-02-02 00:00:00.000000 swanlab-0.3.7/PKG-INFO
```

### Comparing `swanlab-0.3.6/.eslintrc-auto-import.json` & `swanlab-0.3.7/.eslintrc-auto-import.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/README.md` & `swanlab-0.3.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,1805 +1,1533 @@
-00000000: 215b 4f76 6572 7669 6577 5d28 7265 6164  ![Overview](read
-00000010: 6d65 5f66 696c 6573 2f73 7761 6e6c 6162  me_files/swanlab
-00000020: 2d6f 7665 7276 6965 772d 6e65 772e 706e  -overview-new.pn
-00000030: 6729 0a0a 3c70 2061 6c69 676e 3d22 6365  g)..<p align="ce
-00000040: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
-00000050: 6874 7470 733a 2f2f 7377 616e 6c61 622e  https://swanlab.
-00000060: 636e 223e 5377 616e 4c61 6220 436c 6f75  cn">SwanLab Clou
-00000070: 643c 2f61 3e20 c2b7 203c 6120 6872 6566  d</a> .. <a href
-00000080: 3d22 6874 7470 733a 2f2f 646f 6373 2e73  ="https://docs.s
-00000090: 7761 6e6c 6162 2e63 6e22 3e44 6f63 756d  wanlab.cn">Docum
-000000a0: 656e 743c 2f61 3e20 c2b7 203c 6120 6872  ent</a> .. <a hr
-000000b0: 6566 3d22 6874 7470 733a 2f2f 6765 656b  ef="https://geek
-000000c0: 7465 6368 7374 7564 696f 2e66 6569 7368  techstudio.feish
-000000d0: 752e 636e 2f77 696b 692f 4e49 5a39 7770  u.cn/wiki/NIZ9wp
-000000e0: 354c 5269 5371 5179 6b69 7a62 4763 567a  5LRiSqQykizbGcVz
-000000f0: 554b 6e69 6322 3e57 6543 6861 743c 2f61  UKnic">WeChat</a
-00000100: 3e20 c2b7 203c 6120 6872 6566 3d22 6874  > .. <a href="ht
-00000110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000120: 2f73 7761 6e68 7562 782f 7377 616e 6c61  /swanhubx/swanla
-00000130: 622f 6973 7375 6573 223e 5265 706f 7274  b/issues">Report
-00000140: 2049 7373 7565 3c2f 613e 20c2 b720 3c61   Issue</a> .. <a
-00000150: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000160: 6565 6b74 6563 6873 7475 6469 6f2e 6665  eektechstudio.fe
-00000170: 6973 6875 2e63 6e2f 7368 6172 652f 6261  ishu.cn/share/ba
-00000180: 7365 2f66 6f72 6d2f 7368 7263 6e79 426c  se/form/shrcnyBl
-00000190: 4b38 4f4d 4430 6577 656f 4663 6332 5376  K8OMD0eweoFcc2Sv
-000001a0: 574b 6322 3e46 6565 6462 6163 6b3c 2f61  WKc">Feedback</a
-000001b0: 3e20 c2b7 203c 6120 6872 6566 3d22 6874  > .. <a href="ht
-000001c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000001d0: 2f53 7761 6e48 7562 582f 5377 616e 4c61  /SwanHubX/SwanLa
-000001e0: 622f 626c 6f62 2f6d 6169 6e2f 4348 414e  b/blob/main/CHAN
-000001f0: 4745 4c4f 472e 6d64 223e 4368 616e 6765  GELOG.md">Change
-00000200: 6c6f 673c 2f61 3e0a 0a0a 3c2f 703e 0a0a  log</a>...</p>..
-00000210: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000220: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
-00000230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000240: 2f53 7761 6e48 7562 582f 5377 616e 4c61  /SwanHubX/SwanLa
-00000250: 622f 626c 6f62 2f6d 6169 6e2f 4c49 4345  b/blob/main/LICE
-00000260: 4e53 4522 3e3c 696d 6720 7372 633d 2268  NSE"><img src="h
-00000270: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000280: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
-00000290: 656e 7365 2f53 7761 6e48 7562 582f 5377  ense/SwanHubX/Sw
-000002a0: 616e 4c61 622e 7376 673f 636f 6c6f 723d  anLab.svg?color=
-000002b0: 6272 6967 6874 6772 6565 6e22 2061 6c74  brightgreen" alt
-000002c0: 3d22 6c69 6365 6e73 6522 3e3c 2f61 3e0a  ="license"></a>.
-000002d0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-000002e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5377  ://github.com/Sw
-000002f0: 616e 4875 6258 2f53 7761 6e4c 6162 2f63  anHubX/SwanLab/c
-00000300: 6f6d 6d69 7473 2f6d 6169 6e22 3e3c 696d  ommits/main"><im
-00000310: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000320: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00000330: 7468 7562 2f6c 6173 742d 636f 6d6d 6974  thub/last-commit
-00000340: 2f53 7761 6e48 7562 582f 5377 616e 4c61  /SwanHubX/SwanLa
-00000350: 6222 2061 6c74 3d22 6c69 6365 6e73 6522  b" alt="license"
-00000360: 3e3c 2f61 3e0a 2020 3c61 2068 7265 663d  ></a>.  <a href=
-00000370: 2268 7474 7073 3a2f 2f70 7970 692e 7079  "https://pypi.py
-00000380: 7468 6f6e 2e6f 7267 2f70 7970 692f 7377  thon.org/pypi/sw
-00000390: 616e 6c61 6222 3e3c 696d 6720 7372 633d  anlab"><img src=
-000003a0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000003b0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f73  elds.io/pypi/v/s
-000003c0: 7761 6e6c 6162 3f63 6f6c 6f72 3d6f 7261  wanlab?color=ora
-000003d0: 6e67 6522 2061 6c74 3d20 2f3e 3c2f 613e  nge" alt= /></a>
-000003e0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-000003f0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
-00000400: 6f6a 6563 742f 7377 616e 6c61 6222 3e3c  oject/swanlab"><
-00000410: 696d 6720 616c 743d 2270 7970 6920 446f  img alt="pypi Do
-00000420: 776e 6c6f 6164 2220 7372 633d 2268 7474  wnload" src="htt
-00000430: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
-00000440: 2e74 6563 682f 6261 6467 652f 7377 616e  .tech/badge/swan
-00000450: 6c61 6222 3e3c 2f61 3e0a 2020 3c61 2068  lab"></a>.  <a h
-00000460: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000470: 6875 622e 636f 6d2f 7377 616e 6875 6278  hub.com/swanhubx
-00000480: 2f73 7761 6e6c 6162 2f69 7373 7565 7322  /swanlab/issues"
-00000490: 3e3c 696d 6720 616c 743d 2269 7373 7565  ><img alt="issue
-000004a0: 7322 2073 7263 3d22 6874 7470 733a 2f2f  s" src="https://
-000004b0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-000004c0: 6974 6875 622f 6973 7375 6573 2f73 7761  ithub/issues/swa
-000004d0: 6e68 7562 782f 7377 616e 6c61 6222 3e3c  nhubx/swanlab"><
-000004e0: 2f61 3e0a 2020 3c62 723e 0a20 203c 6120  /a>.  <br>.  <a 
-000004f0: 6872 6566 3d22 6874 7470 733a 2f2f 7377  href="https://sw
-00000500: 616e 6c61 622e 636e 2220 7461 7267 6574  anlab.cn" target
-00000510: 3d22 5f62 6c61 6e6b 223e 0a20 2020 2020  ="_blank">.     
-00000520: 2020 203c 696d 6720 616c 743d 2253 7461     <img alt="Sta
-00000530: 7469 6320 4261 6467 6522 2073 7263 3d22  tic Badge" src="
-00000540: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000550: 6c64 732e 696f 2f62 6164 6765 2f50 726f  lds.io/badge/Pro
-00000560: 6475 6374 2d53 7761 6e4c 6162 e4ba 91e7  duct-SwanLab....
-00000570: abaf e789 882d 3633 3661 3366 223e 3c2f  .....-636a3f"></
-00000580: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
-00000590: 7470 733a 2f2f 6765 656b 7465 6368 7374  tps://geektechst
-000005a0: 7564 696f 2e66 6569 7368 752e 636e 2f77  udio.feishu.cn/w
-000005b0: 696b 692f 4e49 5a39 7770 354c 5269 5371  iki/NIZ9wp5LRiSq
-000005c0: 5179 6b69 7a62 4763 567a 554b 6e69 6322  QykizbGcVzUKnic"
-000005d0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000005e0: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
-000005f0: 6c74 3d22 5374 6174 6963 2042 6164 6765  lt="Static Badge
-00000600: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000610: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000620: 6467 652f 5765 4368 6174 2de5 beae e4bf  dge/WeChat-.....
-00000630: a12d 3463 6235 3565 223e 3c2f 613e 0a20  .-4cb55e"></a>. 
-00000640: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000650: 2f2f 7777 772e 7869 616f 686f 6e67 7368  //www.xiaohongsh
-00000660: 752e 636f 6d2f 7573 6572 2f70 726f 6669  u.com/user/profi
-00000670: 6c65 2f36 3035 3738 3662 3930 3030 3030  le/605786b900000
-00000680: 3030 3030 3130 3033 6138 3122 2074 6172  00001003a81" tar
-00000690: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
-000006a0: 2020 2020 2020 3c69 6d67 2061 6c74 3d22        <img alt="
-000006b0: 5374 6174 6963 2042 6164 6765 2220 7372  Static Badge" sr
-000006c0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000006d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000006e0: e5b0 8fe7 baa2 e4b9 a62d 4630 3434 3338  .........-F04438
-000006f0: 223e 3c2f 613e 0a0a 3c2f 703e 0a0a 3c64  "></a>..</p>..<d
-00000700: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-00000710: 223e 0a20 203c 6120 6872 6566 3d22 2e2f  ">.  <a href="./
-00000720: 5245 4144 4d45 2e6d 6422 3e3c 696d 6720  README.md"><img 
-00000730: 616c 743d 22e8 8bb1 e696 87e6 9687 e6a1  alt="...........
-00000740: a322 2073 7263 3d22 6874 7470 733a 2f2f  ." src="https://
-00000750: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000760: 6164 6765 2f45 6e67 6c69 7368 2d64 3964  adge/English-d9d
-00000770: 3964 3922 3e3c 2f61 3e0a 2020 3c61 2068  9d9"></a>.  <a h
-00000780: 7265 663d 222e 2f52 4541 444d 455f 636e  ref="./README_cn
-00000790: 2e6d 6422 3e3c 696d 6720 616c 743d 22e4  .md"><img alt=".
-000007a0: b8ad e696 87e6 9687 e6a1 a322 2073 7263  ..........." src
-000007b0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000007c0: 6965 6c64 732e 696f 2f62 6164 6765 2fe7  ields.io/badge/.
-000007d0: ae80 e4bd 93e4 b8ad e696 872d 6439 6439  ...........-d9d9
-000007e0: 6439 223e 3c2f 613e 0a3c 2f64 6976 3e0a  d9"></a>.</div>.
-000007f0: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
-00000800: 6172 793e 5461 626c 6520 6f66 2063 6f6e  ary>Table of con
-00000810: 7465 6e74 733c 2f73 756d 6d61 7279 3e0a  tents</summary>.
-00000820: 0a23 2323 2320 544f 430a 0a2d 205b f09f  .#### TOC..- [..
-00000830: 918b f09f 8fbb 2049 6e74 726f 6475 6374  ...... Introduct
-00000840: 696f 6e5d 2823 2d49 6e74 726f 6475 6374  ion](#-Introduct
-00000850: 696f 6e29 0a2d 205b f09f 8f81 2051 7569  ion).- [.... Qui
-00000860: 636b 2053 7461 7274 5d28 23f0 9f8f 812d  ck Start](#....-
-00000870: 7175 6963 6b2d 7374 6172 7429 0a20 2020  quick-start).   
-00000880: 202d 205b 312e 496e 7374 616c 6c61 7469   - [1.Installati
-00000890: 6f6e 5d28 2331 696e 7374 616c 6c61 7469  on](#1installati
-000008a0: 6f6e 290a 2020 2020 2d20 5b32 2e4c 6f67  on).    - [2.Log
-000008b0: 2049 6e20 616e 6420 4765 7420 7468 6520   In and Get the 
-000008c0: 4150 4920 4b65 795d 2823 326c 6f67 2d69  API Key](#2log-i
-000008d0: 6e2d 616e 642d 6765 742d 7468 652d 6170  n-and-get-the-ap
-000008e0: 692d 6b65 7929 0a20 2020 202d 205b 332e  i-key).    - [3.
-000008f0: 496e 7465 6772 6174 6520 5377 616e 4c61  Integrate SwanLa
-00000900: 6220 7769 7468 2059 6f75 7220 436f 6465  b with Your Code
-00000910: 5d28 2333 2d69 6e74 6567 7261 7465 2d73  ](#3-integrate-s
-00000920: 7761 6e6c 6162 2d77 6974 682d 796f 7572  wanlab-with-your
-00000930: 2d63 6f64 6529 0a2d 205b f09f 9383 204d  -code).- [.... M
-00000940: 6f72 6520 4578 616d 706c 6573 5d28 232d  ore Examples](#-
-00000950: 6d6f 7265 2d65 7861 6d70 6c65 7329 0a2d  more-examples).-
-00000960: 205b f09f 92bb 2053 656c 662d 686f 7374   [.... Self-host
-00000970: 6564 5d28 232d 7365 6c66 2d68 6f73 7465  ed](#-self-hoste
-00000980: 6429 0a20 2020 202d 205b 4f66 666c 696e  d).    - [Offlin
-00000990: 6520 4578 7065 7269 6d65 6e74 2054 7261  e Experiment Tra
-000009a0: 636b 696e 675d 2823 6f66 666c 696e 652d  cking](#offline-
-000009b0: 6578 7065 7269 6d65 6e74 2d74 7261 636b  experiment-track
-000009c0: 696e 6729 0a20 2020 202d 205b 4f70 656e  ing).    - [Open
-000009d0: 204f 6666 6c69 6e65 2044 6173 6862 6f61   Offline Dashboa
-000009e0: 7264 5d28 236f 7065 6e2d 6f66 666c 696e  rd](#open-offlin
-000009f0: 652d 626f 6172 6429 0a2d 205b f09f 9a97  e-board).- [....
-00000a00: 2049 6e74 6567 7261 7469 6f6e 5d28 232d   Integration](#-
-00000a10: 696e 7465 6772 6174 696f 6e29 0a2d 205b  integration).- [
-00000a20: f09f 869a 2043 6f6d 7061 7269 736f 6e20  .... Comparison 
-00000a30: 7769 7468 2046 616d 696c 6961 7220 546f  with Familiar To
-00000a40: 6f6c 735d 2823 2d63 6f6d 7061 7269 736f  ols](#-compariso
-00000a50: 6e2d 7769 7468 2d66 616d 696c 6961 722d  n-with-familiar-
-00000a60: 746f 6f6c 7329 0a20 2020 202d 205b 5465  tools).    - [Te
-00000a70: 6e73 6f72 626f 6172 6420 7673 2053 7761  nsorboard vs Swa
-00000a80: 6e4c 6162 5d28 2374 656e 736f 7262 6f61  nLab](#tensorboa
-00000a90: 7264 2d76 732d 7377 616e 6c61 6229 0a20  rd-vs-swanlab). 
-00000aa0: 2020 202d 205b 5765 6967 6874 7320 2620     - [Weights & 
-00000ab0: 4269 6173 6573 2076 7320 5377 616e 4c61  Biases vs SwanLa
-00000ac0: 625d 2823 7765 6967 6874 732d 616e 642d  b](#weights-and-
-00000ad0: 6269 6173 6573 2d76 732d 7377 616e 6c61  biases-vs-swanla
-00000ae0: 6229 0a2d 205b f09f 9ba3 efb8 8f20 526f  b).- [....... Ro
-00000af0: 6164 6d61 705d 2823 2545 4625 4238 2538  admap](#%EF%B8%8
-00000b00: 462d 726f 6164 6d61 7029 0a20 2020 202d  F-roadmap).    -
-00000b10: 205b 496e 2050 726f 6772 6573 7320 4e6f   [In Progress No
-00000b20: 775d 2823 696e 2d70 726f 6772 6573 732d  w](#in-progress-
-00000b30: 6e6f 7729 0a20 2020 202d 205b 4e65 7874  now).    - [Next
-00000b40: 2050 6c61 6e6e 6564 5d28 236e 6578 742d   Planned](#next-
-00000b50: 706c 616e 6e65 6429 0a20 2020 202d 205b  planned).    - [
-00000b60: 4c6f 6e67 2054 6572 6d20 436f 6e63 6572  Long Term Concer
-00000b70: 6e5d 2823 6c6f 6e67 2d74 6572 6d2d 636f  n](#long-term-co
-00000b80: 6e63 6572 6e29 0a2d 205b f09f 91a5 2043  ncern).- [.... C
-00000b90: 6f6d 6d75 6e69 7479 5d28 232d 636f 6d6d  ommunity](#-comm
-00000ba0: 756e 6974 7929 0a20 2020 202d 205b 436f  unity).    - [Co
-00000bb0: 6d6d 756e 6974 7920 616e 6420 5375 7070  mmunity and Supp
-00000bc0: 6f72 745d 2823 636f 6d6d 756e 6974 792d  ort](#community-
-00000bd0: 616e 642d 7375 7070 6f72 7429 0a20 2020  and-support).   
-00000be0: 202d 205b 5377 616e 4c61 6220 5245 4144   - [SwanLab READ
-00000bf0: 4d45 2042 6164 6765 5d28 2373 7761 6e6c  ME Badge](#swanl
-00000c00: 6162 2d72 6561 646d 652d 6261 6467 6529  ab-readme-badge)
-00000c10: 0a20 2020 202d 205b 4369 7469 6e67 2053  .    - [Citing S
-00000c20: 7761 6e4c 6162 2069 6e20 7468 6520 5061  wanLab in the Pa
-00000c30: 7065 725d 2823 6369 7469 6e67 2d73 7761  per](#citing-swa
-00000c40: 6e6c 6162 2d69 6e2d 7468 652d 7061 7065  nlab-in-the-pape
-00000c50: 7229 0a20 2020 202d 205b 436f 6e74 7269  r).    - [Contri
-00000c60: 6275 7465 2074 6f20 5377 616e 4c61 625d  bute to SwanLab]
-00000c70: 2823 636f 6e74 7269 6275 7465 2d74 6f2d  (#contribute-to-
-00000c80: 7377 616e 6c61 6229 0a20 2020 202d 205b  swanlab).    - [
-00000c90: 446f 776e 6c6f 6164 2049 636f 6e5d 2823  Download Icon](#
-00000ca0: 646f 776e 6c6f 6164 2d69 636f 6e29 0a2d  download-icon).-
-00000cb0: 205b f09f 9383 204c 6963 656e 7365 5d28   [.... License](
-00000cc0: 232d 6c69 6365 6e73 6529 0a0a 3c62 722f  #-license)..<br/
-00000cd0: 3e0a 0a3c 2f64 6574 6169 6c73 3e0a 0a23  >..</details>..#
-00000ce0: 2320 f09f 918b f09f 8fbb 2049 6e74 726f  # ........ Intro
-00000cf0: 6475 6374 696f 6e0a 0a53 7761 6e4c 6162  duction..SwanLab
-00000d00: 2069 7320 616e 206f 7065 6e2d 736f 7572   is an open-sour
-00000d10: 6365 2c20 6c69 6768 7477 6569 6768 7420  ce, lightweight 
-00000d20: 4149 2065 7870 6572 696d 656e 7420 7472  AI experiment tr
-00000d30: 6163 6b69 6e67 2074 6f6f 6c20 7468 6174  acking tool that
-00000d40: 2070 726f 7669 6465 7320 6120 706c 6174   provides a plat
-00000d50: 666f 726d 2066 6f72 2074 7261 636b 696e  form for trackin
-00000d60: 672c 2063 6f6d 7061 7269 6e67 2c20 616e  g, comparing, an
-00000d70: 640a 636f 6c6c 6162 6f72 6174 696e 6720  d.collaborating 
-00000d80: 6f6e 2065 7870 6572 696d 656e 7473 2c20  on experiments, 
-00000d90: 6169 6d69 6e67 2074 6f20 6163 6365 6c65  aiming to accele
-00000da0: 7261 7465 2074 6865 2072 6573 6561 7263  rate the researc
-00000db0: 6820 616e 6420 6465 7665 6c6f 706d 656e  h and developmen
-00000dc0: 7420 6566 6669 6369 656e 6379 206f 6620  t efficiency of 
-00000dd0: 4149 2074 6561 6d73 2062 7920 3130 3020  AI teams by 100 
-00000de0: 7469 6d65 732e 0a0a 5377 616e 4c61 62e6  times...SwanLab.
-00000df0: 98af e4b8 80e4 b8aa e5bc 80e6 ba90 e380  ................
-00000e00: 81e8 bdbb e987 8fe7 baa7 e79a 8441 49e5  .............AI.
-00000e10: ae9e e9aa 8ce8 b79f e8b8 aae5 b7a5 e585  ................
-00000e20: b7ef bc8c e68f 90e4 be9b e4ba 86e4 b880  ................
-00000e30: e4b8 aae8 b79f e8b8 aae3 8081 e6af 94e8  ................
-00000e40: be83 e380 81e5 928c e58d 8fe4 bd9c e5ae  ................
-00000e50: 9ee9 aa8c e79a 84e5 b9b3 e58f b0ef bc8c  ................
-00000e60: e697 a8e5 9ca8 e58a a0e9 809f 4149 e7a0  ............AI..
-00000e70: 94e5 8f91 e59b a2e9 989f 3130 30e5 808d  ..........100...
-00000e80: e79a 84e7 a094 e58f 91e6 9588 e78e 87e3  ................
-00000e90: 8082 0a0a 4974 206f 6666 6572 7320 6120  ....It offers a 
-00000ea0: 7573 6572 2d66 7269 656e 646c 7920 4150  user-friendly AP
-00000eb0: 4920 616e 6420 6120 6465 6365 6e74 2069  I and a decent i
-00000ec0: 6e74 6572 6661 6365 2c20 636f 6d62 696e  nterface, combin
-00000ed0: 696e 6720 6665 6174 7572 6573 2073 7563  ing features suc
-00000ee0: 6820 6173 2074 7261 636b 696e 6720 6879  h as tracking hy
-00000ef0: 7065 7270 6172 616d 6574 6572 2c20 7265  perparameter, re
-00000f00: 636f 7264 696e 670a 6d65 7472 6963 2c20  cording.metric, 
-00000f10: 6f6e 6c69 6e65 2063 6f6c 6c61 626f 7261  online collabora
-00000f20: 7469 6f6e 2c20 7368 6172 696e 6720 6578  tion, sharing ex
-00000f30: 7065 7269 6d65 6e74 206c 696e 6b2c 2072  periment link, r
-00000f40: 6561 6c2d 7469 6d65 206d 6573 7361 6765  eal-time message
-00000f50: 206e 6f74 6966 6963 6174 696f 6e73 2c20   notifications, 
-00000f60: 616c 6c6f 7769 6e67 2079 6f75 2074 6f20  allowing you to 
-00000f70: 7175 6963 6b6c 7920 7472 6163 6b20 4d4c  quickly track ML
-00000f80: 0a65 7870 6572 696d 656e 7473 2c20 7669  .experiments, vi
-00000f90: 7375 616c 697a 6520 7072 6f63 6573 7365  sualize processe
-00000fa0: 732c 2061 6e64 2073 6861 7265 2077 6974  s, and share wit
-00000fb0: 6820 7065 6572 732e 0a0a 4279 2075 7369  h peers...By usi
-00000fc0: 6e67 2c20 7265 7365 6172 6368 6572 7320  ng, researchers 
-00000fd0: 6361 6e20 6163 6375 6d75 6c61 7465 2074  can accumulate t
-00000fe0: 6865 6972 2074 7261 696e 696e 6720 6578  heir training ex
-00000ff0: 7065 7269 656e 6365 7320 616e 6420 7365  periences and se
-00001000: 616d 6c65 7373 6c79 2063 6f6d 6d75 6e69  amlessly communi
-00001010: 6361 7465 2061 6e64 2063 6f6c 6c61 626f  cate and collabo
-00001020: 7261 7465 2077 6974 6820 7065 6572 732e  rate with peers.
-00001030: 0a4d 6163 6869 6e65 206c 6561 726e 696e  .Machine learnin
-00001040: 6720 656e 6769 6e65 6572 7320 6361 6e20  g engineers can 
-00001050: 6465 7665 6c6f 7020 6d6f 6465 6c73 2066  develop models f
-00001060: 6f72 2070 726f 6475 6374 696f 6e20 6d6f  or production mo
-00001070: 7265 2065 6666 6963 6965 6e74 6c79 2e0a  re efficiently..
-00001080: 0a21 5b5d 2872 6561 646d 655f 6669 6c65  .![](readme_file
-00001090: 732f 696e 7472 6f64 7563 7469 6f6e 2e70  s/introduction.p
-000010a0: 6e67 290a 0a48 6572 6520 6973 2074 6865  ng)..Here is the
-000010b0: 2045 6e67 6c69 7368 2076 6572 7369 6f6e   English version
-000010c0: 206f 6620 7468 6520 636f 7265 2066 6561   of the core fea
-000010d0: 7475 7265 206c 6973 7420 666f 7220 616e  ture list for an
-000010e0: 2041 4920 706c 6174 666f 726d 3a0a 0a2a   AI platform:..*
-000010f0: 2a31 2e20 f09f 938a 2045 7870 6572 696d  *1. .... Experim
-00001100: 656e 7461 6c20 4d65 7472 6963 7320 616e  ental Metrics an
-00001110: 6420 5472 6163 6b69 6e67 2048 7970 6572  d Tracking Hyper
-00001120: 7061 7261 6d65 7465 722a 2a3a 2045 6d62  parameter**: Emb
-00001130: 6564 2079 6f75 7220 6d61 6368 696e 6520  ed your machine 
-00001140: 6c65 6172 6e69 6e67 2070 6970 656c 696e  learning pipelin
-00001150: 6520 7769 7468 206d 696e 696d 616c 6973  e with minimalis
-00001160: 7469 6320 636f 6465 0a61 6e64 2074 7261  tic code.and tra
-00001170: 636b 206b 6579 2074 7261 696e 696e 6720  ck key training 
-00001180: 6d65 7472 6963 732e 0a0a 2d20 466c 6578  metrics...- Flex
-00001190: 6962 6c65 2072 6563 6f72 6469 6e67 206f  ible recording o
-000011a0: 6620 6879 7065 7270 6172 616d 6574 6572  f hyperparameter
-000011b0: 7320 616e 6420 6578 7065 7269 6d65 6e74  s and experiment
-000011c0: 2063 6f6e 6669 6775 7261 7469 6f6e 732e   configurations.
-000011d0: 0a2d 202a 2a53 7570 706f 7274 6564 206d  .- **Supported m
-000011e0: 6574 6164 6174 6120 7479 7065 732a 2a3a  etadata types**:
-000011f0: 2073 6361 6c61 7220 6d65 7472 6963 732c   scalar metrics,
-00001200: 2069 6d61 6765 732c 2061 7564 696f 2c20   images, audio, 
-00001210: 7465 7874 2c20 6574 632e 0a2d 202a 2a53  text, etc..- **S
-00001220: 7570 706f 7274 6564 2063 6861 7274 2074  upported chart t
-00001230: 7970 6573 2a2a 3a20 6c69 6e65 2067 7261  ypes**: line gra
-00001240: 7068 732c 206d 6564 6961 2063 6861 7274  phs, media chart
-00001250: 7320 2869 6d61 6765 732c 2061 7564 696f  s (images, audio
-00001260: 2c20 7465 7874 292c 2065 7463 2e0a 2d20  , text), etc..- 
-00001270: 2a2a 4175 746f 6d61 7469 6320 6c6f 6767  **Automatic logg
-00001280: 696e 672a 2a3a 2063 6f6e 736f 6c65 206c  ing**: console l
-00001290: 6f67 6769 6e67 2c20 4750 5520 6861 7264  ogging, GPU hard
-000012a0: 7761 7265 2c20 4769 7420 696e 666f 726d  ware, Git inform
-000012b0: 6174 696f 6e2c 2050 7974 686f 6e20 696e  ation, Python in
-000012c0: 7465 7270 7265 7465 722c 206c 6973 7420  terpreter, list 
-000012d0: 6f66 2050 7974 686f 6e20 6c69 6272 6172  of Python librar
-000012e0: 6965 732c 0a20 2063 6f64 6520 6469 7265  ies,.  code dire
-000012f0: 6374 6f72 792e 0a0a 2a2a 322e 20e2 9aa1  ctory...**2. ...
-00001300: efb8 8f20 436f 6d70 7265 6865 6e73 6976  ... Comprehensiv
-00001310: 6520 4672 616d 6577 6f72 6b20 496e 7465  e Framework Inte
-00001320: 6772 6174 696f 6e2a 2a3a 2050 7954 6f72  gration**: PyTor
-00001330: 6368 e380 8154 656e 736f 7266 6c6f 77e3  ch...Tensorflow.
-00001340: 8081 5079 546f 7263 6820 4c69 6768 746e  ..PyTorch Lightn
-00001350: 696e 67e3 8081 f09f a497 4875 6767 696e  ing.......Huggin
-00001360: 6746 6163 65e3 8081 5472 616e 7366 6f72  gFace...Transfor
-00001370: 6d65 7273 e380 814d 4d45 6e67 696e 65e3  mers...MMEngine.
-00001380: 8081 556c 7472 616c 7974 6963 73e3 8081  ..Ultralytics...
-00001390: 6661 7374 6169 e380 8154 656e 736f 7262  fastai...Tensorb
-000013a0: 6f61 7264 e380 814f 7065 6e41 49e3 8081  oard...OpenAI...
-000013b0: 5a68 6970 7541 49e3 8081 4879 6472 61e3  ZhipuAI...Hydra.
-000013c0: 8081 2e2e 2e0a 0a2a 2a33 2e20 f09f 93a6  .......**3. ....
-000013d0: 204f 7267 616e 697a 696e 6720 4578 7065   Organizing Expe
-000013e0: 7269 6d65 6e74 732a 2a3a 2043 656e 7472  riments**: Centr
-000013f0: 616c 697a 6564 2064 6173 6862 6f61 7264  alized dashboard
-00001400: 2066 6f72 2065 6666 6963 6965 6e74 6c79   for efficiently
-00001410: 206d 616e 6167 696e 6720 6d75 6c74 6970   managing multip
-00001420: 6c65 2070 726f 6a65 6374 7320 616e 6420  le projects and 
-00001430: 6578 7065 7269 6d65 6e74 732c 0a70 726f  experiments,.pro
-00001440: 7669 6469 6e67 2061 6e20 6f76 6572 7669  viding an overvi
-00001450: 6577 206f 6620 7472 6169 6e69 6e67 2061  ew of training a
-00001460: 7420 6120 676c 616e 6365 2e0a 0a2a 2a34  t a glance...**4
-00001470: 2e20 f09f 869a 2043 6f6d 7061 7269 6e67  . .... Comparing
-00001480: 2052 6573 756c 7473 2a2a 3a20 5573 6520   Results**: Use 
-00001490: 6f6e 6c69 6e65 2074 6162 6c65 7320 616e  online tables an
-000014a0: 6420 7061 6972 6564 2063 6861 7274 7320  d paired charts 
-000014b0: 746f 2063 6f6d 7061 7265 2074 6865 2068  to compare the h
-000014c0: 7970 6572 7061 7261 6d65 7465 7273 2061  yperparameters a
-000014d0: 6e64 206f 7574 636f 6d65 7320 6f66 2064  nd outcomes of d
-000014e0: 6966 6665 7265 6e74 0a65 7870 6572 696d  ifferent.experim
-000014f0: 656e 7473 2c20 6465 7665 6c6f 7069 6e67  ents, developing
-00001500: 2069 7465 7261 7469 7665 2069 6e73 7069   iterative inspi
-00001510: 7261 7469 6f6e 2e0a 0a2a 2a35 2e20 f09f  ration...**5. ..
-00001520: 91a5 204f 6e6c 696e 6520 436f 6c6c 6162  .. Online Collab
-00001530: 6f72 6174 696f 6e2a 2a3a 2043 6f6c 6c61  oration**: Colla
-00001540: 626f 7261 7465 2077 6974 6820 796f 7572  borate with your
-00001550: 2074 6561 6d20 6f6e 2074 7261 696e 696e   team on trainin
-00001560: 6720 7072 6f6a 6563 7473 2c20 7375 7070  g projects, supp
-00001570: 6f72 7469 6e67 2072 6561 6c2d 7469 6d65  orting real-time
-00001580: 2073 796e 6368 726f 6e69 7a61 7469 6f6e   synchronization
-00001590: 206f 660a 6578 7065 7269 6d65 6e74 7320   of.experiments 
-000015a0: 756e 6465 7220 7468 6520 7361 6d65 2070  under the same p
-000015b0: 726f 6a65 6374 2c20 616c 6c6f 7769 6e67  roject, allowing
-000015c0: 2079 6f75 2074 6f20 7379 6e63 6872 6f6e   you to synchron
-000015d0: 697a 6520 7472 6169 6e69 6e67 2072 6563  ize training rec
-000015e0: 6f72 6473 206f 6620 7468 6520 7465 616d  ords of the team
-000015f0: 206f 6e6c 696e 6520 616e 6420 7368 6172   online and shar
-00001600: 6520 696e 7369 6768 7473 0a61 6e64 2073  e insights.and s
-00001610: 7567 6765 7374 696f 6e73 2062 6173 6564  uggestions based
-00001620: 206f 6e20 7265 7375 6c74 732e 0a0a 2a2a   on results...**
-00001630: 362e 20e2 9c89 efb8 8f20 5368 6172 696e  6. ...... Sharin
-00001640: 6720 5265 7375 6c74 732a 2a3a 2043 6f70  g Results**: Cop
-00001650: 7920 616e 6420 7365 6e64 2070 6572 7369  y and send persi
-00001660: 7374 656e 7420 5552 4c73 2074 6f20 7368  stent URLs to sh
-00001670: 6172 6520 6561 6368 2065 7870 6572 696d  are each experim
-00001680: 656e 742c 2065 6666 6963 6965 6e74 6c79  ent, efficiently
-00001690: 2073 656e 6420 7468 656d 2074 6f20 636f   send them to co
-000016a0: 6c6c 6561 6775 6573 2c0a 6f72 2065 6d62  lleagues,.or emb
-000016b0: 6564 2074 6865 6d20 696e 206f 6e6c 696e  ed them in onlin
-000016c0: 6520 6e6f 7465 732e 0a0a 2a2a 372e 20f0  e notes...**7. .
-000016d0: 9f92 bb20 5365 6c66 2d68 6f73 7469 6e67  ... Self-hosting
-000016e0: 2053 7570 706f 7274 2a2a 3a20 5375 7070   Support**: Supp
-000016f0: 6f72 7473 206f 6666 6c69 6e65 206d 6f64  orts offline mod
-00001700: 6520 7769 7468 2061 2073 656c 662d 686f  e with a self-ho
-00001710: 7374 6564 2063 6f6d 6d75 6e69 7479 2076  sted community v
-00001720: 6572 7369 6f6e 2074 6861 7420 616c 736f  ersion that also
-00001730: 2061 6c6c 6f77 7320 666f 7220 6461 7368   allows for dash
-00001740: 626f 6172 640a 7669 6577 696e 6720 616e  board.viewing an
-00001750: 6420 6578 7065 7269 6d65 6e74 206d 616e  d experiment man
-00001760: 6167 656d 656e 742e 0a0a 3e20 5c5b 2149  agement...> \[!I
-00001770: 4d50 4f52 5441 4e54 5d0a 3e0a 3e20 2a2a  MPORTANT].>.> **
-00001780: 5374 6172 2055 732a 2a2c 2059 6f75 2077  Star Us**, You w
-00001790: 696c 6c20 7265 6365 6976 6520 616c 6c20  ill receive all 
-000017a0: 7265 6c65 6173 6520 6e6f 7469 6669 6361  release notifica
-000017b0: 7469 6f6e 7320 6672 6f6d 2047 6974 4875  tions from GitHu
-000017c0: 6220 7769 7468 6f75 7420 616e 7920 6465  b without any de
-000017d0: 6c61 7920 7e20 e2ad 90ef b88f 0a0a 0a0a  lay ~ ..........
-000017e0: 215b 7374 6172 2d75 735d 2872 6561 646d  ![star-us](readm
-000017f0: 655f 6669 6c65 732f 7374 6172 2d75 732e  e_files/star-us.
-00001800: 706e 6729 0a0a 3c62 723e 0a0a 2323 20f0  png)..<br>..## .
-00001810: 9f8f 8120 5175 6963 6b20 5374 6172 740a  ... Quick Start.
-00001820: 0a23 2323 2031 2e49 6e73 7461 6c6c 6174  .### 1.Installat
-00001830: 696f 6e0a 0a60 6060 6261 7368 0a70 6970  ion..```bash.pip
-00001840: 2069 6e73 7461 6c6c 2073 7761 6e6c 6162   install swanlab
-00001850: 0a60 6060 0a0a 2323 2320 322e 4c6f 6720  .```..### 2.Log 
-00001860: 696e 2061 6e64 2067 6574 2074 6865 2041  in and get the A
-00001870: 5049 204b 6579 0a0a 312e 202a 2a46 7265  PI Key..1. **Fre
-00001880: 6520 5b53 6967 6e20 5570 5d28 6874 7470  e [Sign Up](http
-00001890: 733a 2f2f 7377 616e 6c61 622e 636e 292a  s://swanlab.cn)*
-000018a0: 2a0a 0a32 2e20 2a2a 4c6f 6720 696e 2074  *..2. **Log in t
-000018b0: 6f20 796f 7572 2061 6363 6f75 6e74 2a2a  o your account**
-000018c0: 2c20 676f 2074 6f20 5573 6572 2053 6574  , go to User Set
-000018d0: 7469 6e67 7320 3e20 5b41 5049 204b 6579  tings > [API Key
-000018e0: 5d28 6874 7470 733a 2f2f 7377 616e 6c61  ](https://swanla
-000018f0: 622e 636e 2f73 6574 7469 6e67 7329 2061  b.cn/settings) a
-00001900: 6e64 2063 6f70 7920 796f 7572 2041 5049  nd copy your API
-00001910: 204b 6579 2e0a 0a33 2e20 2a2a 4f70 656e   Key...3. **Open
-00001920: 2079 6f75 7220 7465 726d 696e 616c 2061   your terminal a
-00001930: 6e64 2065 6e74 6572 2a2a 3a0a 0a60 6060  nd enter**:..```
-00001940: 6261 7368 0a73 7761 6e6c 6162 206c 6f67  bash.swanlab log
-00001950: 696e 0a60 6060 0a0a 5768 656e 2070 726f  in.```..When pro
-00001960: 6d70 7465 642c 2065 6e74 6572 2079 6f75  mpted, enter you
-00001970: 7220 4150 4920 4b65 7920 616e 6420 7072  r API Key and pr
-00001980: 6573 7320 456e 7465 7220 746f 2063 6f6d  ess Enter to com
-00001990: 706c 6574 6520 7468 6520 6c6f 6769 6e2e  plete the login.
-000019a0: 0a0a 2323 2320 332e 2049 6e74 6567 7261  ..### 3. Integra
-000019b0: 7465 2053 7761 6e4c 6162 2077 6974 6820  te SwanLab with 
-000019c0: 596f 7572 2043 6f64 650a 0a60 6060 7079  Your Code..```py
-000019d0: 7468 6f6e 0a69 6d70 6f72 7420 7377 616e  thon.import swan
-000019e0: 6c61 620a 0a23 2043 7265 6174 6520 6120  lab..# Create a 
-000019f0: 6e65 7720 5377 616e 4c61 6220 6578 7065  new SwanLab expe
-00001a00: 7269 6d65 6e74 0a73 7761 6e6c 6162 2e69  riment.swanlab.i
-00001a10: 6e69 7428 0a20 2020 2070 726f 6a65 6374  nit(.    project
-00001a20: 3d22 6d79 2d66 6972 7374 2d6d 6c22 2c0a  ="my-first-ml",.
-00001a30: 2020 2020 636f 6e66 6967 3d7b 276c 6561      config={'lea
-00001a40: 726e 696e 672d 7261 7465 273a 2030 2e30  rning-rate': 0.0
-00001a50: 3033 7d0a 290a 0a23 204c 6f67 206d 6574  03}.)..# Log met
-00001a60: 7269 6373 0a66 6f72 2069 2069 6e20 7261  rics.for i in ra
-00001a70: 6e67 6528 3130 293a 0a20 2020 2073 7761  nge(10):.    swa
-00001a80: 6e6c 6162 2e6c 6f67 287b 226c 6f73 7322  nlab.log({"loss"
-00001a90: 3a20 697d 290a 6060 600a 0a2a 2a41 6c6c  : i}).```..**All
-00001aa0: 2073 6574 212a 2a20 5669 7369 7420 5b53   set!** Visit [S
-00001ab0: 7761 6e4c 6162 5d28 6874 7470 733a 2f2f  wanLab](https://
-00001ac0: 7377 616e 6c61 622e 636e 2920 746f 2073  swanlab.cn) to s
-00001ad0: 6565 2079 6f75 7220 6669 7273 7420 5377  ee your first Sw
-00001ae0: 616e 4c61 6220 6578 7065 7269 6d65 6e74  anLab experiment
-00001af0: 2e0a 0a21 5b4d 4e49 5354 5d28 7265 6164  ...![MNIST](read
-00001b00: 6d65 5f66 696c 6573 2f72 6561 646d 652d  me_files/readme-
-00001b10: 6d6e 6973 742e 706e 6729 0a0a 3c62 723e  mnist.png)..<br>
-00001b20: 0a0a 2323 20f0 9f93 8320 4d6f 7265 2045  ..## .... More E
-00001b30: 7861 6d70 6c65 730a 0a3c 6465 7461 696c  xamples..<detail
-00001b40: 733e 0a3c 7375 6d6d 6172 793e 4d4e 4953  s>.<summary>MNIS
-00001b50: 543c 2f73 756d 6d61 7279 3e0a 0a60 6060  T</summary>..```
-00001b60: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f73  python.import os
-00001b70: 0a69 6d70 6f72 7420 746f 7263 680a 6672  .import torch.fr
-00001b80: 6f6d 2074 6f72 6368 2069 6d70 6f72 7420  om torch import 
-00001b90: 6e6e 2c20 6f70 7469 6d2c 2075 7469 6c73  nn, optim, utils
-00001ba0: 0a69 6d70 6f72 7420 746f 7263 682e 6e6e  .import torch.nn
-00001bb0: 2e66 756e 6374 696f 6e61 6c20 6173 2046  .functional as F
-00001bc0: 0a66 726f 6d20 746f 7263 6876 6973 696f  .from torchvisio
-00001bd0: 6e2e 6461 7461 7365 7473 2069 6d70 6f72  n.datasets impor
-00001be0: 7420 4d4e 4953 540a 6672 6f6d 2074 6f72  t MNIST.from tor
-00001bf0: 6368 7669 7369 6f6e 2e74 7261 6e73 666f  chvision.transfo
-00001c00: 726d 7320 696d 706f 7274 2054 6f54 656e  rms import ToTen
-00001c10: 736f 720a 696d 706f 7274 2073 7761 6e6c  sor.import swanl
-00001c20: 6162 0a0a 0a23 2043 4e4e e7bd 91e7 bb9c  ab...# CNN......
-00001c30: e69e 84e5 bbba 0a63 6c61 7373 2043 6f6e  .......class Con
-00001c40: 764e 6574 286e 6e2e 4d6f 6475 6c65 293a  vNet(nn.Module):
-00001c50: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00001c60: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00001c70: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00001c80: 5f28 290a 2020 2020 2020 2020 2320 312c  _().        # 1,
-00001c90: 3238 7832 380a 2020 2020 2020 2020 7365  28x28.        se
-00001ca0: 6c66 2e63 6f6e 7631 203d 206e 6e2e 436f  lf.conv1 = nn.Co
-00001cb0: 6e76 3264 2831 2c20 3130 2c20 3529 2020  nv2d(1, 10, 5)  
-00001cc0: 2320 3130 2c20 3234 7832 340a 2020 2020  # 10, 24x24.    
-00001cd0: 2020 2020 7365 6c66 2e63 6f6e 7632 203d      self.conv2 =
-00001ce0: 206e 6e2e 436f 6e76 3264 2831 302c 2032   nn.Conv2d(10, 2
-00001cf0: 302c 2033 2920 2023 2031 3238 2c20 3130  0, 3)  # 128, 10
-00001d00: 7831 300a 2020 2020 2020 2020 7365 6c66  x10.        self
-00001d10: 2e66 6331 203d 206e 6e2e 4c69 6e65 6172  .fc1 = nn.Linear
-00001d20: 2832 3020 2a20 3130 202a 2031 302c 2035  (20 * 10 * 10, 5
-00001d30: 3030 290a 2020 2020 2020 2020 7365 6c66  00).        self
-00001d40: 2e66 6332 203d 206e 6e2e 4c69 6e65 6172  .fc2 = nn.Linear
-00001d50: 2835 3030 2c20 3130 290a 0a20 2020 2064  (500, 10)..    d
-00001d60: 6566 2066 6f72 7761 7264 2873 656c 662c  ef forward(self,
-00001d70: 2078 293a 0a20 2020 2020 2020 2069 6e5f   x):.        in_
-00001d80: 7369 7a65 203d 2078 2e73 697a 6528 3029  size = x.size(0)
-00001d90: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-00001da0: 656c 662e 636f 6e76 3128 7829 2020 2320  elf.conv1(x)  # 
-00001db0: 3234 0a20 2020 2020 2020 206f 7574 203d  24.        out =
-00001dc0: 2046 2e72 656c 7528 6f75 7429 0a20 2020   F.relu(out).   
-00001dd0: 2020 2020 206f 7574 203d 2046 2e6d 6178       out = F.max
-00001de0: 5f70 6f6f 6c32 6428 6f75 742c 2032 2c20  _pool2d(out, 2, 
-00001df0: 3229 2020 2320 3132 0a20 2020 2020 2020  2)  # 12.       
-00001e00: 206f 7574 203d 2073 656c 662e 636f 6e76   out = self.conv
-00001e10: 3228 6f75 7429 2020 2320 3130 0a20 2020  2(out)  # 10.   
-00001e20: 2020 2020 206f 7574 203d 2046 2e72 656c       out = F.rel
-00001e30: 7528 6f75 7429 0a20 2020 2020 2020 206f  u(out).        o
-00001e40: 7574 203d 206f 7574 2e76 6965 7728 696e  ut = out.view(in
-00001e50: 5f73 697a 652c 202d 3129 0a20 2020 2020  _size, -1).     
-00001e60: 2020 206f 7574 203d 2073 656c 662e 6663     out = self.fc
-00001e70: 3128 6f75 7429 0a20 2020 2020 2020 206f  1(out).        o
-00001e80: 7574 203d 2046 2e72 656c 7528 6f75 7429  ut = F.relu(out)
-00001e90: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-00001ea0: 656c 662e 6663 3228 6f75 7429 0a20 2020  elf.fc2(out).   
-00001eb0: 2020 2020 206f 7574 203d 2046 2e6c 6f67       out = F.log
-00001ec0: 5f73 6f66 746d 6178 286f 7574 2c20 6469  _softmax(out, di
-00001ed0: 6d3d 3129 0a20 2020 2020 2020 2072 6574  m=1).        ret
-00001ee0: 7572 6e20 6f75 740a 0a0a 2320 e68d 95e8  urn out...# ....
-00001ef0: 8eb7 e5b9 b6e5 8faf e8a7 86e5 8c96 e589  ................
-00001f00: 8d32 30e5 bca0 e59b bee5 838f 0a64 6566  .20..........def
-00001f10: 206c 6f67 5f69 6d61 6765 7328 6c6f 6164   log_images(load
-00001f20: 6572 2c20 6e75 6d5f 696d 6167 6573 3d31  er, num_images=1
-00001f30: 3629 3a0a 2020 2020 696d 6167 6573 5f6c  6):.    images_l
-00001f40: 6f67 6765 6420 3d20 300a 2020 2020 6c6f  ogged = 0.    lo
-00001f50: 6767 6564 5f69 6d61 6765 7320 3d20 5b5d  gged_images = []
-00001f60: 0a20 2020 2066 6f72 2069 6d61 6765 732c  .    for images,
-00001f70: 206c 6162 656c 7320 696e 206c 6f61 6465   labels in loade
-00001f80: 723a 0a20 2020 2020 2020 2023 2069 6d61  r:.        # ima
-00001f90: 6765 733a 2062 6174 6368 206f 6620 696d  ges: batch of im
-00001fa0: 6167 6573 2c20 6c61 6265 6c73 3a20 6261  ages, labels: ba
-00001fb0: 7463 6820 6f66 206c 6162 656c 730a 2020  tch of labels.  
-00001fc0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00001fd0: 616e 6765 2869 6d61 6765 732e 7368 6170  ange(images.shap
-00001fe0: 655b 305d 293a 0a20 2020 2020 2020 2020  e[0]):.         
-00001ff0: 2020 2069 6620 696d 6167 6573 5f6c 6f67     if images_log
-00002000: 6765 6420 3c20 6e75 6d5f 696d 6167 6573  ged < num_images
-00002010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002020: 2020 2320 e4bd bfe7 94a8 7377 616e 6c61    # ......swanla
-00002030: 622e 496d 6167 65e5 b086 e59b bee5 838f  b.Image.........
-00002040: e8bd ace6 8da2 e4b8 ba77 616e 6462 e58f  .........wandb..
-00002050: afe8 a786 e58c 96e6 a0bc e5bc 8f0a 2020  ..............  
-00002060: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00002070: 6767 6564 5f69 6d61 6765 732e 6170 7065  gged_images.appe
-00002080: 6e64 2873 7761 6e6c 6162 2e49 6d61 6765  nd(swanlab.Image
-00002090: 2869 6d61 6765 735b 695d 2c20 6361 7074  (images[i], capt
-000020a0: 696f 6e3d 6622 4c61 6265 6c3a 207b 6c61  ion=f"Label: {la
-000020b0: 6265 6c73 5b69 5d7d 2229 290a 2020 2020  bels[i]}")).    
-000020c0: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-000020d0: 6573 5f6c 6f67 6765 6420 2b3d 2031 0a20  es_logged += 1. 
-000020e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000020f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002100: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
-00002110: 6620 696d 6167 6573 5f6c 6f67 6765 6420  f images_logged 
-00002120: 3e3d 206e 756d 5f69 6d61 6765 733a 0a20  >= num_images:. 
-00002130: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00002140: 0a20 2020 2073 7761 6e6c 6162 2e6c 6f67  .    swanlab.log
-00002150: 287b 224d 4e49 5354 2d50 7265 7669 6577  ({"MNIST-Preview
-00002160: 223a 206c 6f67 6765 645f 696d 6167 6573  ": logged_images
-00002170: 7d29 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  })...if __name__
-00002180: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
-00002190: 0a20 2020 2023 20e5 889d e5a7 8be5 8c96  .    # .........
-000021a0: 7377 616e 6c61 620a 2020 2020 7275 6e20  swanlab.    run 
-000021b0: 3d20 7377 616e 6c61 622e 696e 6974 280a  = swanlab.init(.
-000021c0: 2020 2020 2020 2020 7072 6f6a 6563 743d          project=
-000021d0: 224d 4e49 5354 2d65 7861 6d70 6c65 222c  "MNIST-example",
-000021e0: 0a20 2020 2020 2020 2065 7870 6572 696d  .        experim
-000021f0: 656e 745f 6e61 6d65 3d22 436f 6e76 4e65  ent_name="ConvNe
-00002200: 7422 2c0a 2020 2020 2020 2020 6465 7363  t",.        desc
-00002210: 7269 7074 696f 6e3d 2254 7261 696e 2043  ription="Train C
-00002220: 6f6e 764e 6574 206f 6e20 4d4e 4953 5420  onvNet on MNIST 
-00002230: 6461 7461 7365 742e 222c 0a20 2020 2020  dataset.",.     
-00002240: 2020 2063 6f6e 6669 673d 7b0a 2020 2020     config={.    
-00002250: 2020 2020 2020 2020 226d 6f64 656c 223a          "model":
-00002260: 2022 434e 4e22 2c0a 2020 2020 2020 2020   "CNN",.        
-00002270: 2020 2020 226f 7074 696d 223a 2022 4164      "optim": "Ad
-00002280: 616d 222c 0a20 2020 2020 2020 2020 2020  am",.           
-00002290: 2022 6c72 223a 2030 2e30 3031 2c0a 2020   "lr": 0.001,.  
-000022a0: 2020 2020 2020 2020 2020 2262 6174 6368            "batch
-000022b0: 5f73 697a 6522 3a20 3531 322c 0a20 2020  _size": 512,.   
-000022c0: 2020 2020 2020 2020 2022 6e75 6d5f 6570           "num_ep
-000022d0: 6f63 6873 223a 2031 302c 0a20 2020 2020  ochs": 10,.     
-000022e0: 2020 2020 2020 2022 7472 6169 6e5f 6461         "train_da
-000022f0: 7461 7365 745f 6e75 6d22 3a20 3535 3030  taset_num": 5500
-00002300: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-00002310: 7661 6c5f 6461 7461 7365 745f 6e75 6d22  val_dataset_num"
-00002320: 3a20 3530 3030 2c0a 2020 2020 2020 2020  : 5000,.        
-00002330: 7d2c 0a20 2020 2029 0a0a 2020 2020 2320  },.    )..    # 
-00002340: e8ae bee7 bdae e8ae ade7 bb83 e69c bae3  ................
-00002350: 8081 e9aa 8ce8 af81 e99b 86e5 928c e6b5  ................
-00002360: 8be8 af95 e99b 860a 2020 2020 6461 7461  ........    data
-00002370: 7365 7420 3d20 4d4e 4953 5428 6f73 2e67  set = MNIST(os.g
-00002380: 6574 6377 6428 292c 2074 7261 696e 3d54  etcwd(), train=T
-00002390: 7275 652c 2064 6f77 6e6c 6f61 643d 5472  rue, download=Tr
-000023a0: 7565 2c20 7472 616e 7366 6f72 6d3d 546f  ue, transform=To
-000023b0: 5465 6e73 6f72 2829 290a 2020 2020 7472  Tensor()).    tr
-000023c0: 6169 6e5f 6461 7461 7365 742c 2076 616c  ain_dataset, val
-000023d0: 5f64 6174 6173 6574 203d 2075 7469 6c73  _dataset = utils
-000023e0: 2e64 6174 612e 7261 6e64 6f6d 5f73 706c  .data.random_spl
-000023f0: 6974 280a 2020 2020 2020 2020 6461 7461  it(.        data
-00002400: 7365 742c 205b 7275 6e2e 636f 6e66 6967  set, [run.config
-00002410: 2e74 7261 696e 5f64 6174 6173 6574 5f6e  .train_dataset_n
-00002420: 756d 2c20 7275 6e2e 636f 6e66 6967 2e76  um, run.config.v
-00002430: 616c 5f64 6174 6173 6574 5f6e 756d 5d0a  al_dataset_num].
-00002440: 2020 2020 290a 0a20 2020 2074 7261 696e      )..    train
-00002450: 5f6c 6f61 6465 7220 3d20 7574 696c 732e  _loader = utils.
-00002460: 6461 7461 2e44 6174 614c 6f61 6465 7228  data.DataLoader(
-00002470: 7472 6169 6e5f 6461 7461 7365 742c 2062  train_dataset, b
-00002480: 6174 6368 5f73 697a 653d 7275 6e2e 636f  atch_size=run.co
-00002490: 6e66 6967 2e62 6174 6368 5f73 697a 652c  nfig.batch_size,
-000024a0: 2073 6875 6666 6c65 3d54 7275 6529 0a20   shuffle=True). 
-000024b0: 2020 2076 616c 5f6c 6f61 6465 7220 3d20     val_loader = 
-000024c0: 7574 696c 732e 6461 7461 2e44 6174 614c  utils.data.DataL
-000024d0: 6f61 6465 7228 7661 6c5f 6461 7461 7365  oader(val_datase
-000024e0: 742c 2062 6174 6368 5f73 697a 653d 312c  t, batch_size=1,
-000024f0: 2073 6875 6666 6c65 3d46 616c 7365 290a   shuffle=False).
-00002500: 0a20 2020 2023 20e5 889d e5a7 8be5 8c96  .    # .........
-00002510: e6a8 a1e5 9e8b e380 81e6 8d9f e5a4 b1e5  ................
-00002520: 87bd e695 b0e5 928c e4bc 98e5 8c96 e599  ................
-00002530: a80a 2020 2020 6d6f 6465 6c20 3d20 436f  ..    model = Co
-00002540: 6e76 4e65 7428 290a 2020 2020 6372 6974  nvNet().    crit
-00002550: 6572 696f 6e20 3d20 6e6e 2e43 726f 7373  erion = nn.Cross
-00002560: 456e 7472 6f70 794c 6f73 7328 290a 2020  EntropyLoss().  
-00002570: 2020 6f70 7469 6d69 7a65 7220 3d20 6f70    optimizer = op
-00002580: 7469 6d2e 4164 616d 286d 6f64 656c 2e70  tim.Adam(model.p
-00002590: 6172 616d 6574 6572 7328 292c 206c 723d  arameters(), lr=
-000025a0: 7275 6e2e 636f 6e66 6967 2e6c 7229 0a0a  run.config.lr)..
-000025b0: 2020 2020 2320 efbc 88e5 8faf e980 89ef      # ..........
-000025c0: bc89 e79c 8be4 b880 e4b8 8be6 95b0 e68d  ................
-000025d0: aee9 9b86 e79a 84e5 898d 3136 e5bc a0e5  ..........16....
-000025e0: 9bbe e583 8f0a 2020 2020 6c6f 675f 696d  ......    log_im
-000025f0: 6167 6573 2874 7261 696e 5f6c 6f61 6465  ages(train_loade
-00002600: 722c 2031 3629 0a0a 2020 2020 2320 e5bc  r, 16)..    # ..
-00002610: 80e5 a78b e8ae ade7 bb83 0a20 2020 2066  ...........    f
-00002620: 6f72 2065 706f 6368 2069 6e20 7261 6e67  or epoch in rang
-00002630: 6528 312c 2072 756e 2e63 6f6e 6669 672e  e(1, run.config.
-00002640: 6e75 6d5f 6570 6f63 6873 293a 0a20 2020  num_epochs):.   
-00002650: 2020 2020 2073 7761 6e6c 6162 2e6c 6f67       swanlab.log
-00002660: 287b 2274 7261 696e 2f65 706f 6368 223a  ({"train/epoch":
-00002670: 2065 706f 6368 7d29 0a20 2020 2020 2020   epoch}).       
-00002680: 2023 20e8 aead e7bb 83e5 beaa e78e af0a   # .............
-00002690: 2020 2020 2020 2020 666f 7220 6974 6572          for iter
-000026a0: 2c20 6261 7463 6820 696e 2065 6e75 6d65  , batch in enume
-000026b0: 7261 7465 2874 7261 696e 5f6c 6f61 6465  rate(train_loade
-000026c0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-000026d0: 782c 2079 203d 2062 6174 6368 0a20 2020  x, y = batch.   
-000026e0: 2020 2020 2020 2020 206f 7074 696d 697a           optimiz
-000026f0: 6572 2e7a 6572 6f5f 6772 6164 2829 0a20  er.zero_grad(). 
-00002700: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00002710: 7420 3d20 6d6f 6465 6c28 7829 0a20 2020  t = model(x).   
-00002720: 2020 2020 2020 2020 206c 6f73 7320 3d20           loss = 
-00002730: 6372 6974 6572 696f 6e28 6f75 7470 7574  criterion(output
-00002740: 2c20 7929 0a20 2020 2020 2020 2020 2020  , y).           
-00002750: 206c 6f73 732e 6261 636b 7761 7264 2829   loss.backward()
-00002760: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-00002770: 696d 697a 6572 2e73 7465 7028 290a 0a20  imizer.step().. 
-00002780: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00002790: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000027a0: 2020 6622 4570 6f63 6820 5b7b 6570 6f63    f"Epoch [{epoc
-000027b0: 687d 2f7b 7275 6e2e 636f 6e66 6967 2e6e  h}/{run.config.n
-000027c0: 756d 5f65 706f 6368 737d 5d2c 2049 7465  um_epochs}], Ite
-000027d0: 7261 7469 6f6e 205b 7b69 7465 7220 2b20  ration [{iter + 
-000027e0: 317d 2f7b 6c65 6e28 7472 6169 6e5f 6c6f  1}/{len(train_lo
-000027f0: 6164 6572 297d 5d2c 204c 6f73 733a 207b  ader)}], Loss: {
-00002800: 6c6f 7373 2e69 7465 6d28 297d 220a 2020  loss.item()}".  
-00002810: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00002820: 2020 2020 2020 2020 2069 6620 6974 6572           if iter
-00002830: 2025 2032 3020 3d3d 2030 3a0a 2020 2020   % 20 == 0:.    
-00002840: 2020 2020 2020 2020 2020 2020 7377 616e              swan
-00002850: 6c61 622e 6c6f 6728 7b22 7472 6169 6e2f  lab.log({"train/
-00002860: 6c6f 7373 223a 206c 6f73 732e 6974 656d  loss": loss.item
-00002870: 2829 7d2c 2073 7465 703d 2865 706f 6368  ()}, step=(epoch
-00002880: 202d 2031 2920 2a20 6c65 6e28 7472 6169   - 1) * len(trai
-00002890: 6e5f 6c6f 6164 6572 2920 2b20 6974 6572  n_loader) + iter
-000028a0: 290a 0a20 2020 2020 2020 2023 20e6 af8f  )..        # ...
-000028b0: 34e4 b8aa 6570 6f63 68e9 aa8c e8af 81e4  4...epoch.......
-000028c0: b880 e6ac a10a 2020 2020 2020 2020 6966  ......        if
-000028d0: 2065 706f 6368 2025 2032 203d 3d20 303a   epoch % 2 == 0:
-000028e0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-000028f0: 656c 2e65 7661 6c28 290a 2020 2020 2020  el.eval().      
-00002900: 2020 2020 2020 636f 7272 6563 7420 3d20        correct = 
-00002910: 300a 2020 2020 2020 2020 2020 2020 746f  0.            to
-00002920: 7461 6c20 3d20 300a 2020 2020 2020 2020  tal = 0.        
-00002930: 2020 2020 7769 7468 2074 6f72 6368 2e6e      with torch.n
-00002940: 6f5f 6772 6164 2829 3a0a 2020 2020 2020  o_grad():.      
-00002950: 2020 2020 2020 2020 2020 666f 7220 6261            for ba
-00002960: 7463 6820 696e 2076 616c 5f6c 6f61 6465  tch in val_loade
-00002970: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00002980: 2020 2020 2020 2078 2c20 7920 3d20 6261         x, y = ba
-00002990: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
-000029a0: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
-000029b0: 206d 6f64 656c 2878 290a 2020 2020 2020   model(x).      
-000029c0: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
-000029d0: 2070 7265 6469 6374 6564 203d 2074 6f72   predicted = tor
-000029e0: 6368 2e6d 6178 286f 7574 7075 742c 2031  ch.max(output, 1
-000029f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002a00: 2020 2020 2020 746f 7461 6c20 2b3d 2079        total += y
-00002a10: 2e73 697a 6528 3029 0a20 2020 2020 2020  .size(0).       
-00002a20: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
-00002a30: 7265 6374 202b 3d20 2870 7265 6469 6374  rect += (predict
-00002a40: 6564 203d 3d20 7929 2e73 756d 2829 2e69  ed == y).sum().i
-00002a50: 7465 6d28 290a 0a20 2020 2020 2020 2020  tem()..         
-00002a60: 2020 2061 6363 7572 6163 7920 3d20 636f     accuracy = co
-00002a70: 7272 6563 7420 2f20 746f 7461 6c0a 2020  rrect / total.  
-00002a80: 2020 2020 2020 2020 2020 7377 616e 6c61            swanla
-00002a90: 622e 6c6f 6728 7b22 7661 6c2f 6163 6375  b.log({"val/accu
-00002aa0: 7261 6379 223a 2061 6363 7572 6163 797d  racy": accuracy}
-00002ab0: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
-00002ac0: 3e0a 0a3c 6465 7461 696c 733e 0a3c 7375  >..<details>.<su
-00002ad0: 6d6d 6172 793e 4661 7368 696f 6e4d 4e53  mmary>FashionMNS
-00002ae0: 4954 3c2f 7375 6d6d 6172 793e 0a0a 6060  IT</summary>..``
-00002af0: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
-00002b00: 730a 696d 706f 7274 2074 6f72 6368 0a66  s.import torch.f
-00002b10: 726f 6d20 746f 7263 6820 696d 706f 7274  rom torch import
-00002b20: 206e 6e2c 206f 7074 696d 2c20 7574 696c   nn, optim, util
-00002b30: 730a 696d 706f 7274 2074 6f72 6368 2e6e  s.import torch.n
-00002b40: 6e2e 6675 6e63 7469 6f6e 616c 2061 7320  n.functional as 
-00002b50: 460a 6672 6f6d 2074 6f72 6368 7669 7369  F.from torchvisi
-00002b60: 6f6e 2e64 6174 6173 6574 7320 696d 706f  on.datasets impo
-00002b70: 7274 2046 6173 6869 6f6e 4d4e 4953 540a  rt FashionMNIST.
-00002b80: 6672 6f6d 2074 6f72 6368 7669 7369 6f6e  from torchvision
-00002b90: 2e74 7261 6e73 666f 726d 7320 696d 706f  .transforms impo
-00002ba0: 7274 2054 6f54 656e 736f 720a 696d 706f  rt ToTensor.impo
-00002bb0: 7274 2073 7761 6e6c 6162 0a0a 0a23 2052  rt swanlab...# R
-00002bc0: 6573 4e65 74e7 bd91 e7bb 9ce6 9e84 e5bb  esNet...........
-00002bd0: ba0a 636c 6173 7320 4261 7369 6362 6c6f  ..class Basicblo
-00002be0: 636b 286e 6e2e 4d6f 6475 6c65 293a 0a20  ck(nn.Module):. 
-00002bf0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00002c00: 7365 6c66 2c20 696e 5f70 6c61 6e65 732c  self, in_planes,
-00002c10: 2070 6c61 6e65 732c 2073 7472 6964 653d   planes, stride=
-00002c20: 3129 3a0a 2020 2020 2020 2020 7375 7065  1):.        supe
-00002c30: 7228 4261 7369 6362 6c6f 636b 2c20 7365  r(Basicblock, se
-00002c40: 6c66 292e 5f5f 696e 6974 5f5f 2829 0a20  lf).__init__(). 
-00002c50: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-00002c60: 3120 3d20 6e6e 2e53 6571 7565 6e74 6961  1 = nn.Sequentia
-00002c70: 6c28 0a20 2020 2020 2020 2020 2020 206e  l(.            n
-00002c80: 6e2e 436f 6e76 3264 2869 6e5f 6368 616e  n.Conv2d(in_chan
-00002c90: 6e65 6c73 3d69 6e5f 706c 616e 6573 2c20  nels=in_planes, 
-00002ca0: 6f75 745f 6368 616e 6e65 6c73 3d70 6c61  out_channels=pla
-00002cb0: 6e65 732c 206b 6572 6e65 6c5f 7369 7a65  nes, kernel_size
-00002cc0: 3d33 2c20 7374 7269 6465 3d73 7472 6964  =3, stride=strid
-00002cd0: 652c 2070 6164 6469 6e67 3d31 2c20 6269  e, padding=1, bi
-00002ce0: 6173 3d46 616c 7365 292c 0a20 2020 2020  as=False),.     
-00002cf0: 2020 2020 2020 206e 6e2e 4261 7463 684e         nn.BatchN
-00002d00: 6f72 6d32 6428 706c 616e 6573 292c 0a20  orm2d(planes),. 
-00002d10: 2020 2020 2020 2020 2020 206e 6e2e 5265             nn.Re
-00002d20: 4c55 2829 0a20 2020 2020 2020 2029 0a20  LU().        ). 
-00002d30: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-00002d40: 3220 3d20 6e6e 2e53 6571 7565 6e74 6961  2 = nn.Sequentia
-00002d50: 6c28 0a20 2020 2020 2020 2020 2020 206e  l(.            n
-00002d60: 6e2e 436f 6e76 3264 2869 6e5f 6368 616e  n.Conv2d(in_chan
-00002d70: 6e65 6c73 3d70 6c61 6e65 732c 206f 7574  nels=planes, out
-00002d80: 5f63 6861 6e6e 656c 733d 706c 616e 6573  _channels=planes
-00002d90: 2c20 6b65 726e 656c 5f73 697a 653d 332c  , kernel_size=3,
-00002da0: 2073 7472 6964 653d 312c 2070 6164 6469   stride=1, paddi
-00002db0: 6e67 3d31 2c20 6269 6173 3d46 616c 7365  ng=1, bias=False
-00002dc0: 292c 0a20 2020 2020 2020 2020 2020 206e  ),.            n
-00002dd0: 6e2e 4261 7463 684e 6f72 6d32 6428 706c  n.BatchNorm2d(pl
-00002de0: 616e 6573 292c 0a20 2020 2020 2020 2029  anes),.        )
-00002df0: 0a0a 2020 2020 2020 2020 6966 2073 7472  ..        if str
-00002e00: 6964 6520 213d 2031 206f 7220 696e 5f70  ide != 1 or in_p
-00002e10: 6c61 6e65 7320 213d 2070 6c61 6e65 733a  lanes != planes:
-00002e20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002e30: 662e 7368 6f72 7463 7574 203d 206e 6e2e  f.shortcut = nn.
-00002e40: 5365 7175 656e 7469 616c 280a 2020 2020  Sequential(.    
-00002e50: 2020 2020 2020 2020 2020 2020 6e6e 2e43              nn.C
-00002e60: 6f6e 7632 6428 696e 5f63 6861 6e6e 656c  onv2d(in_channel
-00002e70: 733d 696e 5f70 6c61 6e65 732c 206f 7574  s=in_planes, out
-00002e80: 5f63 6861 6e6e 656c 733d 706c 616e 6573  _channels=planes
-00002e90: 2c20 6b65 726e 656c 5f73 697a 653d 332c  , kernel_size=3,
-00002ea0: 2073 7472 6964 653d 7374 7269 6465 2c20   stride=stride, 
-00002eb0: 7061 6464 696e 673d 3129 2c0a 2020 2020  padding=1),.    
-00002ec0: 2020 2020 2020 2020 2020 2020 6e6e 2e42              nn.B
-00002ed0: 6174 6368 4e6f 726d 3264 2870 6c61 6e65  atchNorm2d(plane
-00002ee0: 7329 0a20 2020 2020 2020 2020 2020 2029  s).            )
-00002ef0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00002f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002f10: 7368 6f72 7463 7574 203d 206e 6e2e 5365  shortcut = nn.Se
-00002f20: 7175 656e 7469 616c 2829 0a0a 2020 2020  quential()..    
-00002f30: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
-00002f40: 2c20 7829 3a0a 2020 2020 2020 2020 6f75  , x):.        ou
-00002f50: 7420 3d20 7365 6c66 2e63 6f6e 7631 2878  t = self.conv1(x
-00002f60: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
-00002f70: 7365 6c66 2e63 6f6e 7632 286f 7574 290a  self.conv2(out).
-00002f80: 2020 2020 2020 2020 6f75 7420 2b3d 2073          out += s
-00002f90: 656c 662e 7368 6f72 7463 7574 2878 290a  elf.shortcut(x).
-00002fa0: 2020 2020 2020 2020 6f75 7420 3d20 462e          out = F.
-00002fb0: 7265 6c75 286f 7574 290a 2020 2020 2020  relu(out).      
-00002fc0: 2020 7265 7475 726e 206f 7574 0a0a 0a63    return out...c
-00002fd0: 6c61 7373 2052 6573 4e65 7428 6e6e 2e4d  lass ResNet(nn.M
-00002fe0: 6f64 756c 6529 3a0a 2020 2020 6465 6620  odule):.    def 
-00002ff0: 5f5f 696e 6974 5f5f 2873 656c 662c 2062  __init__(self, b
-00003000: 6c6f 636b 2c20 6e75 6d5f 626c 6f63 6b2c  lock, num_block,
-00003010: 206e 756d 5f63 6c61 7373 6573 293a 0a20   num_classes):. 
-00003020: 2020 2020 2020 2073 7570 6572 2852 6573         super(Res
-00003030: 4e65 742c 2073 656c 6629 2e5f 5f69 6e69  Net, self).__ini
-00003040: 745f 5f28 290a 2020 2020 2020 2020 7365  t__().        se
-00003050: 6c66 2e69 6e5f 706c 616e 6573 203d 2031  lf.in_planes = 1
-00003060: 360a 2020 2020 2020 2020 7365 6c66 2e63  6.        self.c
-00003070: 6f6e 7631 203d 206e 6e2e 5365 7175 656e  onv1 = nn.Sequen
-00003080: 7469 616c 280a 2020 2020 2020 2020 2020  tial(.          
-00003090: 2020 6e6e 2e43 6f6e 7632 6428 696e 5f63    nn.Conv2d(in_c
-000030a0: 6861 6e6e 656c 733d 312c 206f 7574 5f63  hannels=1, out_c
-000030b0: 6861 6e6e 656c 733d 3136 2c20 6b65 726e  hannels=16, kern
-000030c0: 656c 5f73 697a 653d 332c 2073 7472 6964  el_size=3, strid
-000030d0: 653d 312c 2070 6164 6469 6e67 3d31 292c  e=1, padding=1),
-000030e0: 0a20 2020 2020 2020 2020 2020 206e 6e2e  .            nn.
-000030f0: 4261 7463 684e 6f72 6d32 6428 3136 292c  BatchNorm2d(16),
-00003100: 0a20 2020 2020 2020 2020 2020 206e 6e2e  .            nn.
-00003110: 5265 4c55 2829 0a20 2020 2020 2020 2029  ReLU().        )
-00003120: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
-00003130: 7870 6f6f 6c20 3d20 6e6e 2e4d 6178 506f  xpool = nn.MaxPo
-00003140: 6f6c 3264 286b 6572 6e65 6c5f 7369 7a65  ol2d(kernel_size
-00003150: 3d33 2c20 7374 7269 6465 3d31 2c20 7061  =3, stride=1, pa
-00003160: 6464 696e 673d 3129 0a0a 2020 2020 2020  dding=1)..      
-00003170: 2020 7365 6c66 2e62 6c6f 636b 3120 3d20    self.block1 = 
-00003180: 7365 6c66 2e5f 6d61 6b65 5f6c 6179 6572  self._make_layer
-00003190: 2862 6c6f 636b 2c20 3136 2c20 6e75 6d5f  (block, 16, num_
-000031a0: 626c 6f63 6b5b 305d 2c20 7374 7269 6465  block[0], stride
-000031b0: 3d31 290a 2020 2020 2020 2020 7365 6c66  =1).        self
-000031c0: 2e62 6c6f 636b 3220 3d20 7365 6c66 2e5f  .block2 = self._
-000031d0: 6d61 6b65 5f6c 6179 6572 2862 6c6f 636b  make_layer(block
-000031e0: 2c20 3332 2c20 6e75 6d5f 626c 6f63 6b5b  , 32, num_block[
-000031f0: 315d 2c20 7374 7269 6465 3d32 290a 2020  1], stride=2).  
-00003200: 2020 2020 2020 7365 6c66 2e62 6c6f 636b        self.block
-00003210: 3320 3d20 7365 6c66 2e5f 6d61 6b65 5f6c  3 = self._make_l
-00003220: 6179 6572 2862 6c6f 636b 2c20 3634 2c20  ayer(block, 64, 
-00003230: 6e75 6d5f 626c 6f63 6b5b 325d 2c20 7374  num_block[2], st
-00003240: 7269 6465 3d32 290a 2020 2020 2020 2020  ride=2).        
-00003250: 2320 7365 6c66 2e62 6c6f 636b 3420 3d20  # self.block4 = 
-00003260: 7365 6c66 2e5f 6d61 6b65 5f6c 6179 6572  self._make_layer
-00003270: 2862 6c6f 636b 2c20 3531 322c 206e 756d  (block, 512, num
-00003280: 5f62 6c6f 636b 5b33 5d2c 2073 7472 6964  _block[3], strid
-00003290: 653d 3229 0a0a 2020 2020 2020 2020 7365  e=2)..        se
-000032a0: 6c66 2e6f 7574 6c61 7965 7220 3d20 6e6e  lf.outlayer = nn
-000032b0: 2e4c 696e 6561 7228 3634 2c20 6e75 6d5f  .Linear(64, num_
-000032c0: 636c 6173 7365 7329 0a0a 2020 2020 6465  classes)..    de
-000032d0: 6620 5f6d 616b 655f 6c61 7965 7228 7365  f _make_layer(se
-000032e0: 6c66 2c20 626c 6f63 6b2c 2070 6c61 6e65  lf, block, plane
-000032f0: 732c 206e 756d 5f62 6c6f 636b 2c20 7374  s, num_block, st
-00003300: 7269 6465 293a 0a20 2020 2020 2020 206c  ride):.        l
-00003310: 6179 6572 7320 3d20 5b5d 0a20 2020 2020  ayers = [].     
-00003320: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00003330: 6528 6e75 6d5f 626c 6f63 6b29 3a0a 2020  e(num_block):.  
-00003340: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
-00003350: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00003360: 2020 2020 206c 6179 6572 732e 6170 7065       layers.appe
-00003370: 6e64 2862 6c6f 636b 2873 656c 662e 696e  nd(block(self.in
-00003380: 5f70 6c61 6e65 732c 2070 6c61 6e65 732c  _planes, planes,
-00003390: 2073 7472 6964 6529 290a 2020 2020 2020   stride)).      
-000033a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000033b0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-000033c0: 7273 2e61 7070 656e 6428 626c 6f63 6b28  rs.append(block(
-000033d0: 706c 616e 6573 2c20 706c 616e 6573 2c20  planes, planes, 
-000033e0: 3129 290a 2020 2020 2020 2020 7365 6c66  1)).        self
-000033f0: 2e69 6e5f 706c 616e 6573 203d 2070 6c61  .in_planes = pla
-00003400: 6e65 730a 2020 2020 2020 2020 7265 7475  nes.        retu
-00003410: 726e 206e 6e2e 5365 7175 656e 7469 616c  rn nn.Sequential
-00003420: 282a 6c61 7965 7273 290a 0a20 2020 2064  (*layers)..    d
-00003430: 6566 2066 6f72 7761 7264 2873 656c 662c  ef forward(self,
-00003440: 2078 293a 0a20 2020 2020 2020 2078 203d   x):.        x =
-00003450: 2073 656c 662e 6d61 7870 6f6f 6c28 7365   self.maxpool(se
-00003460: 6c66 2e63 6f6e 7631 2878 2929 0a20 2020  lf.conv1(x)).   
-00003470: 2020 2020 2078 203d 2073 656c 662e 626c       x = self.bl
-00003480: 6f63 6b31 2878 2920 2023 205b 3230 302c  ock1(x)  # [200,
-00003490: 2036 342c 2032 382c 2032 385d 0a20 2020   64, 28, 28].   
-000034a0: 2020 2020 2078 203d 2073 656c 662e 626c       x = self.bl
-000034b0: 6f63 6b32 2878 2920 2023 205b 3230 302c  ock2(x)  # [200,
-000034c0: 2031 3238 2c20 3134 2c20 3134 5d0a 2020   128, 14, 14].  
-000034d0: 2020 2020 2020 7820 3d20 7365 6c66 2e62        x = self.b
-000034e0: 6c6f 636b 3328 7829 2020 2320 5b32 3030  lock3(x)  # [200
-000034f0: 2c20 3235 362c 2037 2c20 375d 0a20 2020  , 256, 7, 7].   
-00003500: 2020 2020 2023 206f 7574 203d 2073 656c       # out = sel
-00003510: 662e 626c 6f63 6b34 286f 7574 290a 2020  f.block4(out).  
-00003520: 2020 2020 2020 7820 3d20 462e 6176 675f        x = F.avg_
-00003530: 706f 6f6c 3264 2878 2c20 3729 2020 2320  pool2d(x, 7)  # 
-00003540: 5b32 3030 2c20 3235 362c 2031 2c20 315d  [200, 256, 1, 1]
-00003550: 0a20 2020 2020 2020 2078 203d 2078 2e76  .        x = x.v
-00003560: 6965 7728 782e 7369 7a65 2830 292c 202d  iew(x.size(0), -
-00003570: 3129 2020 2320 5b32 3030 2c32 3536 5d0a  1)  # [200,256].
-00003580: 2020 2020 2020 2020 6f75 7420 3d20 7365          out = se
-00003590: 6c66 2e6f 7574 6c61 7965 7228 7829 0a20  lf.outlayer(x). 
-000035a0: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-000035b0: 740a 0a0a 2320 e68d 95e8 8eb7 e5b9 b6e5  t...# ..........
-000035c0: 8faf e8a7 86e5 8c96 e589 8d32 30e5 bca0  ...........20...
-000035d0: e59b bee5 838f 0a64 6566 206c 6f67 5f69  .......def log_i
-000035e0: 6d61 6765 7328 6c6f 6164 6572 2c20 6e75  mages(loader, nu
-000035f0: 6d5f 696d 6167 6573 3d31 3629 3a0a 2020  m_images=16):.  
-00003600: 2020 696d 6167 6573 5f6c 6f67 6765 6420    images_logged 
-00003610: 3d20 300a 2020 2020 6c6f 6767 6564 5f69  = 0.    logged_i
-00003620: 6d61 6765 7320 3d20 5b5d 0a20 2020 2066  mages = [].    f
-00003630: 6f72 2069 6d61 6765 732c 206c 6162 656c  or images, label
-00003640: 7320 696e 206c 6f61 6465 723a 0a20 2020  s in loader:.   
-00003650: 2020 2020 2023 2069 6d61 6765 733a 2062       # images: b
-00003660: 6174 6368 206f 6620 696d 6167 6573 2c20  atch of images, 
-00003670: 6c61 6265 6c73 3a20 6261 7463 6820 6f66  labels: batch of
-00003680: 206c 6162 656c 730a 2020 2020 2020 2020   labels.        
-00003690: 666f 7220 6920 696e 2072 616e 6765 2869  for i in range(i
-000036a0: 6d61 6765 732e 7368 6170 655b 305d 293a  mages.shape[0]):
-000036b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000036c0: 696d 6167 6573 5f6c 6f67 6765 6420 3c20  images_logged < 
-000036d0: 6e75 6d5f 696d 6167 6573 3a0a 2020 2020  num_images:.    
-000036e0: 2020 2020 2020 2020 2020 2020 2320 e4bd              # ..
-000036f0: bfe7 94a8 7377 616e 6c61 622e 496d 6167  ....swanlab.Imag
-00003700: 65e5 b086 e59b bee5 838f e8bd ace6 8da2  e...............
-00003710: e4b8 ba77 616e 6462 e58f afe8 a786 e58c  ...wandb........
-00003720: 96e6 a0bc e5bc 8f0a 2020 2020 2020 2020  ........        
-00003730: 2020 2020 2020 2020 6c6f 6767 6564 5f69          logged_i
-00003740: 6d61 6765 732e 6170 7065 6e64 2873 7761  mages.append(swa
-00003750: 6e6c 6162 2e49 6d61 6765 2869 6d61 6765  nlab.Image(image
-00003760: 735b 695d 2c20 6361 7074 696f 6e3d 6622  s[i], caption=f"
-00003770: 4c61 6265 6c3a 207b 6c61 6265 6c73 5b69  Label: {labels[i
-00003780: 5d7d 222c 2073 697a 653d 2831 3238 2c20  ]}", size=(128, 
-00003790: 3132 3829 2929 0a20 2020 2020 2020 2020  128))).         
-000037a0: 2020 2020 2020 2069 6d61 6765 735f 6c6f         images_lo
-000037b0: 6767 6564 202b 3d20 310a 2020 2020 2020  gged += 1.      
-000037c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000037d0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000037e0: 6b0a 2020 2020 2020 2020 6966 2069 6d61  k.        if ima
-000037f0: 6765 735f 6c6f 6767 6564 203e 3d20 6e75  ges_logged >= nu
-00003800: 6d5f 696d 6167 6573 3a0a 2020 2020 2020  m_images:.      
-00003810: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00003820: 7377 616e 6c61 622e 6c6f 6728 7b22 5072  swanlab.log({"Pr
-00003830: 6576 6965 772f 4d4e 4953 5422 3a20 6c6f  eview/MNIST": lo
-00003840: 6767 6564 5f69 6d61 6765 737d 290a 0a0a  gged_images})...
-00003850: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
-00003860: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2023  __main__":.    #
-00003870: 20e8 aebe e7bd ae64 6576 6963 650a 2020   ......device.  
-00003880: 2020 7472 793a 0a20 2020 2020 2020 2075    try:.        u
-00003890: 7365 5f6d 7073 203d 2074 6f72 6368 2e62  se_mps = torch.b
-000038a0: 6163 6b65 6e64 732e 6d70 732e 6973 5f61  ackends.mps.is_a
-000038b0: 7661 696c 6162 6c65 2829 0a20 2020 2065  vailable().    e
-000038c0: 7863 6570 7420 4174 7472 6962 7574 6545  xcept AttributeE
-000038d0: 7272 6f72 3a0a 2020 2020 2020 2020 7573  rror:.        us
-000038e0: 655f 6d70 7320 3d20 4661 6c73 650a 0a20  e_mps = False.. 
-000038f0: 2020 2069 6620 746f 7263 682e 6375 6461     if torch.cuda
-00003900: 2e69 735f 6176 6169 6c61 626c 6528 293a  .is_available():
-00003910: 0a20 2020 2020 2020 2064 6576 6963 6520  .        device 
-00003920: 3d20 2263 7564 6122 0a20 2020 2065 6c69  = "cuda".    eli
-00003930: 6620 7573 655f 6d70 733a 0a20 2020 2020  f use_mps:.     
-00003940: 2020 2064 6576 6963 6520 3d20 226d 7073     device = "mps
-00003950: 220a 2020 2020 656c 7365 3a0a 2020 2020  ".    else:.    
-00003960: 2020 2020 6465 7669 6365 203d 2022 6370      device = "cp
-00003970: 7522 0a0a 2020 2020 2320 e588 9de5 a78b  u"..    # ......
-00003980: e58c 9673 7761 6e6c 6162 0a20 2020 2072  ...swanlab.    r
-00003990: 756e 203d 2073 7761 6e6c 6162 2e69 6e69  un = swanlab.ini
-000039a0: 7428 0a20 2020 2020 2020 2070 726f 6a65  t(.        proje
-000039b0: 6374 3d22 4661 7368 696f 6e4d 4e49 5354  ct="FashionMNIST
-000039c0: 222c 0a20 2020 2020 2020 2077 6f72 6b73  ",.        works
-000039d0: 7061 6365 3d22 5377 616e 4c61 6222 2c0a  pace="SwanLab",.
-000039e0: 2020 2020 2020 2020 6578 7065 7269 6d65          experime
-000039f0: 6e74 5f6e 616d 653d 2252 6573 6e65 7431  nt_name="Resnet1
-00003a00: 382d 4164 616d 222c 0a20 2020 2020 2020  8-Adam",.       
-00003a10: 2063 6f6e 6669 673d 7b0a 2020 2020 2020   config={.      
-00003a20: 2020 2020 2020 226d 6f64 656c 223a 2022        "model": "
-00003a30: 5265 736e 6574 3334 222c 0a20 2020 2020  Resnet34",.     
-00003a40: 2020 2020 2020 2022 6f70 7469 6d22 3a20         "optim": 
-00003a50: 2241 6461 6d22 2c0a 2020 2020 2020 2020  "Adam",.        
-00003a60: 2020 2020 226c 7222 3a20 302e 3030 312c      "lr": 0.001,
-00003a70: 0a20 2020 2020 2020 2020 2020 2022 6261  .            "ba
-00003a80: 7463 685f 7369 7a65 223a 2033 322c 0a20  tch_size": 32,. 
-00003a90: 2020 2020 2020 2020 2020 2022 6e75 6d5f             "num_
-00003aa0: 6570 6f63 6873 223a 2031 302c 0a20 2020  epochs": 10,.   
-00003ab0: 2020 2020 2020 2020 2022 7472 6169 6e5f           "train_
-00003ac0: 6461 7461 7365 745f 6e75 6d22 3a20 3535  dataset_num": 55
-00003ad0: 3030 302c 0a20 2020 2020 2020 2020 2020  000,.           
-00003ae0: 2022 7661 6c5f 6461 7461 7365 745f 6e75   "val_dataset_nu
-00003af0: 6d22 3a20 3530 3030 2c0a 2020 2020 2020  m": 5000,.      
-00003b00: 2020 2020 2020 2264 6576 6963 6522 3a20        "device": 
-00003b10: 6465 7669 6365 2c0a 2020 2020 2020 2020  device,.        
-00003b20: 2020 2020 226e 756d 5f63 6c61 7373 6573      "num_classes
-00003b30: 223a 2031 302c 0a20 2020 2020 2020 207d  ": 10,.        }
-00003b40: 2c0a 2020 2020 290a 0a20 2020 2023 20e8  ,.    )..    # .
-00003b50: aebe e7bd aee8 aead e7bb 83e6 9cba e380  ................
-00003b60: 81e9 aa8c e8af 81e9 9b86 e592 8ce6 b58b  ................
-00003b70: e8af 95e9 9b86 0a20 2020 2064 6174 6173  .......    datas
-00003b80: 6574 203d 2046 6173 6869 6f6e 4d4e 4953  et = FashionMNIS
-00003b90: 5428 6f73 2e67 6574 6377 6428 292c 2074  T(os.getcwd(), t
-00003ba0: 7261 696e 3d54 7275 652c 2064 6f77 6e6c  rain=True, downl
-00003bb0: 6f61 643d 5472 7565 2c20 7472 616e 7366  oad=True, transf
-00003bc0: 6f72 6d3d 546f 5465 6e73 6f72 2829 290a  orm=ToTensor()).
-00003bd0: 2020 2020 7472 6169 6e5f 6461 7461 7365      train_datase
-00003be0: 742c 2076 616c 5f64 6174 6173 6574 203d  t, val_dataset =
-00003bf0: 2075 7469 6c73 2e64 6174 612e 7261 6e64   utils.data.rand
-00003c00: 6f6d 5f73 706c 6974 280a 2020 2020 2020  om_split(.      
-00003c10: 2020 6461 7461 7365 742c 205b 7275 6e2e    dataset, [run.
-00003c20: 636f 6e66 6967 2e74 7261 696e 5f64 6174  config.train_dat
-00003c30: 6173 6574 5f6e 756d 2c20 7275 6e2e 636f  aset_num, run.co
-00003c40: 6e66 6967 2e76 616c 5f64 6174 6173 6574  nfig.val_dataset
-00003c50: 5f6e 756d 5d0a 2020 2020 290a 0a20 2020  _num].    )..   
-00003c60: 2074 7261 696e 5f6c 6f61 6465 7220 3d20   train_loader = 
-00003c70: 7574 696c 732e 6461 7461 2e44 6174 614c  utils.data.DataL
-00003c80: 6f61 6465 7228 7472 6169 6e5f 6461 7461  oader(train_data
-00003c90: 7365 742c 2062 6174 6368 5f73 697a 653d  set, batch_size=
-00003ca0: 7275 6e2e 636f 6e66 6967 2e62 6174 6368  run.config.batch
-00003cb0: 5f73 697a 652c 2073 6875 6666 6c65 3d54  _size, shuffle=T
-00003cc0: 7275 6529 0a20 2020 2076 616c 5f6c 6f61  rue).    val_loa
-00003cd0: 6465 7220 3d20 7574 696c 732e 6461 7461  der = utils.data
-00003ce0: 2e44 6174 614c 6f61 6465 7228 7661 6c5f  .DataLoader(val_
-00003cf0: 6461 7461 7365 742c 2062 6174 6368 5f73  dataset, batch_s
-00003d00: 697a 653d 312c 2073 6875 6666 6c65 3d46  ize=1, shuffle=F
-00003d10: 616c 7365 290a 0a20 2020 2023 20e5 889d  alse)..    # ...
-00003d20: e5a7 8be5 8c96 e6a8 a1e5 9e8b e380 81e6  ................
-00003d30: 8d9f e5a4 b1e5 87bd e695 b0e5 928c e4bc  ................
-00003d40: 98e5 8c96 e599 a80a 2020 2020 6966 2072  ........    if r
-00003d50: 756e 2e63 6f6e 6669 672e 6d6f 6465 6c20  un.config.model 
-00003d60: 3d3d 2022 5265 736e 6574 3138 223a 0a20  == "Resnet18":. 
-00003d70: 2020 2020 2020 206d 6f64 656c 203d 2052         model = R
-00003d80: 6573 4e65 7428 4261 7369 6362 6c6f 636b  esNet(Basicblock
-00003d90: 2c20 5b31 2c20 312c 2031 2c20 315d 2c20  , [1, 1, 1, 1], 
-00003da0: 3130 290a 2020 2020 656c 6966 2072 756e  10).    elif run
-00003db0: 2e63 6f6e 6669 672e 6d6f 6465 6c20 3d3d  .config.model ==
-00003dc0: 2022 5265 736e 6574 3334 223a 0a20 2020   "Resnet34":.   
-00003dd0: 2020 2020 206d 6f64 656c 203d 2052 6573       model = Res
-00003de0: 4e65 7428 4261 7369 6362 6c6f 636b 2c20  Net(Basicblock, 
-00003df0: 5b32 2c20 332c 2035 2c20 325d 2c20 3130  [2, 3, 5, 2], 10
-00003e00: 290a 2020 2020 656c 6966 2072 756e 2e63  ).    elif run.c
-00003e10: 6f6e 6669 672e 6d6f 6465 6c20 3d3d 2022  onfig.model == "
-00003e20: 5265 736e 6574 3530 223a 0a20 2020 2020  Resnet50":.     
-00003e30: 2020 206d 6f64 656c 203d 2052 6573 4e65     model = ResNe
-00003e40: 7428 4261 7369 6362 6c6f 636b 2c20 5b33  t(Basicblock, [3
-00003e50: 2c20 342c 2036 2c20 335d 2c20 3130 290a  , 4, 6, 3], 10).
-00003e60: 0a20 2020 206d 6f64 656c 2e74 6f28 746f  .    model.to(to
-00003e70: 7263 682e 6465 7669 6365 2864 6576 6963  rch.device(devic
-00003e80: 6529 290a 0a20 2020 2063 7269 7465 7269  e))..    criteri
-00003e90: 6f6e 203d 206e 6e2e 4372 6f73 7345 6e74  on = nn.CrossEnt
-00003ea0: 726f 7079 4c6f 7373 2829 0a20 2020 206f  ropyLoss().    o
-00003eb0: 7074 696d 697a 6572 203d 206f 7074 696d  ptimizer = optim
-00003ec0: 2e41 6461 6d28 6d6f 6465 6c2e 7061 7261  .Adam(model.para
-00003ed0: 6d65 7465 7273 2829 2c20 6c72 3d72 756e  meters(), lr=run
-00003ee0: 2e63 6f6e 6669 672e 6c72 290a 0a20 2020  .config.lr)..   
-00003ef0: 2023 20ef bc88 e58f afe9 8089 efbc 89e7   # .............
-00003f00: 9c8b e4b8 80e4 b88b e695 b0e6 8dae e99b  ................
-00003f10: 86e7 9a84 e589 8d31 36e5 bca0 e59b bee5  .......16.......
-00003f20: 838f 0a20 2020 206c 6f67 5f69 6d61 6765  ...    log_image
-00003f30: 7328 7472 6169 6e5f 6c6f 6164 6572 2c20  s(train_loader, 
-00003f40: 3136 290a 0a20 2020 2023 20e5 bc80 e5a7  16)..    # .....
-00003f50: 8be8 aead e7bb 830a 2020 2020 666f 7220  ........    for 
-00003f60: 6570 6f63 6820 696e 2072 616e 6765 2831  epoch in range(1
-00003f70: 2c20 7275 6e2e 636f 6e66 6967 2e6e 756d  , run.config.num
-00003f80: 5f65 706f 6368 7320 2b20 3129 3a0a 2020  _epochs + 1):.  
-00003f90: 2020 2020 2020 7377 616e 6c61 622e 6c6f        swanlab.lo
-00003fa0: 6728 7b22 7472 6169 6e2f 6570 6f63 6822  g({"train/epoch"
-00003fb0: 3a20 6570 6f63 687d 2c20 7374 6570 3d65  : epoch}, step=e
-00003fc0: 706f 6368 290a 2020 2020 2020 2020 2320  poch).        # 
-00003fd0: e8ae ade7 bb83 e5be aae7 8eaf 0a20 2020  .............   
-00003fe0: 2020 2020 2066 6f72 2069 7465 722c 2062       for iter, b
-00003ff0: 6174 6368 2069 6e20 656e 756d 6572 6174  atch in enumerat
-00004000: 6528 7472 6169 6e5f 6c6f 6164 6572 293a  e(train_loader):
-00004010: 0a20 2020 2020 2020 2020 2020 2078 2c20  .            x, 
-00004020: 7920 3d20 6261 7463 680a 2020 2020 2020  y = batch.      
-00004030: 2020 2020 2020 782c 2079 203d 2078 2e74        x, y = x.t
-00004040: 6f28 6465 7669 6365 292c 2079 2e74 6f28  o(device), y.to(
-00004050: 6465 7669 6365 290a 2020 2020 2020 2020  device).        
-00004060: 2020 2020 6f70 7469 6d69 7a65 722e 7a65      optimizer.ze
-00004070: 726f 5f67 7261 6428 290a 2020 2020 2020  ro_grad().      
-00004080: 2020 2020 2020 6f75 7470 7574 203d 206d        output = m
-00004090: 6f64 656c 2878 290a 2020 2020 2020 2020  odel(x).        
-000040a0: 2020 2020 6c6f 7373 203d 2063 7269 7465      loss = crite
-000040b0: 7269 6f6e 286f 7574 7075 742c 2079 290a  rion(output, y).
-000040c0: 2020 2020 2020 2020 2020 2020 6c6f 7373              loss
-000040d0: 2e62 6163 6b77 6172 6428 290a 2020 2020  .backward().    
-000040e0: 2020 2020 2020 2020 6f70 7469 6d69 7a65          optimize
-000040f0: 722e 7374 6570 2829 0a0a 2020 2020 2020  r.step()..      
-00004100: 2020 2020 2020 6966 2069 7465 7220 2520        if iter % 
-00004110: 3430 203d 3d20 303a 0a20 2020 2020 2020  40 == 0:.       
-00004120: 2020 2020 2020 2020 2070 7269 6e74 280a           print(.
-00004130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004140: 2020 2020 6622 4570 6f63 6820 5b7b 6570      f"Epoch [{ep
-00004150: 6f63 687d 2f7b 7275 6e2e 636f 6e66 6967  och}/{run.config
-00004160: 2e6e 756d 5f65 706f 6368 737d 5d2c 2049  .num_epochs}], I
-00004170: 7465 7261 7469 6f6e 205b 7b69 7465 7220  teration [{iter 
-00004180: 2b20 317d 2f7b 6c65 6e28 7472 6169 6e5f  + 1}/{len(train_
-00004190: 6c6f 6164 6572 297d 5d2c 204c 6f73 733a  loader)}], Loss:
-000041a0: 207b 6c6f 7373 2e69 7465 6d28 297d 220a   {loss.item()}".
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000041d0: 2020 7377 616e 6c61 622e 6c6f 6728 7b22    swanlab.log({"
-000041e0: 7472 6169 6e2f 6c6f 7373 223a 206c 6f73  train/loss": los
-000041f0: 732e 6974 656d 2829 7d2c 2073 7465 703d  s.item()}, step=
-00004200: 2865 706f 6368 202d 2031 2920 2a20 6c65  (epoch - 1) * le
-00004210: 6e28 7472 6169 6e5f 6c6f 6164 6572 2920  n(train_loader) 
-00004220: 2b20 6974 6572 290a 0a20 2020 2020 2020  + iter)..       
-00004230: 2023 20e6 af8f 34e4 b8aa 6570 6f63 68e9   # ...4...epoch.
-00004240: aa8c e8af 81e4 b880 e6ac a10a 2020 2020  ............    
-00004250: 2020 2020 6966 2065 706f 6368 2025 2032      if epoch % 2
-00004260: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00004270: 2020 206d 6f64 656c 2e65 7661 6c28 290a     model.eval().
-00004280: 2020 2020 2020 2020 2020 2020 636f 7272              corr
-00004290: 6563 7420 3d20 300a 2020 2020 2020 2020  ect = 0.        
-000042a0: 2020 2020 746f 7461 6c20 3d20 300a 2020      total = 0.  
-000042b0: 2020 2020 2020 2020 2020 7769 7468 2074            with t
-000042c0: 6f72 6368 2e6e 6f5f 6772 6164 2829 3a0a  orch.no_grad():.
-000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042e0: 666f 7220 6261 7463 6820 696e 2076 616c  for batch in val
-000042f0: 5f6c 6f61 6465 723a 0a20 2020 2020 2020  _loader:.       
-00004300: 2020 2020 2020 2020 2020 2020 2078 2c20               x, 
-00004310: 7920 3d20 6261 7463 680a 2020 2020 2020  y = batch.      
-00004320: 2020 2020 2020 2020 2020 2020 2020 782c                x,
-00004330: 2079 203d 2078 2e74 6f28 6465 7669 6365   y = x.to(device
-00004340: 292c 2079 2e74 6f28 6465 7669 6365 290a  ), y.to(device).
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004360: 2020 2020 6f75 7470 7574 203d 206d 6f64      output = mod
-00004370: 656c 2878 290a 2020 2020 2020 2020 2020  el(x).          
-00004380: 2020 2020 2020 2020 2020 5f2c 2070 7265            _, pre
-00004390: 6469 6374 6564 203d 2074 6f72 6368 2e6d  dicted = torch.m
-000043a0: 6178 286f 7574 7075 742c 2031 290a 2020  ax(output, 1).  
-000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043c0: 2020 746f 7461 6c20 2b3d 2079 2e73 697a    total += y.siz
-000043d0: 6528 3029 0a20 2020 2020 2020 2020 2020  e(0).           
-000043e0: 2020 2020 2020 2020 2063 6f72 7265 6374           correct
-000043f0: 202b 3d20 2870 7265 6469 6374 6564 203d   += (predicted =
-00004400: 3d20 7929 2e73 756d 2829 2e69 7465 6d28  = y).sum().item(
-00004410: 290a 0a20 2020 2020 2020 2020 2020 2061  )..            a
-00004420: 6363 7572 6163 7920 3d20 636f 7272 6563  ccuracy = correc
-00004430: 7420 2f20 746f 7461 6c0a 2020 2020 2020  t / total.      
-00004440: 2020 2020 2020 7377 616e 6c61 622e 6c6f        swanlab.lo
-00004450: 6728 7b22 7661 6c2f 6163 6375 7261 6379  g({"val/accuracy
-00004460: 223a 2061 6363 7572 6163 797d 2c20 7374  ": accuracy}, st
-00004470: 6570 3d65 706f 6368 290a 6060 600a 0a3c  ep=epoch).```..<
-00004480: 2f64 6574 6169 6c73 3e0a 0a3c 6272 3e0a  /details>..<br>.
-00004490: 0a23 2320 f09f 92bb 2053 656c 662d 686f  .## .... Self-ho
-000044a0: 7374 6564 0a0a 5468 6520 636f 6d6d 756e  sted..The commun
-000044b0: 6974 7920 6564 6974 696f 6e20 7375 7070  ity edition supp
-000044c0: 6f72 7473 206f 6666 6c69 6e65 2076 6965  orts offline vie
-000044d0: 7769 6e67 206f 6620 5377 616e 4c61 6220  wing of SwanLab 
-000044e0: 6461 7368 626f 6172 6473 2e0a 0a23 2323  dashboards...###
-000044f0: 204f 6666 6c69 6e65 2045 7870 6572 696d   Offline Experim
-00004500: 656e 7420 5472 6163 6b69 6e67 0a0a 5365  ent Tracking..Se
-00004510: 7420 7468 6520 7061 7261 6d65 7465 7273  t the parameters
-00004520: 2060 6c6f 6769 7260 2061 6e64 2060 6d6f   `logir` and `mo
-00004530: 6465 6020 696e 2073 7761 6e6c 6162 2e69  de` in swanlab.i
-00004540: 6e69 7420 746f 2074 7261 636b 2065 7870  nit to track exp
-00004550: 6572 696d 656e 7473 206f 6666 6c69 6e65  eriments offline
-00004560: 3a0a 0a60 6060 7079 7468 6f6e 0a2e 2e2e  :..```python....
-00004570: 0a0a 7377 616e 6c61 622e 696e 6974 280a  ..swanlab.init(.
-00004580: 2020 2020 6c6f 6764 6972 3d27 2e2f 6c6f      logdir='./lo
-00004590: 6773 272c 0a20 2020 206d 6f64 653d 276c  gs',.    mode='l
-000045a0: 6f63 616c 272c 0a29 0a0a 2e2e 2e0a 6060  ocal',.)......``
-000045b0: 600a 0a2d 2054 6865 2070 6172 616d 6574  `..- The paramet
-000045c0: 6572 2060 6d6f 6465 6020 6973 2073 6574  er `mode` is set
-000045d0: 2074 6f20 606c 6f63 616c 602c 2077 6869   to `local`, whi
-000045e0: 6368 2064 6973 6162 6c65 7320 7379 6e63  ch disables sync
-000045f0: 6872 6f6e 697a 696e 6720 7468 6520 6578  hronizing the ex
-00004600: 7065 7269 6d65 6e74 2074 6f20 7468 6520  periment to the 
-00004610: 636c 6f75 642e 0a0a 2d20 5468 6520 7365  cloud...- The se
-00004620: 7474 696e 6720 6f66 2074 6865 2070 6172  tting of the par
-00004630: 616d 6574 6572 2060 6c6f 6764 6972 6020  ameter `logdir` 
-00004640: 6973 206f 7074 696f 6e61 6c2c 2061 6e64  is optional, and
-00004650: 2069 7420 7370 6563 6966 6965 7320 7468   it specifies th
-00004660: 6520 6c6f 6361 7469 6f6e 2066 6f72 2073  e location for s
-00004670: 6176 696e 6720 5377 616e 4c61 6220 6c6f  aving SwanLab lo
-00004680: 6720 6669 6c65 7320 2862 790a 2020 6465  g files (by.  de
-00004690: 6661 756c 7420 7361 7665 6420 696e 2074  fault saved in t
-000046a0: 6865 2060 7377 616e 6c6f 6760 2066 6f6c  he `swanlog` fol
-000046b0: 6465 7229 2e0a 0a2d 204c 6f67 2066 696c  der)...- Log fil
-000046c0: 6573 2077 696c 6c20 6265 2063 7265 6174  es will be creat
-000046d0: 6564 2061 6e64 2075 7064 6174 6564 2064  ed and updated d
-000046e0: 7572 696e 6720 7472 6163 6b69 6e67 206f  uring tracking o
-000046f0: 6620 6578 7065 7269 6d65 6e74 732c 2061  f experiments, a
-00004700: 6e64 206c 6175 6e63 6869 6e67 206f 6666  nd launching off
-00004710: 6c69 6e65 2064 6173 6862 6f61 7264 7320  line dashboards 
-00004720: 7769 6c6c 2061 6c73 6f20 6265 0a20 2062  will also be.  b
-00004730: 6173 6564 206f 6e20 7468 6573 6520 6c6f  ased on these lo
-00004740: 6720 6669 6c65 732e 0a0a 4f74 6865 7220  g files...Other 
-00004750: 7061 7274 7320 6172 6520 636f 6d70 6c65  parts are comple
-00004760: 7465 6c79 2063 6f6e 7369 7374 656e 7420  tely consistent 
-00004770: 7769 7468 2063 6c6f 7564 2075 7361 6765  with cloud usage
-00004780: 2e0a 0a23 2323 204f 7065 6e20 4f66 666c  ...### Open Offl
-00004790: 696e 6520 426f 6172 640a 0a4f 7065 6e20  ine Board..Open 
-000047a0: 7468 6520 7465 726d 696e 616c 2061 6e64  the terminal and
-000047b0: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-000047c0: 6e67 2063 6f6d 6d61 6e64 2074 6f20 6f70  ng command to op
-000047d0: 656e 2061 2053 7761 6e4c 6162 2064 6173  en a SwanLab das
-000047e0: 6862 6f61 7264 3a0a 0a60 6060 6261 7368  hboard:..```bash
-000047f0: 0a73 7761 6e6c 6162 2077 6174 6368 202d  .swanlab watch -
-00004800: 6c20 2e2f 6c6f 6773 0a60 6060 0a0a 4166  l ./logs.```..Af
-00004810: 7465 7220 7468 6520 6f70 6572 6174 696f  ter the operatio
-00004820: 6e20 6973 2063 6f6d 706c 6574 6564 2c20  n is completed, 
-00004830: 5377 616e 4c61 6220 7769 6c6c 2070 726f  SwanLab will pro
-00004840: 7669 6465 2079 6f75 2077 6974 6820 6120  vide you with a 
-00004850: 6c6f 6361 6c20 5552 4c20 6c69 6e6b 2028  local URL link (
-00004860: 6465 6661 756c 740a 6973 205b 6874 7470  default.is [http
-00004870: 3a2f 2f31 3237 2e30 2e30 2e31 3a35 3039  ://127.0.0.1:509
-00004880: 325d 2868 7474 703a 2f2f 3132 372e 302e  2](http://127.0.
-00004890: 302e 313a 3530 3932 2929 2e0a 0a56 6973  0.1:5092))...Vis
-000048a0: 6974 2074 6869 7320 6c69 6e6b 2074 6f20  it this link to 
-000048b0: 7669 6577 2074 6865 2065 7870 6572 696d  view the experim
-000048c0: 656e 7420 6f66 666c 696e 6520 696e 2074  ent offline in t
-000048d0: 6865 2062 726f 7773 6572 2064 6173 6862  he browser dashb
-000048e0: 6f61 7264 2e0a 0a3c 6272 3e0a 0a23 2320  oard...<br>..## 
-000048f0: f09f 9a97 2049 6e74 6567 7261 7469 6f6e  .... Integration
-00004900: 0a0a 436f 6d62 696e 6520 796f 7572 2066  ..Combine your f
-00004910: 6176 6f72 6974 6520 6672 616d 6577 6f72  avorite framewor
-00004920: 6b20 7769 7468 0a53 7761 6e4c 6162 2c20  k with.SwanLab, 
-00004930: 5b4d 6f72 6520 496e 7465 6772 6174 696f  [More Integratio
-00004940: 6e5d 2868 7474 7073 3a2f 2f64 6f63 732e  n](https://docs.
-00004950: 7377 616e 6c61 622e 636e 2f7a 682f 6775  swanlab.cn/zh/gu
-00004960: 6964 655f 636c 6f75 642f 696e 7465 6772  ide_cloud/integr
-00004970: 6174 696f 6e2f 696e 7465 6772 6174 696f  ation/integratio
-00004980: 6e2d 7079 746f 7263 682d 6c69 6768 746e  n-pytorch-lightn
-00004990: 696e 672e 6874 6d6c 292e 0a0a 3c64 6574  ing.html)...<det
-000049a0: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
-000049b0: 3e0a 2020 2020 3c73 7472 6f6e 673e e29a  >.    <strong>..
-000049c0: a1ef b88f 2050 7954 6f72 6368 204c 6967  .... PyTorch Lig
-000049d0: 6874 6e69 6e67 3c2f 7374 726f 6e67 3e0a  htning</strong>.
-000049e0: 2020 3c2f 7375 6d6d 6172 793e 0a20 203c    </summary>.  <
-000049f0: 6272 3e0a 0a43 7265 6174 6520 616e 2069  br>..Create an i
-00004a00: 6e73 7461 6e63 6520 7573 696e 6720 6053  nstance using `S
-00004a10: 7761 6e4c 6162 4c6f 6767 6572 6020 616e  wanLabLogger` an
-00004a20: 6420 7061 7373 2069 7420 696e 746f 2074  d pass it into t
-00004a30: 6865 2060 6c6f 6767 6572 6020 7061 7261  he `logger` para
-00004a40: 6d65 7465 7220 6f66 2060 5472 6169 6e65  meter of `Traine
-00004a50: 7260 2074 6f20 656e 6162 6c65 2053 7761  r` to enable Swa
-00004a60: 6e4c 6162 2074 6f0a 7265 636f 7264 2074  nLab to.record t
-00004a70: 7261 696e 696e 6720 6d65 7472 6963 732e  raining metrics.
-00004a80: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00004a90: 2073 7761 6e6c 6162 2e69 6e74 6567 7261   swanlab.integra
-00004aa0: 7469 6f6e 2e70 7974 6f72 6368 5f6c 6967  tion.pytorch_lig
-00004ab0: 6874 6e69 6e67 2069 6d70 6f72 7420 5377  htning import Sw
-00004ac0: 616e 4c61 624c 6f67 6765 720a 696d 706f  anLabLogger.impo
-00004ad0: 7274 2069 6d70 6f72 746c 6962 2e75 7469  rt importlib.uti
-00004ae0: 6c0a 696d 706f 7274 206f 730a 696d 706f  l.import os.impo
-00004af0: 7274 2070 7974 6f72 6368 5f6c 6967 6874  rt pytorch_light
-00004b00: 6e69 6e67 2061 7320 706c 0a66 726f 6d20  ning as pl.from 
-00004b10: 746f 7263 6820 696d 706f 7274 206e 6e2c  torch import nn,
-00004b20: 206f 7074 696d 2c20 7574 696c 730a 6672   optim, utils.fr
-00004b30: 6f6d 2074 6f72 6368 7669 7369 6f6e 2e64  om torchvision.d
-00004b40: 6174 6173 6574 7320 696d 706f 7274 204d  atasets import M
-00004b50: 4e49 5354 0a66 726f 6d20 746f 7263 6876  NIST.from torchv
-00004b60: 6973 696f 6e2e 7472 616e 7366 6f72 6d73  ision.transforms
-00004b70: 2069 6d70 6f72 7420 546f 5465 6e73 6f72   import ToTensor
-00004b80: 0a0a 656e 636f 6465 7220 3d20 6e6e 2e53  ..encoder = nn.S
-00004b90: 6571 7565 6e74 6961 6c28 6e6e 2e4c 696e  equential(nn.Lin
-00004ba0: 6561 7228 3238 202a 2032 382c 2031 3238  ear(28 * 28, 128
-00004bb0: 292c 206e 6e2e 5265 4c55 2829 2c20 6e6e  ), nn.ReLU(), nn
-00004bc0: 2e4c 696e 6561 7228 3132 382c 2033 2929  .Linear(128, 3))
-00004bd0: 0a64 6563 6f64 6572 203d 206e 6e2e 5365  .decoder = nn.Se
-00004be0: 7175 656e 7469 616c 286e 6e2e 4c69 6e65  quential(nn.Line
-00004bf0: 6172 2833 2c20 3132 3829 2c20 6e6e 2e52  ar(3, 128), nn.R
-00004c00: 654c 5528 292c 206e 6e2e 4c69 6e65 6172  eLU(), nn.Linear
-00004c10: 2831 3238 2c20 3238 202a 2032 3829 290a  (128, 28 * 28)).
-00004c20: 0a0a 636c 6173 7320 4c69 7441 7574 6f45  ..class LitAutoE
-00004c30: 6e63 6f64 6572 2870 6c2e 4c69 6768 746e  ncoder(pl.Lightn
-00004c40: 696e 674d 6f64 756c 6529 3a0a 2020 2020  ingModule):.    
-00004c50: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00004c60: 662c 2065 6e63 6f64 6572 2c20 6465 636f  f, encoder, deco
-00004c70: 6465 7229 3a0a 2020 2020 2020 2020 7375  der):.        su
-00004c80: 7065 7228 292e 5f5f 696e 6974 5f5f 2829  per().__init__()
-00004c90: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-00004ca0: 636f 6465 7220 3d20 656e 636f 6465 720a  coder = encoder.
-00004cb0: 2020 2020 2020 2020 7365 6c66 2e64 6563          self.dec
-00004cc0: 6f64 6572 203d 2064 6563 6f64 6572 0a0a  oder = decoder..
-00004cd0: 2020 2020 6465 6620 7472 6169 6e69 6e67      def training
-00004ce0: 5f73 7465 7028 7365 6c66 2c20 6261 7463  _step(self, batc
-00004cf0: 682c 2062 6174 6368 5f69 6478 293a 0a20  h, batch_idx):. 
-00004d00: 2020 2020 2020 2023 2074 7261 696e 696e         # trainin
-00004d10: 675f 7374 6570 2064 6566 696e 6573 2074  g_step defines t
-00004d20: 6865 2074 7261 696e 206c 6f6f 702e 0a20  he train loop.. 
-00004d30: 2020 2020 2020 2023 2069 7420 6973 2069         # it is i
-00004d40: 6e64 6570 656e 6465 6e74 206f 6620 666f  ndependent of fo
-00004d50: 7277 6172 640a 2020 2020 2020 2020 782c  rward.        x,
-00004d60: 2079 203d 2062 6174 6368 0a20 2020 2020   y = batch.     
-00004d70: 2020 2078 203d 2078 2e76 6965 7728 782e     x = x.view(x.
-00004d80: 7369 7a65 2830 292c 202d 3129 0a20 2020  size(0), -1).   
-00004d90: 2020 2020 207a 203d 2073 656c 662e 656e       z = self.en
-00004da0: 636f 6465 7228 7829 0a20 2020 2020 2020  coder(x).       
-00004db0: 2078 5f68 6174 203d 2073 656c 662e 6465   x_hat = self.de
-00004dc0: 636f 6465 7228 7a29 0a20 2020 2020 2020  coder(z).       
-00004dd0: 206c 6f73 7320 3d20 6e6e 2e66 756e 6374   loss = nn.funct
-00004de0: 696f 6e61 6c2e 6d73 655f 6c6f 7373 2878  ional.mse_loss(x
-00004df0: 5f68 6174 2c20 7829 0a20 2020 2020 2020  _hat, x).       
-00004e00: 2023 204c 6f67 6769 6e67 2074 6f20 5465   # Logging to Te
-00004e10: 6e73 6f72 426f 6172 6420 2869 6620 696e  nsorBoard (if in
-00004e20: 7374 616c 6c65 6429 2062 7920 6465 6661  stalled) by defa
-00004e30: 756c 740a 2020 2020 2020 2020 7365 6c66  ult.        self
-00004e40: 2e6c 6f67 2822 7472 6169 6e5f 6c6f 7373  .log("train_loss
-00004e50: 222c 206c 6f73 7329 0a20 2020 2020 2020  ", loss).       
-00004e60: 2072 6574 7572 6e20 6c6f 7373 0a0a 2020   return loss..  
-00004e70: 2020 6465 6620 7465 7374 5f73 7465 7028    def test_step(
-00004e80: 7365 6c66 2c20 6261 7463 682c 2062 6174  self, batch, bat
-00004e90: 6368 5f69 6478 293a 0a20 2020 2020 2020  ch_idx):.       
-00004ea0: 2023 2074 6573 745f 7374 6570 2064 6566   # test_step def
-00004eb0: 696e 6573 2074 6865 2074 6573 7420 6c6f  ines the test lo
-00004ec0: 6f70 2e0a 2020 2020 2020 2020 2320 6974  op..        # it
-00004ed0: 2069 7320 696e 6465 7065 6e64 656e 7420   is independent 
-00004ee0: 6f66 2066 6f72 7761 7264 0a20 2020 2020  of forward.     
-00004ef0: 2020 2078 2c20 7920 3d20 6261 7463 680a     x, y = batch.
-00004f00: 2020 2020 2020 2020 7820 3d20 782e 7669          x = x.vi
-00004f10: 6577 2878 2e73 697a 6528 3029 2c20 2d31  ew(x.size(0), -1
-00004f20: 290a 2020 2020 2020 2020 7a20 3d20 7365  ).        z = se
-00004f30: 6c66 2e65 6e63 6f64 6572 2878 290a 2020  lf.encoder(x).  
-00004f40: 2020 2020 2020 785f 6861 7420 3d20 7365        x_hat = se
-00004f50: 6c66 2e64 6563 6f64 6572 287a 290a 2020  lf.decoder(z).  
-00004f60: 2020 2020 2020 6c6f 7373 203d 206e 6e2e        loss = nn.
-00004f70: 6675 6e63 7469 6f6e 616c 2e6d 7365 5f6c  functional.mse_l
-00004f80: 6f73 7328 785f 6861 742c 2078 290a 2020  oss(x_hat, x).  
-00004f90: 2020 2020 2020 2320 4c6f 6767 696e 6720        # Logging 
-00004fa0: 746f 2054 656e 736f 7242 6f61 7264 2028  to TensorBoard (
-00004fb0: 6966 2069 6e73 7461 6c6c 6564 2920 6279  if installed) by
-00004fc0: 2064 6566 6175 6c74 0a20 2020 2020 2020   default.       
-00004fd0: 2073 656c 662e 6c6f 6728 2274 6573 745f   self.log("test_
-00004fe0: 6c6f 7373 222c 206c 6f73 7329 0a20 2020  loss", loss).   
-00004ff0: 2020 2020 2072 6574 7572 6e20 6c6f 7373       return loss
-00005000: 0a0a 2020 2020 6465 6620 636f 6e66 6967  ..    def config
-00005010: 7572 655f 6f70 7469 6d69 7a65 7273 2873  ure_optimizers(s
-00005020: 656c 6629 3a0a 2020 2020 2020 2020 6f70  elf):.        op
-00005030: 7469 6d69 7a65 7220 3d20 6f70 7469 6d2e  timizer = optim.
-00005040: 4164 616d 2873 656c 662e 7061 7261 6d65  Adam(self.parame
-00005050: 7465 7273 2829 2c20 6c72 3d31 652d 3329  ters(), lr=1e-3)
-00005060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005070: 6f70 7469 6d69 7a65 720a 0a0a 2320 696e  optimizer...# in
-00005080: 6974 2074 6865 2061 7574 6f65 6e63 6f64  it the autoencod
-00005090: 6572 0a61 7574 6f65 6e63 6f64 6572 203d  er.autoencoder =
-000050a0: 204c 6974 4175 746f 456e 636f 6465 7228   LitAutoEncoder(
-000050b0: 656e 636f 6465 722c 2064 6563 6f64 6572  encoder, decoder
-000050c0: 290a 0a23 2073 6574 7570 2064 6174 610a  )..# setup data.
-000050d0: 6461 7461 7365 7420 3d20 4d4e 4953 5428  dataset = MNIST(
-000050e0: 6f73 2e67 6574 6377 6428 292c 2074 7261  os.getcwd(), tra
-000050f0: 696e 3d54 7275 652c 2064 6f77 6e6c 6f61  in=True, downloa
-00005100: 643d 5472 7565 2c20 7472 616e 7366 6f72  d=True, transfor
-00005110: 6d3d 546f 5465 6e73 6f72 2829 290a 7472  m=ToTensor()).tr
-00005120: 6169 6e5f 6461 7461 7365 742c 2076 616c  ain_dataset, val
-00005130: 5f64 6174 6173 6574 203d 2075 7469 6c73  _dataset = utils
-00005140: 2e64 6174 612e 7261 6e64 6f6d 5f73 706c  .data.random_spl
-00005150: 6974 2864 6174 6173 6574 2c20 5b35 3530  it(dataset, [550
-00005160: 3030 2c20 3530 3030 5d29 0a74 6573 745f  00, 5000]).test_
-00005170: 6461 7461 7365 7420 3d20 4d4e 4953 5428  dataset = MNIST(
-00005180: 6f73 2e67 6574 6377 6428 292c 2074 7261  os.getcwd(), tra
-00005190: 696e 3d46 616c 7365 2c20 646f 776e 6c6f  in=False, downlo
-000051a0: 6164 3d54 7275 652c 2074 7261 6e73 666f  ad=True, transfo
-000051b0: 726d 3d54 6f54 656e 736f 7228 2929 0a0a  rm=ToTensor())..
-000051c0: 7472 6169 6e5f 6c6f 6164 6572 203d 2075  train_loader = u
-000051d0: 7469 6c73 2e64 6174 612e 4461 7461 4c6f  tils.data.DataLo
-000051e0: 6164 6572 2874 7261 696e 5f64 6174 6173  ader(train_datas
-000051f0: 6574 290a 7661 6c5f 6c6f 6164 6572 203d  et).val_loader =
-00005200: 2075 7469 6c73 2e64 6174 612e 4461 7461   utils.data.Data
-00005210: 4c6f 6164 6572 2876 616c 5f64 6174 6173  Loader(val_datas
-00005220: 6574 290a 7465 7374 5f6c 6f61 6465 7220  et).test_loader 
-00005230: 3d20 7574 696c 732e 6461 7461 2e44 6174  = utils.data.Dat
-00005240: 614c 6f61 6465 7228 7465 7374 5f64 6174  aLoader(test_dat
-00005250: 6173 6574 290a 0a73 7761 6e6c 6162 5f6c  aset)..swanlab_l
-00005260: 6f67 6765 7220 3d20 5377 616e 4c61 624c  ogger = SwanLabL
-00005270: 6f67 6765 7228 0a20 2020 2070 726f 6a65  ogger(.    proje
-00005280: 6374 3d22 7377 616e 6c61 625f 6578 616d  ct="swanlab_exam
-00005290: 706c 6522 2c0a 2020 2020 6578 7065 7269  ple",.    experi
-000052a0: 6d65 6e74 5f6e 616d 653d 2265 7861 6d70  ment_name="examp
-000052b0: 6c65 5f65 7870 6572 696d 656e 7422 2c0a  le_experiment",.
-000052c0: 2020 2020 636c 6f75 643d 4661 6c73 652c      cloud=False,
-000052d0: 0a29 0a0a 7472 6169 6e65 7220 3d20 706c  .)..trainer = pl
-000052e0: 2e54 7261 696e 6572 286c 696d 6974 5f74  .Trainer(limit_t
-000052f0: 7261 696e 5f62 6174 6368 6573 3d31 3030  rain_batches=100
-00005300: 2c20 6d61 785f 6570 6f63 6873 3d35 2c20  , max_epochs=5, 
-00005310: 6c6f 6767 6572 3d73 7761 6e6c 6162 5f6c  logger=swanlab_l
-00005320: 6f67 6765 7229 0a0a 7472 6169 6e65 722e  ogger)..trainer.
-00005330: 6669 7428 6d6f 6465 6c3d 6175 746f 656e  fit(model=autoen
-00005340: 636f 6465 722c 2074 7261 696e 5f64 6174  coder, train_dat
-00005350: 616c 6f61 6465 7273 3d74 7261 696e 5f6c  aloaders=train_l
-00005360: 6f61 6465 722c 2076 616c 5f64 6174 616c  oader, val_datal
-00005370: 6f61 6465 7273 3d76 616c 5f6c 6f61 6465  oaders=val_loade
-00005380: 7229 0a74 7261 696e 6572 2e74 6573 7428  r).trainer.test(
-00005390: 6461 7461 6c6f 6164 6572 733d 7465 7374  dataloaders=test
-000053a0: 5f6c 6f61 6465 7229 0a0a 6060 600a 0a3c  _loader)..```..<
-000053b0: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
-000053c0: 696c 733e 0a3c 7375 6d6d 6172 793e 0a20  ils>.<summary>. 
-000053d0: 203c 7374 726f 6e67 3e20 f09f a497 4875   <strong> ....Hu
-000053e0: 6767 696e 6746 6163 6520 5472 616e 7366  ggingFace Transf
-000053f0: 6f72 6d65 7273 3c2f 7374 726f 6e67 3e0a  ormers</strong>.
-00005400: 3c2f 7375 6d6d 6172 793e 0a0a 3c62 723e  </summary>..<br>
-00005410: 0a0a 4372 6561 7465 2061 6e20 696e 7374  ..Create an inst
-00005420: 616e 6365 2075 7369 6e67 2060 5377 616e  ance using `Swan
-00005430: 4c61 6243 616c 6c62 6163 6b60 2061 6e64  LabCallback` and
-00005440: 2070 6173 7320 6974 2069 6e74 6f20 7468   pass it into th
-00005450: 6520 6063 616c 6c62 6163 6b73 6020 7061  e `callbacks` pa
-00005460: 7261 6d65 7465 7220 6f66 2060 5472 6169  rameter of `Trai
-00005470: 6e65 7260 2074 6f20 656e 6162 6c65 2053  ner` to enable S
-00005480: 7761 6e4c 6162 2074 6f0a 7265 636f 7264  wanLab to.record
-00005490: 2074 7261 696e 696e 6720 6d65 7472 6963   training metric
-000054a0: 732e 0a0a 6060 6070 7974 686f 6e0a 696d  s...```python.im
-000054b0: 706f 7274 2065 7661 6c75 6174 650a 696d  port evaluate.im
-000054c0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-000054d0: 0a69 6d70 6f72 7420 7377 616e 6c61 620a  .import swanlab.
-000054e0: 6672 6f6d 2073 7761 6e6c 6162 2e69 6e74  from swanlab.int
-000054f0: 6567 7261 7469 6f6e 2e68 7567 6769 6e67  egration.hugging
-00005500: 6661 6365 2069 6d70 6f72 7420 5377 616e  face import Swan
-00005510: 4c61 6243 616c 6c62 6163 6b0a 6672 6f6d  LabCallback.from
-00005520: 2064 6174 6173 6574 7320 696d 706f 7274   datasets import
-00005530: 206c 6f61 645f 6461 7461 7365 740a 6672   load_dataset.fr
-00005540: 6f6d 2074 7261 6e73 666f 726d 6572 7320  om transformers 
-00005550: 696d 706f 7274 2041 7574 6f4d 6f64 656c  import AutoModel
-00005560: 466f 7253 6571 7565 6e63 6543 6c61 7373  ForSequenceClass
-00005570: 6966 6963 6174 696f 6e2c 2041 7574 6f54  ification, AutoT
-00005580: 6f6b 656e 697a 6572 2c20 5472 6169 6e65  okenizer, Traine
-00005590: 722c 2054 7261 696e 696e 6741 7267 756d  r, TrainingArgum
-000055a0: 656e 7473 0a0a 0a64 6566 2074 6f6b 656e  ents...def token
-000055b0: 697a 655f 6675 6e63 7469 6f6e 2865 7861  ize_function(exa
-000055c0: 6d70 6c65 7329 3a0a 2020 2020 7265 7475  mples):.    retu
-000055d0: 726e 2074 6f6b 656e 697a 6572 2865 7861  rn tokenizer(exa
-000055e0: 6d70 6c65 735b 2274 6578 7422 5d2c 2070  mples["text"], p
-000055f0: 6164 6469 6e67 3d22 6d61 785f 6c65 6e67  adding="max_leng
-00005600: 7468 222c 2074 7275 6e63 6174 696f 6e3d  th", truncation=
-00005610: 5472 7565 290a 0a0a 6465 6620 636f 6d70  True)...def comp
-00005620: 7574 655f 6d65 7472 6963 7328 6576 616c  ute_metrics(eval
-00005630: 5f70 7265 6429 3a0a 2020 2020 6c6f 6769  _pred):.    logi
-00005640: 7473 2c20 6c61 6265 6c73 203d 2065 7661  ts, labels = eva
-00005650: 6c5f 7072 6564 0a20 2020 2070 7265 6469  l_pred.    predi
-00005660: 6374 696f 6e73 203d 206e 702e 6172 676d  ctions = np.argm
-00005670: 6178 286c 6f67 6974 732c 2061 7869 733d  ax(logits, axis=
-00005680: 2d31 290a 2020 2020 7265 7475 726e 206d  -1).    return m
-00005690: 6574 7269 632e 636f 6d70 7574 6528 7072  etric.compute(pr
-000056a0: 6564 6963 7469 6f6e 733d 7072 6564 6963  edictions=predic
-000056b0: 7469 6f6e 732c 2072 6566 6572 656e 6365  tions, reference
-000056c0: 733d 6c61 6265 6c73 290a 0a0a 6461 7461  s=labels)...data
-000056d0: 7365 7420 3d20 6c6f 6164 5f64 6174 6173  set = load_datas
-000056e0: 6574 2822 7965 6c70 5f72 6576 6965 775f  et("yelp_review_
-000056f0: 6675 6c6c 2229 0a0a 746f 6b65 6e69 7a65  full")..tokenize
-00005700: 7220 3d20 4175 746f 546f 6b65 6e69 7a65  r = AutoTokenize
-00005710: 722e 6672 6f6d 5f70 7265 7472 6169 6e65  r.from_pretraine
-00005720: 6428 2262 6572 742d 6261 7365 2d63 6173  d("bert-base-cas
-00005730: 6564 2229 0a0a 746f 6b65 6e69 7a65 645f  ed")..tokenized_
-00005740: 6461 7461 7365 7473 203d 2064 6174 6173  datasets = datas
-00005750: 6574 2e6d 6170 2874 6f6b 656e 697a 655f  et.map(tokenize_
-00005760: 6675 6e63 7469 6f6e 2c20 6261 7463 6865  function, batche
-00005770: 643d 5472 7565 290a 0a73 6d61 6c6c 5f74  d=True)..small_t
-00005780: 7261 696e 5f64 6174 6173 6574 203d 2074  rain_dataset = t
-00005790: 6f6b 656e 697a 6564 5f64 6174 6173 6574  okenized_dataset
-000057a0: 735b 2274 7261 696e 225d 2e73 6875 6666  s["train"].shuff
-000057b0: 6c65 2873 6565 643d 3432 292e 7365 6c65  le(seed=42).sele
-000057c0: 6374 2872 616e 6765 2831 3030 3029 290a  ct(range(1000)).
-000057d0: 736d 616c 6c5f 6576 616c 5f64 6174 6173  small_eval_datas
-000057e0: 6574 203d 2074 6f6b 656e 697a 6564 5f64  et = tokenized_d
-000057f0: 6174 6173 6574 735b 2274 6573 7422 5d2e  atasets["test"].
-00005800: 7368 7566 666c 6528 7365 6564 3d34 3229  shuffle(seed=42)
-00005810: 2e73 656c 6563 7428 7261 6e67 6528 3130  .select(range(10
-00005820: 3030 2929 0a0a 6d65 7472 6963 203d 2065  00))..metric = e
-00005830: 7661 6c75 6174 652e 6c6f 6164 2822 6163  valuate.load("ac
-00005840: 6375 7261 6379 2229 0a0a 6d6f 6465 6c20  curacy")..model 
-00005850: 3d20 4175 746f 4d6f 6465 6c46 6f72 5365  = AutoModelForSe
-00005860: 7175 656e 6365 436c 6173 7369 6669 6361  quenceClassifica
-00005870: 7469 6f6e 2e66 726f 6d5f 7072 6574 7261  tion.from_pretra
-00005880: 696e 6564 2822 6265 7274 2d62 6173 652d  ined("bert-base-
-00005890: 6361 7365 6422 2c20 6e75 6d5f 6c61 6265  cased", num_labe
-000058a0: 6c73 3d35 290a 0a74 7261 696e 696e 675f  ls=5)..training_
-000058b0: 6172 6773 203d 2054 7261 696e 696e 6741  args = TrainingA
-000058c0: 7267 756d 656e 7473 280a 2020 2020 6f75  rguments(.    ou
-000058d0: 7470 7574 5f64 6972 3d22 7465 7374 5f74  tput_dir="test_t
-000058e0: 7261 696e 6572 222c 0a20 2020 2072 6570  rainer",.    rep
-000058f0: 6f72 745f 746f 3d22 6e6f 6e65 222c 0a20  ort_to="none",. 
-00005900: 2020 206e 756d 5f74 7261 696e 5f65 706f     num_train_epo
-00005910: 6368 733d 332c 0a20 2020 206c 6f67 6769  chs=3,.    loggi
-00005920: 6e67 5f73 7465 7073 3d35 302c 0a29 0a0a  ng_steps=50,.)..
-00005930: 7377 616e 6c61 625f 6361 6c6c 6261 636b  swanlab_callback
-00005940: 203d 2053 7761 6e4c 6162 4361 6c6c 6261   = SwanLabCallba
-00005950: 636b 2865 7870 6572 696d 656e 745f 6e61  ck(experiment_na
-00005960: 6d65 3d22 5472 616e 7366 6f72 6d65 7273  me="Transformers
-00005970: 5465 7374 222c 2063 6c6f 7564 3d46 616c  Test", cloud=Fal
-00005980: 7365 290a 0a74 7261 696e 6572 203d 2054  se)..trainer = T
-00005990: 7261 696e 6572 280a 2020 2020 6d6f 6465  rainer(.    mode
-000059a0: 6c3d 6d6f 6465 6c2c 0a20 2020 2061 7267  l=model,.    arg
-000059b0: 733d 7472 6169 6e69 6e67 5f61 7267 732c  s=training_args,
-000059c0: 0a20 2020 2074 7261 696e 5f64 6174 6173  .    train_datas
-000059d0: 6574 3d73 6d61 6c6c 5f74 7261 696e 5f64  et=small_train_d
-000059e0: 6174 6173 6574 2c0a 2020 2020 6576 616c  ataset,.    eval
-000059f0: 5f64 6174 6173 6574 3d73 6d61 6c6c 5f65  _dataset=small_e
-00005a00: 7661 6c5f 6461 7461 7365 742c 0a20 2020  val_dataset,.   
-00005a10: 2063 6f6d 7075 7465 5f6d 6574 7269 6373   compute_metrics
-00005a20: 3d63 6f6d 7075 7465 5f6d 6574 7269 6373  =compute_metrics
-00005a30: 2c0a 2020 2020 6361 6c6c 6261 636b 733d  ,.    callbacks=
-00005a40: 5b73 7761 6e6c 6162 5f63 616c 6c62 6163  [swanlab_callbac
-00005a50: 6b5d 2c0a 290a 0a74 7261 696e 6572 2e74  k],.)..trainer.t
-00005a60: 7261 696e 2829 0a60 6060 0a0a 3c2f 6465  rain().```..</de
-00005a70: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
-00005a80: 3e0a 3c73 756d 6d61 7279 3e0a 2020 3c73  >.<summary>.  <s
-00005a90: 7472 6f6e 673e 204d 4d45 6e67 696e 6528  trong> MMEngine(
-00005aa0: 4d4d 4465 7465 6374 696f 6e20 6574 632e  MMDetection etc.
-00005ab0: 293c 2f73 7472 6f6e 673e 0a3c 2f73 756d  )</strong>.</sum
-00005ac0: 6d61 7279 3e0a 3c62 723e 0a0a 496e 7465  mary>.<br>..Inte
-00005ad0: 6772 6174 6520 6053 7761 6e6c 6162 5669  grate `SwanlabVi
-00005ae0: 7342 6163 6b65 6e64 6020 696e 746f 204d  sBackend` into M
-00005af0: 4d45 6e67 696e 6520 746f 2065 6e61 626c  MEngine to enabl
-00005b00: 6520 6175 746f 6d61 7469 6320 6c6f 6767  e automatic logg
-00005b10: 696e 6720 6f66 2074 7261 696e 696e 6720  ing of training 
-00005b20: 6d65 7472 6963 7320 6279 2053 7761 6e4c  metrics by SwanL
-00005b30: 6162 2e0a 0a41 6464 2074 6865 2066 6f6c  ab...Add the fol
-00005b40: 6c6f 7769 6e67 2063 6f64 6520 736e 6970  lowing code snip
-00005b50: 7065 7420 746f 2079 6f75 7220 4d4d 2063  pet to your MM c
-00005b60: 6f6e 6669 6720 6669 6c65 2074 6f20 7374  onfig file to st
-00005b70: 6172 7420 7472 6169 6e69 6e67 3a0a 0a60  art training:..`
-00005b80: 6060 7079 7468 6f6e 0a63 7573 746f 6d5f  ``python.custom_
-00005b90: 696d 706f 7274 7320 3d20 6469 6374 2869  imports = dict(i
-00005ba0: 6d70 6f72 7473 3d5b 2273 7761 6e6c 6162  mports=["swanlab
-00005bb0: 2e69 6e74 6567 7261 7469 6f6e 2e6d 6d65  .integration.mme
-00005bc0: 6e67 696e 6522 5d2c 2061 6c6c 6f77 5f66  ngine"], allow_f
-00005bd0: 6169 6c65 645f 696d 706f 7274 733d 4661  ailed_imports=Fa
-00005be0: 6c73 6529 0a0a 7669 735f 6261 636b 656e  lse)..vis_backen
-00005bf0: 6473 203d 205b 0a20 2020 2064 6963 7428  ds = [.    dict(
-00005c00: 0a20 2020 2020 2020 2074 7970 653d 2253  .        type="S
-00005c10: 7761 6e6c 6162 5669 7342 6163 6b65 6e64  wanlabVisBackend
-00005c20: 222c 0a20 2020 2020 2020 2073 6176 655f  ",.        save_
-00005c30: 6469 723d 2272 756e 732f 7377 616e 6c61  dir="runs/swanla
-00005c40: 6222 2c0a 2020 2020 2020 2020 696e 6974  b",.        init
-00005c50: 5f6b 7761 7267 733d 7b0a 2020 2020 2020  _kwargs={.      
-00005c60: 2020 2020 2020 2270 726f 6a65 6374 223a        "project":
-00005c70: 2022 7377 616e 6c61 622d 6d6d 656e 6769   "swanlab-mmengi
-00005c80: 6e65 222c 0a20 2020 2020 2020 207d 2c0a  ne",.        },.
-00005c90: 2020 2020 292c 0a5d 0a0a 7669 7375 616c      ),.]..visual
-00005ca0: 697a 6572 203d 2064 6963 7428 0a20 2020  izer = dict(.   
-00005cb0: 2074 7970 653d 2256 6973 7561 6c69 7a65   type="Visualize
-00005cc0: 7222 2c0a 2020 2020 7669 735f 6261 636b  r",.    vis_back
-00005cd0: 656e 6473 3d76 6973 5f62 6163 6b65 6e64  ends=vis_backend
-00005ce0: 732c 0a29 0a60 6060 0a3c 2f64 6574 6169  s,.).```.</detai
-00005cf0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a3c  ls>..<details>.<
-00005d00: 7375 6d6d 6172 793e 0a20 203c 7374 726f  summary>.  <stro
-00005d10: 6e67 3e20 556c 7472 616c 7974 6963 733c  ng> Ultralytics<
-00005d20: 2f73 7472 6f6e 673e 0a3c 2f73 756d 6d61  /strong>.</summa
-00005d30: 7279 3e0a 3c62 723e 0a0a 496e 7465 6772  ry>.<br>..Integr
-00005d40: 6174 696e 6720 5377 616e 4c61 6220 696e  ating SwanLab in
-00005d50: 746f 2055 6c74 7261 6c79 7469 6373 2069  to Ultralytics i
-00005d60: 7320 7665 7279 2073 696d 706c 653b 2079  s very simple; y
-00005d70: 6f75 2063 616e 2075 7365 2074 6865 2060  ou can use the `
-00005d80: 6164 645f 7377 616e 6c61 625f 6361 6c6c  add_swanlab_call
-00005d90: 6261 636b 6020 6675 6e63 7469 6f6e 3a0a  back` function:.
-00005da0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00005db0: 756c 7472 616c 7974 6963 7320 696d 706f  ultralytics impo
-00005dc0: 7274 2059 4f4c 4f0a 6672 6f6d 2073 7761  rt YOLO.from swa
-00005dd0: 6e6c 6162 2e69 6e74 6567 7261 7469 6f6e  nlab.integration
-00005de0: 2e75 6c74 7261 6c79 7469 6373 2069 6d70  .ultralytics imp
-00005df0: 6f72 7420 6164 645f 7377 616e 6c61 625f  ort add_swanlab_
-00005e00: 6361 6c6c 6261 636b 0a0a 6d6f 6465 6c20  callback..model 
-00005e10: 3d20 594f 4c4f 2822 796f 6c6f 7638 6e2e  = YOLO("yolov8n.
-00005e20: 7961 6d6c 2229 0a6d 6f64 656c 2e6c 6f61  yaml").model.loa
-00005e30: 6428 290a 0a61 6464 5f73 7761 6e6c 6162  d()..add_swanlab
-00005e40: 5f63 616c 6c62 6163 6b28 6d6f 6465 6c29  _callback(model)
-00005e50: 0a0a 6d6f 6465 6c2e 7472 6169 6e28 0a20  ..model.train(. 
-00005e60: 2020 2064 6174 613d 222e 2f63 6f63 6f2e     data="./coco.
-00005e70: 7961 6d6c 222c 0a20 2020 2065 706f 6368  yaml",.    epoch
-00005e80: 733d 3530 2c20 0a20 2020 2069 6d67 737a  s=50, .    imgsz
-00005e90: 3d33 3230 2c0a 290a 6060 600a 0a3c 2f64  =320,.).```..</d
-00005ea0: 6574 6169 6c73 3e0a 0a0a 0a3c 6272 3e0a  etails>....<br>.
-00005eb0: 0a23 2320 f09f 869a 2043 6f6d 7061 7269  .## .... Compari
-00005ec0: 736f 6e20 7769 7468 2066 616d 696c 6961  son with familia
-00005ed0: 7220 746f 6f6c 730a 0a23 2323 2054 656e  r tools..### Ten
-00005ee0: 736f 7262 6f61 7264 2076 7320 5377 616e  sorboard vs Swan
-00005ef0: 4c61 620a 0a2d 202a 2ae2 9881 efb8 8f20  Lab..- **...... 
-00005f00: 4f6e 6c69 6e65 2055 7361 6765 2053 7570  Online Usage Sup
-00005f10: 706f 7274 2a2a 3a0a 2020 5769 7468 2053  port**:.  With S
-00005f20: 7761 6e4c 6162 2c20 7472 6169 6e69 6e67  wanLab, training
-00005f30: 2065 7870 6572 696d 656e 7473 2063 616e   experiments can
-00005f40: 2062 6520 636f 6e76 656e 6965 6e74 6c79   be conveniently
-00005f50: 2073 796e 6368 726f 6e69 7a65 6420 616e   synchronized an
-00005f60: 6420 7361 7665 6420 696e 2074 6865 2063  d saved in the c
-00005f70: 6c6f 7564 2c20 616c 6c6f 7769 6e67 2066  loud, allowing f
-00005f80: 6f72 2072 656d 6f74 650a 2020 6d6f 6e69  or remote.  moni
-00005f90: 746f 7269 6e67 206f 6620 7472 6169 6e69  toring of traini
-00005fa0: 6e67 2070 726f 6772 6573 732c 206d 616e  ng progress, man
-00005fb0: 6167 696e 6720 6869 7374 6f72 6963 616c  aging historical
-00005fc0: 2070 726f 6a65 6374 732c 2073 6861 7269   projects, shari
-00005fd0: 6e67 2065 7870 6572 696d 656e 7420 6c69  ng experiment li
-00005fe0: 6e6b 732c 2073 656e 6469 6e67 2072 6561  nks, sending rea
-00005ff0: 6c2d 7469 6d65 0a20 206e 6f74 6966 6963  l-time.  notific
-00006000: 6174 696f 6e20 6d65 7373 6167 6573 2c20  ation messages, 
-00006010: 616e 6420 7669 6577 696e 6720 6578 7065  and viewing expe
-00006020: 7269 6d65 6e74 7320 6163 726f 7373 206d  riments across m
-00006030: 756c 7469 706c 6520 6465 7669 6365 732e  ultiple devices.
-00006040: 2049 6e20 636f 6e74 7261 7374 2c20 5465   In contrast, Te
-00006050: 6e73 6f72 426f 6172 6420 6973 2061 6e20  nsorBoard is an 
-00006060: 6f66 666c 696e 650a 2020 6578 7065 7269  offline.  experi
-00006070: 6d65 6e74 2074 7261 636b 696e 6720 746f  ment tracking to
-00006080: 6f6c 2e0a 0a2d 202a 2af0 9f91 a520 436f  ol...- **.... Co
-00006090: 6c6c 6162 6f72 6174 6976 6520 4d75 6c74  llaborative Mult
-000060a0: 692d 7573 6572 2045 6e76 6972 6f6e 6d65  i-user Environme
-000060b0: 6e74 2a2a 3a0a 2020 5377 616e 4c61 6220  nt**:.  SwanLab 
-000060c0: 6661 6369 6c69 7461 7465 7320 6561 7379  facilitates easy
-000060d0: 206d 616e 6167 656d 656e 7420 6f66 206d   management of m
-000060e0: 756c 7469 2d70 6572 736f 6e20 7472 6169  ulti-person trai
-000060f0: 6e69 6e67 2070 726f 6a65 6374 7320 616e  ning projects an
-00006100: 6420 7368 6172 696e 6720 6f66 2065 7870  d sharing of exp
-00006110: 6572 696d 656e 7420 6c69 6e6b 7320 666f  eriment links fo
-00006120: 720a 2020 636f 6c6c 6162 6f72 6174 6976  r.  collaborativ
-00006130: 6520 6d61 6368 696e 6520 6c65 6172 6e69  e machine learni
-00006140: 6e67 2061 6372 6f73 7320 7465 616d 732e  ng across teams.
-00006150: 2049 7420 616c 736f 2065 6e61 626c 6573   It also enables
-00006160: 2063 726f 7373 2d73 7061 6365 2063 6f6d   cross-space com
-00006170: 6d75 6e69 6361 7469 6f6e 2061 6e64 2064  munication and d
-00006180: 6973 6375 7373 696f 6e2e 204f 6e20 7468  iscussion. On th
-00006190: 6520 6f74 6865 720a 2020 6861 6e64 2c20  e other.  hand, 
-000061a0: 5465 6e73 6f72 426f 6172 6420 6973 2070  TensorBoard is p
-000061b0: 7269 6d61 7269 6c79 2064 6573 6967 6e65  rimarily designe
-000061c0: 6420 666f 7220 696e 6469 7669 6475 616c  d for individual
-000061d0: 2075 7365 2c20 6d61 6b69 6e67 2069 7420   use, making it 
-000061e0: 6469 6666 6963 756c 7420 746f 2063 6f6c  difficult to col
-000061f0: 6c61 626f 7261 7465 2061 6e64 2073 6861  laborate and sha
-00006200: 7265 2065 7870 6572 696d 656e 7473 0a20  re experiments. 
-00006210: 2077 6974 6820 6d75 6c74 6970 6c65 2075   with multiple u
-00006220: 7365 7273 2e0a 0a2d 202a 2af0 9f92 bb20  sers...- **.... 
-00006230: 5065 7273 6973 7465 6e74 2c20 4365 6e74  Persistent, Cent
-00006240: 7261 6c69 7a65 6420 4461 7368 626f 6172  ralized Dashboar
-00006250: 642a 2a3a 0a20 2052 6567 6172 646c 6573  d**:.  Regardles
-00006260: 7320 6f66 2077 6865 7265 2079 6f75 2061  s of where you a
-00006270: 7265 2074 7261 696e 696e 6720 796f 7572  re training your
-00006280: 206d 6f64 656c 732c 2062 6520 6974 206f   models, be it o
-00006290: 6e20 6120 6c6f 6361 6c20 636f 6d70 7574  n a local comput
-000062a0: 6572 2c20 6120 6c61 6220 636c 7573 7465  er, a lab cluste
-000062b0: 722c 206f 7220 6f6e 2070 7562 6c69 6320  r, or on public 
-000062c0: 636c 6f75 6420 4750 550a 2020 696e 7374  cloud GPU.  inst
-000062d0: 616e 6365 732c 2079 6f75 7220 7265 7375  ances, your resu
-000062e0: 6c74 7320 6172 6520 6c6f 6767 6564 2074  lts are logged t
-000062f0: 6f20 7468 6520 7361 6d65 2063 656e 7472  o the same centr
-00006300: 616c 697a 6564 2064 6173 6862 6f61 7264  alized dashboard
-00006310: 2e20 5573 696e 6720 5465 6e73 6f72 426f  . Using TensorBo
-00006320: 6172 642c 206f 6e20 7468 6520 6f74 6865  ard, on the othe
-00006330: 7220 6861 6e64 2c20 7265 7175 6972 6573  r hand, requires
-00006340: 0a20 2073 7065 6e64 696e 6720 7469 6d65  .  spending time
-00006350: 2063 6f70 7969 6e67 2061 6e64 206d 616e   copying and man
-00006360: 6167 696e 6720 5446 4576 656e 7420 6669  aging TFEvent fi
-00006370: 6c65 7320 6672 6f6d 2064 6966 6665 7265  les from differe
-00006380: 6e74 206d 6163 6869 6e65 732e 0a0a 2d20  nt machines...- 
-00006390: 2a2a f09f 92aa 204d 6f72 6520 506f 7765  **.... More Powe
-000063a0: 7266 756c 2054 6162 6c65 732a 2a3a 0a20  rful Tables**:. 
-000063b0: 2053 7761 6e4c 6162 2074 6162 6c65 7320   SwanLab tables 
-000063c0: 616c 6c6f 7720 796f 7520 746f 2076 6965  allow you to vie
-000063d0: 772c 2073 6561 7263 682c 2061 6e64 2066  w, search, and f
-000063e0: 696c 7465 7220 7265 7375 6c74 7320 6672  ilter results fr
-000063f0: 6f6d 2076 6172 696f 7573 2065 7870 6572  om various exper
-00006400: 696d 656e 7473 2c20 6d61 6b69 6e67 2069  iments, making i
-00006410: 7420 6561 7379 2074 6f20 7265 7669 6577  t easy to review
-00006420: 0a20 2074 686f 7573 616e 6473 206f 6620  .  thousands of 
-00006430: 6d6f 6465 6c20 7665 7273 696f 6e73 2074  model versions t
-00006440: 6f20 6669 6e64 2074 6865 2062 6573 742d  o find the best-
-00006450: 7065 7266 6f72 6d69 6e67 206d 6f64 656c  performing model
-00006460: 7320 666f 7220 6469 6666 6572 656e 7420  s for different 
-00006470: 7461 736b 732e 2054 656e 736f 7242 6f61  tasks. TensorBoa
-00006480: 7264 2069 7320 6e6f 7420 7765 6c6c 2d73  rd is not well-s
-00006490: 7569 7465 6420 666f 720a 2020 6c61 7267  uited for.  larg
-000064a0: 652d 7363 616c 6520 7072 6f6a 6563 7473  e-scale projects
-000064b0: 2e0a 0a23 2323 2057 6569 6768 7473 2061  ...### Weights a
-000064c0: 6e64 2042 6961 7365 7320 7673 2053 7761  nd Biases vs Swa
-000064d0: 6e4c 6162 0a0a 2d20 5765 6967 6874 7320  nLab..- Weights 
-000064e0: 616e 6420 4269 6173 6573 2069 7320 616e  and Biases is an
-000064f0: 206f 6e6c 696e 652d 6f6e 6c79 2c20 7072   online-only, pr
-00006500: 6f70 7269 6574 6172 7920 4d4c 4f70 7320  oprietary MLOps 
-00006510: 706c 6174 666f 726d 2e0a 0a2d 204e 6f74  platform...- Not
-00006520: 206f 6e6c 7920 646f 6573 2053 7761 6e4c   only does SwanL
-00006530: 6162 2073 7570 706f 7274 206f 6e6c 696e  ab support onlin
-00006540: 6520 7573 6167 652c 2062 7574 2069 7420  e usage, but it 
-00006550: 616c 736f 206f 6666 6572 7320 616e 206f  also offers an o
-00006560: 7065 6e2d 736f 7572 6365 2c20 6672 6565  pen-source, free
-00006570: 2c20 616e 6420 7365 6c66 2d68 6f73 7465  , and self-hoste
-00006580: 6420 7665 7273 696f 6e2e 0a0a 3c62 723e  d version...<br>
-00006590: 0a0a 2323 20f0 9f9b a3ef b88f 2052 6f61  ..## ....... Roa
-000065a0: 646d 6170 0a0a 546f 6f6c 7320 6576 6f6c  dmap..Tools evol
-000065b0: 7665 2069 6e20 6974 6572 6174 696f 6e20  ve in iteration 
-000065c0: 616e 6420 6665 6564 6261 636b 7e2c 2077  and feedback~, w
-000065d0: 656c 636f 6d65 0a74 6f20 5b73 7562 6d69  elcome.to [submi
-000065e0: 7420 6665 6174 7572 6520 7375 6767 6573  t feature sugges
-000065f0: 7469 6f6e 735d 2868 7474 7073 3a2f 2f67  tions](https://g
-00006600: 6565 6b74 6563 6873 7475 6469 6f2e 6665  eektechstudio.fe
-00006610: 6973 6875 2e63 6e2f 7368 6172 652f 6261  ishu.cn/share/ba
-00006620: 7365 2f66 6f72 6d2f 7368 7263 6e79 426c  se/form/shrcnyBl
-00006630: 4b38 4f4d 4430 6577 656f 4663 6332 5376  K8OMD0eweoFcc2Sv
-00006640: 574b 6329 0a0a 2323 2320 496e 2050 726f  WKc)..### In Pro
-00006650: 6772 6573 7320 4e6f 770a 0a2d 2060 5461  gress Now..- `Ta
-00006660: 626c 6560 3a20 4d6f 7265 2066 6c65 7869  ble`: More flexi
-00006670: 626c 6520 6d75 6c74 6964 696d 656e 7369  ble multidimensi
-00006680: 6f6e 616c 2074 6162 6c65 2063 6861 7274  onal table chart
-00006690: 732c 2073 7569 7461 626c 6520 666f 7220  s, suitable for 
-000066a0: 4c4c 4d2c 2041 4947 432c 206d 6f64 656c  LLM, AIGC, model
-000066b0: 2065 7661 6c75 6174 696f 6e20 616e 6420   evaluation and 
-000066c0: 6f74 6865 7220 7363 656e 6172 696f 732e  other scenarios.
-000066d0: 0a0a 2d20 2a2a 456d 6169 6c20 6e6f 7469  ..- **Email noti
-000066e0: 6669 6361 7469 6f6e f09f 93a7 2a2a 3a20  fication....**: 
-000066f0: 5768 656e 2074 7261 696e 696e 6720 6973  When training is
-00006700: 2069 6e74 6572 7275 7074 6564 2075 6e65   interrupted une
-00006710: 7870 6563 7465 646c 792c 2077 6865 6e20  xpectedly, when 
-00006720: 7472 6169 6e69 6e67 2069 7320 636f 6d70  training is comp
-00006730: 6c65 7465 642c 2061 6e64 2077 6865 6e20  leted, and when 
-00006740: 6375 7374 6f6d 0a20 2073 6974 7561 7469  custom.  situati
-00006750: 6f6e 7320 6f63 6375 722c 2073 656e 6420  ons occur, send 
-00006760: 6e6f 7469 6669 6361 7469 6f6e 2065 6d61  notification ema
-00006770: 696c 732e 0a0a 2323 2320 4e65 7874 2050  ils...### Next P
-00006780: 6c61 6e6e 6564 0a0a 2d20 604d 6f6c 6563  lanned..- `Molec
-00006790: 756c 6560 3a20 5669 7375 616c 697a 6174  ule`: Visualizat
-000067a0: 696f 6e20 6368 6172 7473 206f 6620 6269  ion charts of bi
-000067b0: 6f63 6865 6d69 7374 7279 206d 6f6c 6563  ochemistry molec
-000067c0: 756c 6573 0a0a 2d20 6050 6c6f 7460 3a20  ules..- `Plot`: 
-000067d0: 4672 6565 2063 6861 7274 2064 7261 7769  Free chart drawi
-000067e0: 6e67 206d 6574 686f 640a 0a2d 2060 4170  ng method..- `Ap
-000067f0: 6960 3a20 4163 6365 7373 2053 7761 6e4c  i`: Access SwanL
-00006800: 6162 2064 6174 6120 7468 726f 7567 6820  ab data through 
-00006810: 4150 492e 0a0a 2d20 2a2a 5379 7374 656d  API...- **System
-00006820: 2068 6172 6477 6172 6520 7265 636f 7264   hardware record
-00006830: 732a 2a3a 2052 6563 6f72 6420 6120 7365  s**: Record a se
-00006840: 7269 6573 206f 6620 6861 7264 7761 7265  ries of hardware
-00006850: 2063 6f6e 6469 7469 6f6e 7320 7375 6368   conditions such
-00006860: 2061 7320 4750 552c 2043 5055 2c20 6469   as GPU, CPU, di
-00006870: 736b 2c20 6e65 7477 6f72 6b2c 2065 7463  sk, network, etc
-00006880: 2e0a 0a2d 202a 2a43 6f64 6520 7265 636f  ...- **Code reco
-00006890: 7264 732a 2a3a 2052 6563 6f72 6420 7472  rds**: Record tr
-000068a0: 6169 6e69 6e67 2063 6f64 650a 0a2d 202a  aining code..- *
-000068b0: 2a4d 6f72 6520 696e 7465 6772 6174 696f  *More integratio
-000068c0: 6e73 2a2a 3a20 4c69 6768 7447 424d 2c20  ns**: LightGBM, 
-000068d0: 5847 426f 6f73 742c 206f 7065 6e61 692c  XGBoost, openai,
-000068e0: 2063 6861 7467 6c6d 2c20 6d6d 2073 6572   chatglm, mm ser
-000068f0: 6965 732c 2e2e 2e0a 2d20 2e2e 2e0a 0a23  ies,....- .....#
-00006900: 2323 204c 6f6e 672d 7465 726d 2043 6f6e  ## Long-term Con
-00006910: 6365 726e 0a0a 2d20 5468 6520 6d6f 7374  cern..- The most
-00006920: 2062 656e 6566 6963 6961 6c20 636f 6c6c   beneficial coll
-00006930: 6162 6f72 6174 6976 6520 7761 7920 666f  aborative way fo
-00006940: 7220 4149 2074 6561 6d20 696e 6e6f 7661  r AI team innova
-00006950: 7469 6f6e 0a0a 2d20 5468 6520 6d6f 7374  tion..- The most
-00006960: 2075 7365 722d 6672 6965 6e64 6c79 2055   user-friendly U
-00006970: 4920 696e 7465 7261 6374 696f 6e0a 0a2d  I interaction..-
-00006980: 2056 6965 7769 6e67 2065 7870 6572 696d   Viewing experim
-00006990: 656e 7473 206f 6e20 6d6f 6269 6c65 0a0a  ents on mobile..
-000069a0: 3c62 723e 0a0a 2323 20f0 9f91 a520 436f  <br>..## .... Co
-000069b0: 6d6d 756e 6974 790a 0a23 2323 2043 6f6d  mmunity..### Com
-000069c0: 6d75 6e69 7479 2061 6e64 2073 7570 706f  munity and suppo
-000069d0: 7274 0a0a 2d20 5b47 6974 4875 6220 4973  rt..- [GitHub Is
-000069e0: 7375 6573 5d28 6874 7470 733a 2f2f 6769  sues](https://gi
-000069f0: 7468 7562 2e63 6f6d 2f53 7761 6e48 7562  thub.com/SwanHub
-00006a00: 582f 5377 616e 4c61 622f 6973 7375 6573  X/SwanLab/issues
-00006a10: 29ef bc9a 4572 726f 7273 2061 6e64 2069  )...Errors and i
-00006a20: 7373 7565 7320 656e 636f 756e 7465 7265  ssues encountere
-00006a30: 6420 7768 656e 2075 7369 6e67 2053 7761  d when using Swa
-00006a40: 6e4c 6162 0a2d 205b 456d 6169 6c20 7375  nLab.- [Email su
-00006a50: 7070 6f72 745d 287a 6579 692e 6c69 6e40  pport](zeyi.lin@
-00006a60: 7377 616e 6875 622e 636f 29ef bc9a 4665  swanhub.co)...Fe
-00006a70: 6564 6261 636b 206f 6e20 6973 7375 6573  edback on issues
-00006a80: 2077 6974 6820 7573 696e 6720 5377 616e   with using Swan
-00006a90: 4c61 620a 2d20 3c61 2068 7265 663d 2268  Lab.- <a href="h
-00006aa0: 7474 7073 3a2f 2f67 6565 6b74 6563 6873  ttps://geektechs
-00006ab0: 7475 6469 6f2e 6665 6973 6875 2e63 6e2f  tudio.feishu.cn/
-00006ac0: 7769 6b69 2f4e 495a 3977 7035 4c52 6953  wiki/NIZ9wp5LRiS
-00006ad0: 7151 796b 697a 6247 6356 7a55 4b6e 6963  qQykizbGcVzUKnic
-00006ae0: 223e 5765 4368 6174 3c2f 613e efbc 9a44  ">WeChat</a>...D
-00006af0: 6973 6375 7373 2069 7373 7565 7320 7573  iscuss issues us
-00006b00: 696e 6720 5377 616e 4c61 622c 0a20 2073  ing SwanLab,.  s
-00006b10: 6861 7265 2074 6865 206c 6174 6573 7420  hare the latest 
-00006b20: 4149 2074 6563 686e 6f6c 6f67 792e 0a0a  AI technology...
-00006b30: 2323 2320 5377 616e 4c61 6220 5245 4144  ### SwanLab READ
-00006b40: 4d45 2042 6164 6765 0a0a 4966 2079 6f75  ME Badge..If you
-00006b50: 206c 696b 6520 746f 2075 7365 2053 7761   like to use Swa
-00006b60: 6e4c 6162 2069 6e20 796f 7572 2077 6f72  nLab in your wor
-00006b70: 6b2c 2070 6c65 6173 6520 6164 6420 7468  k, please add th
-00006b80: 6520 5377 616e 4c61 6220 6261 6467 6520  e SwanLab badge 
-00006b90: 746f 2079 6f75 7220 5245 4144 4d45 3a0a  to your README:.
-00006ba0: 0a5b 215b 7377 616e 6c61 625d 2868 7474  .[![swanlab](htt
-00006bb0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00006bc0: 2e69 6f2f 6261 6467 652f 706f 7765 7265  .io/badge/powere
-00006bd0: 6425 3230 6279 2d53 7761 6e4c 6162 2d34  d%20by-SwanLab-4
-00006be0: 3338 3434 3029 5d28 6874 7470 733a 2f2f  38440)](https://
-00006bf0: 6769 7468 7562 2e63 6f6d 2f73 7761 6e68  github.com/swanh
-00006c00: 7562 782f 7377 616e 6c61 6229 0a0a 6060  ubx/swanlab)..``
-00006c10: 600a 5b21 5b73 7761 6e6c 6162 5d28 6874  `.[![swanlab](ht
-00006c20: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00006c30: 732e 696f 2f62 6164 6765 2f70 6f77 6572  s.io/badge/power
-00006c40: 6564 2532 3062 792d 5377 616e 4c61 622d  ed%20by-SwanLab-
-00006c50: 3433 3834 3430 295d 2868 7474 7073 3a2f  438440)](https:/
-00006c60: 2f67 6974 6875 622e 636f 6d2f 7377 616e  /github.com/swan
-00006c70: 6875 6278 2f73 7761 6e6c 6162 290a 6060  hubx/swanlab).``
-00006c80: 600a 0a23 2323 2043 6974 696e 6720 5377  `..### Citing Sw
-00006c90: 616e 4c61 6220 696e 2074 6865 2070 6170  anLab in the pap
-00006ca0: 6572 0a0a 4966 2079 6f75 2066 696e 6420  er..If you find 
-00006cb0: 5377 616e 4c61 6220 6865 6c70 6675 6c20  SwanLab helpful 
-00006cc0: 666f 7220 796f 7572 2072 6573 6561 7263  for your researc
-00006cd0: 6820 6a6f 7572 6e65 792c 2070 6c65 6173  h journey, pleas
-00006ce0: 6520 636f 6e73 6964 6572 2063 6974 696e  e consider citin
-00006cf0: 6720 696e 2074 6865 2066 6f6c 6c6f 7769  g in the followi
-00006d00: 6e67 2066 6f72 6d61 743a 0a0a 6060 6062  ng format:..```b
-00006d10: 6962 7465 780a 4073 6f66 7477 6172 657b  ibtex.@software{
-00006d20: 5a65 7969 6c69 6e5f 5377 616e 4c61 625f  Zeyilin_SwanLab_
-00006d30: 3230 3233 2c0a 2020 6175 7468 6f72 203d  2023,.  author =
-00006d40: 207b 5a65 7969 204c 696e 2c20 5368 616f   {Zeyi Lin, Shao
-00006d50: 686f 6e67 2043 6865 6e2c 204b 616e 6720  hong Chen, Kang 
-00006d60: 4c69 2c20 5169 7573 6861 6e20 4a69 616e  Li, Qiushan Jian
-00006d70: 672c 205a 6972 7569 2043 6169 2c20 204b  g, Zirui Cai,  K
-00006d80: 6169 6661 6e67 204a 6920 616e 6420 7b54  aifang Ji and {T
-00006d90: 6865 2053 7761 6e4c 6162 2074 6561 6d7d  he SwanLab team}
-00006da0: 7d2c 0a20 2064 6f69 203d 207b 3130 2e35  },.  doi = {10.5
-00006db0: 3238 312f 7a65 6e6f 646f 2e31 3131 3030  281/zenodo.11100
-00006dc0: 3535 307d 2c0a 2020 6c69 6365 6e73 6520  550},.  license 
-00006dd0: 3d20 7b41 7061 6368 652d 322e 307d 2c0a  = {Apache-2.0},.
-00006de0: 2020 7469 746c 6520 3d20 7b7b 5377 616e    title = {{Swan
-00006df0: 4c61 627d 7d2c 0a20 2075 726c 203d 207b  Lab}},.  url = {
-00006e00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00006e10: 6f6d 2f73 7761 6e68 7562 782f 7377 616e  om/swanhubx/swan
-00006e20: 6c61 627d 2c0a 2020 7965 6172 203d 207b  lab},.  year = {
-00006e30: 3230 3233 7d0a 7d0a 6060 600a 0a23 2323  2023}.}.```..###
-00006e40: 2043 6f6e 7472 6962 7574 6520 746f 2053   Contribute to S
-00006e50: 7761 6e4c 6162 0a0a 436f 6e73 6964 6572  wanLab..Consider
-00006e60: 696e 6720 636f 6e74 7269 6275 7469 6e67  ing contributing
-00006e70: 2074 6f20 5377 616e 4c61 623f 2046 6972   to SwanLab? Fir
-00006e80: 7374 2c20 706c 6561 7365 2074 616b 6520  st, please take 
-00006e90: 736f 6d65 2074 696d 6520 746f 2072 6561  some time to rea
-00006ea0: 640a 7468 6520 5b43 6f6e 7472 6962 7574  d.the [Contribut
-00006eb0: 696f 6e20 4775 6964 656c 696e 6573 5d28  ion Guidelines](
-00006ec0: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
-00006ed0: 2e0a 0a41 7420 7468 6520 7361 6d65 2074  ...At the same t
-00006ee0: 696d 652c 2077 6520 7761 726d 6c79 2077  ime, we warmly w
-00006ef0: 656c 636f 6d65 2073 7570 706f 7274 2066  elcome support f
-00006f00: 6f72 2053 7761 6e4c 6162 2074 6872 6f75  or SwanLab throu
-00006f10: 6768 2073 6f63 6961 6c20 6d65 6469 612c  gh social media,
-00006f20: 2065 7665 6e74 732c 2061 6e64 2063 6f6e   events, and con
-00006f30: 6665 7265 6e63 6520 7368 6172 696e 672e  ference sharing.
-00006f40: 2054 6861 6e6b 2079 6f75 210a 0a3c 6272   Thank you!..<br
-00006f50: 3e0a 0a2a 2a43 6f6e 7472 6962 7574 6f72  >..**Contributor
-00006f60: 732a 2a0a 0a3c 6120 6872 6566 3d22 6874  s**..<a href="ht
-00006f70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006f80: 2f73 7761 6e68 7562 782f 7377 616e 6c61  /swanhubx/swanla
-00006f90: 622f 6772 6170 6873 2f63 6f6e 7472 6962  b/graphs/contrib
-00006fa0: 7574 6f72 7322 3e0a 2020 3c69 6d67 2073  utors">.  <img s
-00006fb0: 7263 3d22 6874 7470 733a 2f2f 636f 6e74  rc="https://cont
-00006fc0: 7269 622e 726f 636b 732f 696d 6167 653f  rib.rocks/image?
-00006fd0: 7265 706f 3d73 7761 6e68 7562 782f 7377  repo=swanhubx/sw
-00006fe0: 616e 6c61 6222 202f 3e0a 3c2f 613e 0a0a  anlab" />.</a>..
-00006ff0: 2323 2320 446f 776e 6c6f 6164 2049 636f  ### Download Ico
-00007000: 6e0a 0a5b 5377 616e 4c61 622d 4963 6f6e  n..[SwanLab-Icon
-00007010: 2d53 5647 5d28 7265 6164 6d65 5f66 696c  -SVG](readme_fil
-00007020: 6573 2f73 7761 6e6c 6162 2d6c 6f67 6f2e  es/swanlab-logo.
-00007030: 7376 6729 0a0a 3c62 723e 0a0a 2323 20f0  svg)..<br>..## .
-00007040: 9f93 8320 4c69 6365 6e73 650a 0a54 6869  ... License..Thi
-00007050: 7320 7265 706f 7369 746f 7279 2066 6f6c  s repository fol
-00007060: 6c6f 7773 2074 6865 205b 4170 6163 6865  lows the [Apache
-00007070: 2032 2e30 204c 6963 656e 7365 5d28 6874   2.0 License](ht
-00007080: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00007090: 2f53 7761 6e48 7562 582f 5377 616e 4c61  /SwanHubX/SwanLa
-000070a0: 622f 626c 6f62 2f6d 6169 6e2f 4c49 4345  b/blob/main/LICE
-000070b0: 4e53 4529 206f 7065 6e20 736f 7572 6365  NSE) open source
-000070c0: 0a6c 6963 656e 7365 2e0a                 .license..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 330a 4e61 6d65 3a20 7377 616e  : 2.3.Name: swan
+00000020: 6c61 620a 5665 7273 696f 6e3a 2030 2e33  lab.Version: 0.3
+00000030: 2e37 0a53 756d 6d61 7279 3a20 5079 7468  .7.Summary: Pyth
+00000040: 6f6e 206c 6962 7261 7279 2066 6f72 2073  on library for s
+00000050: 7472 6561 6d6c 696e 6564 2074 7261 636b  treamlined track
+00000060: 696e 6720 616e 6420 6d61 6e61 6765 6d65  ing and manageme
+00000070: 6e74 206f 6620 4149 2074 7261 696e 696e  nt of AI trainin
+00000080: 6720 7072 6f63 6573 7365 732e 0a50 726f  g processes..Pro
+00000090: 6a65 6374 2d55 524c 3a20 486f 6d65 7061  ject-URL: Homepa
+000000a0: 6765 2c20 6874 7470 733a 2f2f 7377 616e  ge, https://swan
+000000b0: 6875 622e 636f 0a50 726f 6a65 6374 2d55  hub.co.Project-U
+000000c0: 524c 3a20 536f 7572 6365 2c20 6874 7470  RL: Source, http
+000000d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+000000e0: 7761 6e48 7562 582f 5377 616e 4c61 620a  wanHubX/SwanLab.
+000000f0: 5072 6f6a 6563 742d 5552 4c3a 2042 7567  Project-URL: Bug
+00000100: 2052 6570 6f72 7473 2c20 6874 7470 733a   Reports, https:
+00000110: 2f2f 6769 7468 7562 2e63 6f6d 2f53 7761  //github.com/Swa
+00000120: 6e48 7562 582f 5377 616e 4c61 622f 6973  nHubX/SwanLab/is
+00000130: 7375 6573 0a50 726f 6a65 6374 2d55 524c  sues.Project-URL
+00000140: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
+00000150: 2068 7474 7073 3a2f 2f67 6565 6b74 6563   https://geektec
+00000160: 6873 7475 6469 6f2e 6665 6973 6875 2e63  hstudio.feishu.c
+00000170: 6e2f 7769 6b69 2f73 7061 6365 2f37 3331  n/wiki/space/731
+00000180: 3035 3933 3332 3533 3734 3031 3334 3434  0593325374013444
+00000190: 3f63 636d 5f6f 7065 6e5f 7479 7065 3d6c  ?ccm_open_type=l
+000001a0: 6172 6b5f 7769 6b69 5f73 7061 6365 4c69  ark_wiki_spaceLi
+000001b0: 6e6b 266f 7065 6e5f 7461 625f 6672 6f6d  nk&open_tab_from
+000001c0: 3d77 696b 695f 686f 6d65 0a41 7574 686f  =wiki_home.Autho
+000001d0: 722d 656d 6169 6c3a 2043 756e 7975 6520  r-email: Cunyue 
+000001e0: 3c74 6561 6d40 7377 616e 6875 622e 636f  <team@swanhub.co
+000001f0: 3e2c 2046 6575 6461 6c6d 616e 203c 7465  >, Feudalman <te
+00000200: 616d 4073 7761 6e68 7562 2e63 6f3e 2c20  am@swanhub.co>, 
+00000210: 5a65 5969 204c 696e 203c 7465 616d 4073  ZeYi Lin <team@s
+00000220: 7761 6e68 7562 2e63 6f3e 2c20 4b61 7368  wanhub.co>, Kash
+00000230: 6977 6142 7974 6520 3c74 6561 6d40 7377  iwaByte <team@sw
+00000240: 616e 6875 622e 636f 3e0a 4c69 6365 6e73  anhub.co>.Licens
+00000250: 652d 4578 7072 6573 7369 6f6e 3a20 4170  e-Expression: Ap
+00000260: 6163 6865 2d32 2e30 0a4c 6963 656e 7365  ache-2.0.License
+00000270: 2d46 696c 653a 204c 4943 454e 5345 0a4b  -File: LICENSE.K
+00000280: 6579 776f 7264 733a 206d 6163 6869 6e65  eywords: machine
+00000290: 206c 6561 726e 696e 672c 7265 7072 6f64   learning,reprod
+000002a0: 7563 6962 696c 6974 792c 7669 7375 616c  ucibility,visual
+000002b0: 697a 6174 696f 6e0a 436c 6173 7369 6669  ization.Classifi
+000002c0: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+000002d0: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
+000002e0: 7068 610a 436c 6173 7369 6669 6572 3a20  pha.Classifier: 
+000002f0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000300: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
+00000310: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
+00000320: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
+00000330: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000340: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000350: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+00000360: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000370: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000380: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
+00000390: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000003a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003b0: 3320 3a3a 204f 6e6c 790a 436c 6173 7369  3 :: Only.Classi
+000003c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000003d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003e0: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+000003f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000400: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000410: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+00000420: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000430: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000440: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000450: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000460: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000470: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000480: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+00000490: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000004a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000004b0: 3a20 332e 3132 0a43 6c61 7373 6966 6965  : 3.12.Classifie
+000004c0: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
+000004d0: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
+000004e0: 6e67 0a43 6c61 7373 6966 6965 723a 2054  ng.Classifier: T
+000004f0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+00000500: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
+00000510: 3a20 4172 7469 6669 6369 616c 2049 6e74  : Artificial Int
+00000520: 656c 6c69 6765 6e63 650a 436c 6173 7369  elligence.Classi
+00000530: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000540: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000550: 6572 696e 6720 3a3a 2056 6973 7561 6c69  ering :: Visuali
+00000560: 7a61 7469 6f6e 0a52 6571 7569 7265 732d  zation.Requires-
+00000570: 5079 7468 6f6e 3a20 3e3d 332e 380a 5265  Python: >=3.8.Re
+00000580: 7175 6972 6573 2d44 6973 743a 2063 6c69  quires-Dist: cli
+00000590: 636b 0a52 6571 7569 7265 732d 4469 7374  ck.Requires-Dist
+000005a0: 3a20 636f 732d 7079 7468 6f6e 2d73 646b  : cos-python-sdk
+000005b0: 2d76 350a 5265 7175 6972 6573 2d44 6973  -v5.Requires-Dis
+000005c0: 743a 2066 6173 7461 7069 3e3d 302e 3131  t: fastapi>=0.11
+000005d0: 302e 310a 5265 7175 6972 6573 2d44 6973  0.1.Requires-Dis
+000005e0: 743a 206e 756d 7079 0a52 6571 7569 7265  t: numpy.Require
+000005f0: 732d 4469 7374 3a20 7065 6577 6565 0a52  s-Dist: peewee.R
+00000600: 6571 7569 7265 732d 4469 7374 3a20 7069  equires-Dist: pi
+00000610: 6c6c 6f77 0a52 6571 7569 7265 732d 4469  llow.Requires-Di
+00000620: 7374 3a20 7073 7574 696c 0a52 6571 7569  st: psutil.Requi
+00000630: 7265 732d 4469 7374 3a20 7079 6e76 6d6c  res-Dist: pynvml
+00000640: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000650: 7079 7961 6d6c 0a52 6571 7569 7265 732d  pyyaml.Requires-
+00000660: 4469 7374 3a20 7265 7175 6573 7473 0a52  Dist: requests.R
+00000670: 6571 7569 7265 732d 4469 7374 3a20 736f  equires-Dist: so
+00000680: 756e 6466 696c 650a 5265 7175 6972 6573  undfile.Requires
+00000690: 2d44 6973 743a 2075 6a73 6f6e 0a52 6571  -Dist: ujson.Req
+000006a0: 7569 7265 732d 4469 7374 3a20 7576 6963  uires-Dist: uvic
+000006b0: 6f72 6e3e 3d30 2e31 342e 300a 5265 7175  orn>=0.14.0.Requ
+000006c0: 6972 6573 2d44 6973 743a 2077 6174 6368  ires-Dist: watch
+000006d0: 646f 670a 5072 6f76 6964 6573 2d45 7874  dog.Provides-Ext
+000006e0: 7261 3a20 6f61 7574 680a 4465 7363 7269  ra: oauth.Descri
+000006f0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000700: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000710: 6e0a 0a21 5b4f 7665 7276 6965 775d 2868  n..![Overview](h
+00000720: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000730: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000740: 2f53 7761 6e48 7562 582f 7377 616e 6c61  /SwanHubX/swanla
+00000750: 622f 6d61 696e 2f72 6561 646d 655f 6669  b/main/readme_fi
+00000760: 6c65 732f 7377 616e 6c61 622d 6f76 6572  les/swanlab-over
+00000770: 7669 6577 2d6e 6577 2e70 6e67 290a 0a3c  view-new.png)..<
+00000780: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000790: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
+000007a0: 3a2f 2f73 7761 6e6c 6162 2e63 6e22 3e53  ://swanlab.cn">S
+000007b0: 7761 6e4c 6162 2043 6c6f 7564 3c2f 613e  wanLab Cloud</a>
+000007c0: 20c2 b720 3c61 2068 7265 663d 2268 7474   .. <a href="htt
+000007d0: 7073 3a2f 2f64 6f63 732e 7377 616e 6c61  ps://docs.swanla
+000007e0: 622e 636e 223e 446f 6375 6d65 6e74 3c2f  b.cn">Document</
+000007f0: 613e 20c2 b720 3c61 2068 7265 663d 2268  a> .. <a href="h
+00000800: 7474 7073 3a2f 2f67 6565 6b74 6563 6873  ttps://geektechs
+00000810: 7475 6469 6f2e 6665 6973 6875 2e63 6e2f  tudio.feishu.cn/
+00000820: 7769 6b69 2f4e 495a 3977 7035 4c52 6953  wiki/NIZ9wp5LRiS
+00000830: 7151 796b 697a 6247 6356 7a55 4b6e 6963  qQykizbGcVzUKnic
+00000840: 223e 5765 4368 6174 3c2f 613e 20c2 b720  ">WeChat</a> .. 
+00000850: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000860: 2f67 6974 6875 622e 636f 6d2f 7377 616e  /github.com/swan
+00000870: 6875 6278 2f73 7761 6e6c 6162 2f69 7373  hubx/swanlab/iss
+00000880: 7565 7322 3e52 6570 6f72 7420 4973 7375  ues">Report Issu
+00000890: 653c 2f61 3e20 c2b7 203c 6120 6872 6566  e</a> .. <a href
+000008a0: 3d22 6874 7470 733a 2f2f 6765 656b 7465  ="https://geekte
+000008b0: 6368 7374 7564 696f 2e66 6569 7368 752e  chstudio.feishu.
+000008c0: 636e 2f73 6861 7265 2f62 6173 652f 666f  cn/share/base/fo
+000008d0: 726d 2f73 6872 636e 7942 6c4b 384f 4d44  rm/shrcnyBlK8OMD
+000008e0: 3065 7765 6f46 6363 3253 7657 4b63 223e  0eweoFcc2SvWKc">
+000008f0: 4665 6564 6261 636b 3c2f 613e 20c2 b720  Feedback</a> .. 
+00000900: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000910: 2f67 6974 6875 622e 636f 6d2f 5377 616e  /github.com/Swan
+00000920: 4875 6258 2f53 7761 6e4c 6162 2f62 6c6f  HubX/SwanLab/blo
+00000930: 622f 6d61 696e 2f43 4841 4e47 454c 4f47  b/main/CHANGELOG
+00000940: 2e6d 6422 3e43 6861 6e67 656c 6f67 3c2f  .md">Changelog</
+00000950: 613e 0a0a 0a3c 2f70 3e0a 0a3c 7020 616c  a>...</p>..<p al
+00000960: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000970: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000980: 2f67 6974 6875 622e 636f 6d2f 5377 616e  /github.com/Swan
+00000990: 4875 6258 2f53 7761 6e4c 6162 2f62 6c6f  HubX/SwanLab/blo
+000009a0: 622f 6d61 696e 2f4c 4943 454e 5345 223e  b/main/LICENSE">
+000009b0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000009c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000009d0: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+000009e0: 5377 616e 4875 6258 2f53 7761 6e4c 6162  SwanHubX/SwanLab
+000009f0: 2e73 7667 3f63 6f6c 6f72 3d62 7269 6768  .svg?color=brigh
+00000a00: 7467 7265 656e 2220 616c 743d 226c 6963  tgreen" alt="lic
+00000a10: 656e 7365 223e 3c2f 613e 0a20 203c 6120  ense"></a>.  <a 
+00000a20: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000a30: 7468 7562 2e63 6f6d 2f53 7761 6e48 7562  thub.com/SwanHub
+00000a40: 582f 5377 616e 4c61 622f 636f 6d6d 6974  X/SwanLab/commit
+00000a50: 732f 6d61 696e 223e 3c69 6d67 2073 7263  s/main"><img src
+00000a60: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000a70: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000a80: 6c61 7374 2d63 6f6d 6d69 742f 5377 616e  last-commit/Swan
+00000a90: 4875 6258 2f53 7761 6e4c 6162 2220 616c  HubX/SwanLab" al
+00000aa0: 743d 226c 6963 656e 7365 223e 3c2f 613e  t="license"></a>
+00000ab0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000ac0: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+00000ad0: 6f72 672f 7079 7069 2f73 7761 6e6c 6162  org/pypi/swanlab
+00000ae0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000af0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000b00: 696f 2f70 7970 692f 762f 7377 616e 6c61  io/pypi/v/swanla
+00000b10: 623f 636f 6c6f 723d 6f72 616e 6765 2220  b?color=orange" 
+00000b20: 616c 743d 202f 3e3c 2f61 3e0a 2020 3c61  alt= /></a>.  <a
+00000b30: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00000b40: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+00000b50: 2f73 7761 6e6c 6162 223e 3c69 6d67 2061  /swanlab"><img a
+00000b60: 6c74 3d22 7079 7069 2044 6f77 6e6c 6f61  lt="pypi Downloa
+00000b70: 6422 2073 7263 3d22 6874 7470 733a 2f2f  d" src="https://
+00000b80: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
+00000b90: 2f62 6164 6765 2f73 7761 6e6c 6162 223e  /badge/swanlab">
+00000ba0: 3c2f 613e 0a20 203c 6120 6872 6566 3d22  </a>.  <a href="
+00000bb0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000bc0: 6f6d 2f73 7761 6e68 7562 782f 7377 616e  om/swanhubx/swan
+00000bd0: 6c61 622f 6973 7375 6573 223e 3c69 6d67  lab/issues"><img
+00000be0: 2061 6c74 3d22 6973 7375 6573 2220 7372   alt="issues" sr
+00000bf0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000c00: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000c10: 2f69 7373 7565 732f 7377 616e 6875 6278  /issues/swanhubx
+00000c20: 2f73 7761 6e6c 6162 223e 3c2f 613e 0a20  /swanlab"></a>. 
+00000c30: 203c 6272 3e0a 2020 3c61 2068 7265 663d   <br>.  <a href=
+00000c40: 2268 7474 7073 3a2f 2f73 7761 6e6c 6162  "https://swanlab
+00000c50: 2e63 6e22 2074 6172 6765 743d 225f 626c  .cn" target="_bl
+00000c60: 616e 6b22 3e0a 2020 2020 2020 2020 3c69  ank">.        <i
+00000c70: 6d67 2061 6c74 3d22 5374 6174 6963 2042  mg alt="Static B
+00000c80: 6164 6765 2220 7372 633d 2268 7474 7073  adge" src="https
+00000c90: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000ca0: 6f2f 6261 6467 652f 5072 6f64 7563 742d  o/badge/Product-
+00000cb0: 5377 616e 4c61 62e4 ba91 e7ab afe7 8988  SwanLab.........
+00000cc0: 2d36 3336 6133 6622 3e3c 2f61 3e0a 2020  -636a3f"></a>.  
+00000cd0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000ce0: 2f67 6565 6b74 6563 6873 7475 6469 6f2e  /geektechstudio.
+00000cf0: 6665 6973 6875 2e63 6e2f 7769 6b69 2f4e  feishu.cn/wiki/N
+00000d00: 495a 3977 7035 4c52 6953 7151 796b 697a  IZ9wp5LRiSqQykiz
+00000d10: 6247 6356 7a55 4b6e 6963 2220 7461 7267  bGcVzUKnic" targ
+00000d20: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
+00000d30: 2020 2020 203c 696d 6720 616c 743d 2253       <img alt="S
+00000d40: 7461 7469 6320 4261 6467 6522 2073 7263  tatic Badge" src
+00000d50: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000d60: 6965 6c64 732e 696f 2f62 6164 6765 2f57  ields.io/badge/W
+00000d70: 6543 6861 742d e5be aee4 bfa1 2d34 6362  eChat-......-4cb
+00000d80: 3535 6522 3e3c 2f61 3e0a 2020 3c61 2068  55e"></a>.  <a h
+00000d90: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000da0: 2e78 6961 6f68 6f6e 6773 6875 2e63 6f6d  .xiaohongshu.com
+00000db0: 2f75 7365 722f 7072 6f66 696c 652f 3630  /user/profile/60
+00000dc0: 3537 3836 6239 3030 3030 3030 3030 3031  5786b90000000001
+00000dd0: 3030 3361 3831 2220 7461 7267 6574 3d22  003a81" target="
+00000de0: 5f62 6c61 6e6b 223e 0a20 2020 2020 2020  _blank">.       
+00000df0: 203c 696d 6720 616c 743d 2253 7461 7469   <img alt="Stati
+00000e00: 6320 4261 6467 6522 2073 7263 3d22 6874  c Badge" src="ht
+00000e10: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000e20: 732e 696f 2f62 6164 6765 2fe5 b08f e7ba  s.io/badge/.....
+00000e30: a2e4 b9a6 2d46 3034 3433 3822 3e3c 2f61  ....-F04438"></a
+00000e40: 3e0a 0a3c 2f70 3e0a 0a3c 6469 7620 616c  >..</p>..<div al
+00000e50: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000e60: 3c61 2068 7265 663d 222e 2f68 7474 7073  <a href="./https
+00000e70: 3a2f 2f67 6974 6875 622e 636f 6d2f 5377  ://github.com/Sw
+00000e80: 616e 4875 6258 2f53 7761 6e4c 6162 2f62  anHubX/SwanLab/b
+00000e90: 6c6f 622f 6d61 696e 2f52 4541 444d 452e  lob/main/README.
+00000ea0: 6d64 223e 3c69 6d67 2061 6c74 3d22 e88b  md"><img alt="..
+00000eb0: b1e6 9687 e696 87e6 a1a3 2220 7372 633d  .........." src=
+00000ec0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000ed0: 656c 6473 2e69 6f2f 6261 6467 652f 456e  elds.io/badge/En
+00000ee0: 676c 6973 682d 6439 6439 6439 223e 3c2f  glish-d9d9d9"></
+00000ef0: 613e 0a20 203c 6120 6872 6566 3d22 2e2f  a>.  <a href="./
+00000f00: 5245 4144 4d45 5f63 6e2e 6d64 223e 3c69  README_cn.md"><i
+00000f10: 6d67 2061 6c74 3d22 e4b8 ade6 9687 e696  mg alt="........
+00000f20: 87e6 a1a3 2220 7372 633d 2268 7474 7073  ...." src="https
+00000f30: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000f40: 6f2f 6261 6467 652f e7ae 80e4 bd93 e4b8  o/badge/........
+00000f50: ade6 9687 2d64 3964 3964 3922 3e3c 2f61  ....-d9d9d9"></a
+00000f60: 3e0a 3c2f 6469 763e 0a0a 3c64 6574 6169  >.</div>..<detai
+00000f70: 6c73 3e0a 3c73 756d 6d61 7279 3e54 6162  ls>.<summary>Tab
+00000f80: 6c65 206f 6620 636f 6e74 656e 7473 3c2f  le of contents</
+00000f90: 7375 6d6d 6172 793e 0a0a 2323 2323 2054  summary>..#### T
+00000fa0: 4f43 0a0a 2d20 5bf0 9f91 8bf0 9f8f bb20  OC..- [........ 
+00000fb0: 496e 7472 6f64 7563 7469 6f6e 5d28 232d  Introduction](#-
+00000fc0: 496e 7472 6f64 7563 7469 6f6e 290a 2d20  Introduction).- 
+00000fd0: 5bf0 9f8f 8120 5175 6963 6b20 5374 6172  [.... Quick Star
+00000fe0: 745d 2823 f09f 8f81 2d71 7569 636b 2d73  t](#....-quick-s
+00000ff0: 7461 7274 290a 2020 2020 2d20 5b31 2e49  tart).    - [1.I
+00001000: 6e73 7461 6c6c 6174 696f 6e5d 2823 3169  nstallation](#1i
+00001010: 6e73 7461 6c6c 6174 696f 6e29 0a20 2020  nstallation).   
+00001020: 202d 205b 322e 4c6f 6720 496e 2061 6e64   - [2.Log In and
+00001030: 2047 6574 2074 6865 2041 5049 204b 6579   Get the API Key
+00001040: 5d28 2332 6c6f 672d 696e 2d61 6e64 2d67  ](#2log-in-and-g
+00001050: 6574 2d74 6865 2d61 7069 2d6b 6579 290a  et-the-api-key).
+00001060: 2020 2020 2d20 5b33 2e49 6e74 6567 7261      - [3.Integra
+00001070: 7465 2053 7761 6e4c 6162 2077 6974 6820  te SwanLab with 
+00001080: 596f 7572 2043 6f64 655d 2823 332d 696e  Your Code](#3-in
+00001090: 7465 6772 6174 652d 7377 616e 6c61 622d  tegrate-swanlab-
+000010a0: 7769 7468 2d79 6f75 722d 636f 6465 290a  with-your-code).
+000010b0: 2d20 5bf0 9f93 8320 4d6f 7265 2045 7861  - [.... More Exa
+000010c0: 6d70 6c65 735d 2823 2d6d 6f72 652d 6578  mples](#-more-ex
+000010d0: 616d 706c 6573 290a 2d20 5bf0 9f92 bb20  amples).- [.... 
+000010e0: 5365 6c66 2d68 6f73 7465 645d 2823 2d73  Self-hosted](#-s
+000010f0: 656c 662d 686f 7374 6564 290a 2020 2020  elf-hosted).    
+00001100: 2d20 5b4f 6666 6c69 6e65 2045 7870 6572  - [Offline Exper
+00001110: 696d 656e 7420 5472 6163 6b69 6e67 5d28  iment Tracking](
+00001120: 236f 6666 6c69 6e65 2d65 7870 6572 696d  #offline-experim
+00001130: 656e 742d 7472 6163 6b69 6e67 290a 2020  ent-tracking).  
+00001140: 2020 2d20 5b4f 7065 6e20 4f66 666c 696e    - [Open Offlin
+00001150: 6520 4461 7368 626f 6172 645d 2823 6f70  e Dashboard](#op
+00001160: 656e 2d6f 6666 6c69 6e65 2d62 6f61 7264  en-offline-board
+00001170: 290a 2d20 5bf0 9f9a 9720 496e 7465 6772  ).- [.... Integr
+00001180: 6174 696f 6e5d 2823 2d69 6e74 6567 7261  ation](#-integra
+00001190: 7469 6f6e 290a 2d20 5bf0 9f86 9a20 436f  tion).- [.... Co
+000011a0: 6d70 6172 6973 6f6e 2077 6974 6820 4661  mparison with Fa
+000011b0: 6d69 6c69 6172 2054 6f6f 6c73 5d28 232d  miliar Tools](#-
+000011c0: 636f 6d70 6172 6973 6f6e 2d77 6974 682d  comparison-with-
+000011d0: 6661 6d69 6c69 6172 2d74 6f6f 6c73 290a  familiar-tools).
+000011e0: 2020 2020 2d20 5b54 656e 736f 7262 6f61      - [Tensorboa
+000011f0: 7264 2076 7320 5377 616e 4c61 625d 2823  rd vs SwanLab](#
+00001200: 7465 6e73 6f72 626f 6172 642d 7673 2d73  tensorboard-vs-s
+00001210: 7761 6e6c 6162 290a 2020 2020 2d20 5b57  wanlab).    - [W
+00001220: 6569 6768 7473 2026 2042 6961 7365 7320  eights & Biases 
+00001230: 7673 2053 7761 6e4c 6162 5d28 2377 6569  vs SwanLab](#wei
+00001240: 6768 7473 2d61 6e64 2d62 6961 7365 732d  ghts-and-biases-
+00001250: 7673 2d73 7761 6e6c 6162 290a 2d20 5bf0  vs-swanlab).- [.
+00001260: 9f9b a3ef b88f 2052 6f61 646d 6170 5d28  ...... Roadmap](
+00001270: 2325 4546 2542 3825 3846 2d72 6f61 646d  #%EF%B8%8F-roadm
+00001280: 6170 290a 2020 2020 2d20 5b49 6e20 5072  ap).    - [In Pr
+00001290: 6f67 7265 7373 204e 6f77 5d28 2369 6e2d  ogress Now](#in-
+000012a0: 7072 6f67 7265 7373 2d6e 6f77 290a 2020  progress-now).  
+000012b0: 2020 2d20 5b4e 6578 7420 506c 616e 6e65    - [Next Planne
+000012c0: 645d 2823 6e65 7874 2d70 6c61 6e6e 6564  d](#next-planned
+000012d0: 290a 2020 2020 2d20 5b4c 6f6e 6720 5465  ).    - [Long Te
+000012e0: 726d 2043 6f6e 6365 726e 5d28 236c 6f6e  rm Concern](#lon
+000012f0: 672d 7465 726d 2d63 6f6e 6365 726e 290a  g-term-concern).
+00001300: 2d20 5bf0 9f91 a520 436f 6d6d 756e 6974  - [.... Communit
+00001310: 795d 2823 2d63 6f6d 6d75 6e69 7479 290a  y](#-community).
+00001320: 2020 2020 2d20 5b43 6f6d 6d75 6e69 7479      - [Community
+00001330: 2061 6e64 2053 7570 706f 7274 5d28 2363   and Support](#c
+00001340: 6f6d 6d75 6e69 7479 2d61 6e64 2d73 7570  ommunity-and-sup
+00001350: 706f 7274 290a 2020 2020 2d20 5b53 7761  port).    - [Swa
+00001360: 6e4c 6162 2052 4541 444d 4520 4261 6467  nLab README Badg
+00001370: 655d 2823 7377 616e 6c61 622d 7265 6164  e](#swanlab-read
+00001380: 6d65 2d62 6164 6765 290a 2020 2020 2d20  me-badge).    - 
+00001390: 5b43 6974 696e 6720 5377 616e 4c61 6220  [Citing SwanLab 
+000013a0: 696e 2074 6865 2050 6170 6572 5d28 2363  in the Paper](#c
+000013b0: 6974 696e 672d 7377 616e 6c61 622d 696e  iting-swanlab-in
+000013c0: 2d74 6865 2d70 6170 6572 290a 2020 2020  -the-paper).    
+000013d0: 2d20 5b43 6f6e 7472 6962 7574 6520 746f  - [Contribute to
+000013e0: 2053 7761 6e4c 6162 5d28 2363 6f6e 7472   SwanLab](#contr
+000013f0: 6962 7574 652d 746f 2d73 7761 6e6c 6162  ibute-to-swanlab
+00001400: 290a 2020 2020 2d20 5b44 6f77 6e6c 6f61  ).    - [Downloa
+00001410: 6420 4963 6f6e 5d28 2364 6f77 6e6c 6f61  d Icon](#downloa
+00001420: 642d 6963 6f6e 290a 2d20 5bf0 9f93 8320  d-icon).- [.... 
+00001430: 4c69 6365 6e73 655d 2823 2d6c 6963 656e  License](#-licen
+00001440: 7365 290a 0a3c 6272 2f3e 0a0a 3c2f 6465  se)..<br/>..</de
+00001450: 7461 696c 733e 0a0a 2323 20f0 9f91 8bf0  tails>..## .....
+00001460: 9f8f bb20 496e 7472 6f64 7563 7469 6f6e  ... Introduction
+00001470: 0a0a 5377 616e 4c61 6220 6973 2061 6e20  ..SwanLab is an 
+00001480: 6f70 656e 2d73 6f75 7263 652c 206c 6967  open-source, lig
+00001490: 6874 7765 6967 6874 2041 4920 6578 7065  htweight AI expe
+000014a0: 7269 6d65 6e74 2074 7261 636b 696e 6720  riment tracking 
+000014b0: 746f 6f6c 2074 6861 7420 7072 6f76 6964  tool that provid
+000014c0: 6573 2061 2070 6c61 7466 6f72 6d20 666f  es a platform fo
+000014d0: 7220 7472 6163 6b69 6e67 2c20 636f 6d70  r tracking, comp
+000014e0: 6172 696e 672c 2061 6e64 0a63 6f6c 6c61  aring, and.colla
+000014f0: 626f 7261 7469 6e67 206f 6e20 6578 7065  borating on expe
+00001500: 7269 6d65 6e74 732c 2061 696d 696e 6720  riments, aiming 
+00001510: 746f 2061 6363 656c 6572 6174 6520 7468  to accelerate th
+00001520: 6520 7265 7365 6172 6368 2061 6e64 2064  e research and d
+00001530: 6576 656c 6f70 6d65 6e74 2065 6666 6963  evelopment effic
+00001540: 6965 6e63 7920 6f66 2041 4920 7465 616d  iency of AI team
+00001550: 7320 6279 2031 3030 2074 696d 6573 2e0a  s by 100 times..
+00001560: 0a53 7761 6e4c 6162 e698 afe4 b880 e4b8  .SwanLab........
+00001570: aae5 bc80 e6ba 90e3 8081 e8bd bbe9 878f  ................
+00001580: e7ba a7e7 9a84 4149 e5ae 9ee9 aa8c e8b7  ......AI........
+00001590: 9fe8 b8aa e5b7 a5e5 85b7 efbc 8ce6 8f90  ................
+000015a0: e4be 9be4 ba86 e4b8 80e4 b8aa e8b7 9fe8  ................
+000015b0: b8aa e380 81e6 af94 e8be 83e3 8081 e592  ................
+000015c0: 8ce5 8d8f e4bd 9ce5 ae9e e9aa 8ce7 9a84  ................
+000015d0: e5b9 b3e5 8fb0 efbc 8ce6 97a8 e59c a8e5  ................
+000015e0: 8aa0 e980 9f41 49e7 a094 e58f 91e5 9ba2  .....AI.........
+000015f0: e998 9f31 3030 e580 8de7 9a84 e7a0 94e5  ...100..........
+00001600: 8f91 e695 88e7 8e87 e380 820a 0a49 7420  .............It 
+00001610: 6f66 6665 7273 2061 2075 7365 722d 6672  offers a user-fr
+00001620: 6965 6e64 6c79 2041 5049 2061 6e64 2061  iendly API and a
+00001630: 2064 6563 656e 7420 696e 7465 7266 6163   decent interfac
+00001640: 652c 2063 6f6d 6269 6e69 6e67 2066 6561  e, combining fea
+00001650: 7475 7265 7320 7375 6368 2061 7320 7472  tures such as tr
+00001660: 6163 6b69 6e67 2068 7970 6572 7061 7261  acking hyperpara
+00001670: 6d65 7465 722c 2072 6563 6f72 6469 6e67  meter, recording
+00001680: 0a6d 6574 7269 632c 206f 6e6c 696e 6520  .metric, online 
+00001690: 636f 6c6c 6162 6f72 6174 696f 6e2c 2073  collaboration, s
+000016a0: 6861 7269 6e67 2065 7870 6572 696d 656e  haring experimen
+000016b0: 7420 6c69 6e6b 2c20 7265 616c 2d74 696d  t link, real-tim
+000016c0: 6520 6d65 7373 6167 6520 6e6f 7469 6669  e message notifi
+000016d0: 6361 7469 6f6e 732c 2061 6c6c 6f77 696e  cations, allowin
+000016e0: 6720 796f 7520 746f 2071 7569 636b 6c79  g you to quickly
+000016f0: 2074 7261 636b 204d 4c0a 6578 7065 7269   track ML.experi
+00001700: 6d65 6e74 732c 2076 6973 7561 6c69 7a65  ments, visualize
+00001710: 2070 726f 6365 7373 6573 2c20 616e 6420   processes, and 
+00001720: 7368 6172 6520 7769 7468 2070 6565 7273  share with peers
+00001730: 2e0a 0a42 7920 7573 696e 672c 2072 6573  ...By using, res
+00001740: 6561 7263 6865 7273 2063 616e 2061 6363  earchers can acc
+00001750: 756d 756c 6174 6520 7468 6569 7220 7472  umulate their tr
+00001760: 6169 6e69 6e67 2065 7870 6572 6965 6e63  aining experienc
+00001770: 6573 2061 6e64 2073 6561 6d6c 6573 736c  es and seamlessl
+00001780: 7920 636f 6d6d 756e 6963 6174 6520 616e  y communicate an
+00001790: 6420 636f 6c6c 6162 6f72 6174 6520 7769  d collaborate wi
+000017a0: 7468 2070 6565 7273 2e0a 4d61 6368 696e  th peers..Machin
+000017b0: 6520 6c65 6172 6e69 6e67 2065 6e67 696e  e learning engin
+000017c0: 6565 7273 2063 616e 2064 6576 656c 6f70  eers can develop
+000017d0: 206d 6f64 656c 7320 666f 7220 7072 6f64   models for prod
+000017e0: 7563 7469 6f6e 206d 6f72 6520 6566 6669  uction more effi
+000017f0: 6369 656e 746c 792e 0a0a 215b 5d28 6874  ciently...![](ht
+00001800: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00001810: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00001820: 5377 616e 4875 6258 2f73 7761 6e6c 6162  SwanHubX/swanlab
+00001830: 2f6d 6169 6e2f 7265 6164 6d65 5f66 696c  /main/readme_fil
+00001840: 6573 2f69 6e74 726f 6475 6374 696f 6e2e  es/introduction.
+00001850: 706e 6729 0a0a 4865 7265 2069 7320 7468  png)..Here is th
+00001860: 6520 456e 676c 6973 6820 7665 7273 696f  e English versio
+00001870: 6e20 6f66 2074 6865 2063 6f72 6520 6665  n of the core fe
+00001880: 6174 7572 6520 6c69 7374 2066 6f72 2061  ature list for a
+00001890: 6e20 4149 2070 6c61 7466 6f72 6d3a 0a0a  n AI platform:..
+000018a0: 2a2a 312e 20f0 9f93 8a20 4578 7065 7269  **1. .... Experi
+000018b0: 6d65 6e74 616c 204d 6574 7269 6373 2061  mental Metrics a
+000018c0: 6e64 2054 7261 636b 696e 6720 4879 7065  nd Tracking Hype
+000018d0: 7270 6172 616d 6574 6572 2a2a 3a20 456d  rparameter**: Em
+000018e0: 6265 6420 796f 7572 206d 6163 6869 6e65  bed your machine
+000018f0: 206c 6561 726e 696e 6720 7069 7065 6c69   learning pipeli
+00001900: 6e65 2077 6974 6820 6d69 6e69 6d61 6c69  ne with minimali
+00001910: 7374 6963 2063 6f64 650a 616e 6420 7472  stic code.and tr
+00001920: 6163 6b20 6b65 7920 7472 6169 6e69 6e67  ack key training
+00001930: 206d 6574 7269 6373 2e0a 0a2d 2046 6c65   metrics...- Fle
+00001940: 7869 626c 6520 7265 636f 7264 696e 6720  xible recording 
+00001950: 6f66 2068 7970 6572 7061 7261 6d65 7465  of hyperparamete
+00001960: 7273 2061 6e64 2065 7870 6572 696d 656e  rs and experimen
+00001970: 7420 636f 6e66 6967 7572 6174 696f 6e73  t configurations
+00001980: 2e0a 2d20 2a2a 5375 7070 6f72 7465 6420  ..- **Supported 
+00001990: 6d65 7461 6461 7461 2074 7970 6573 2a2a  metadata types**
+000019a0: 3a20 7363 616c 6172 206d 6574 7269 6373  : scalar metrics
+000019b0: 2c20 696d 6167 6573 2c20 6175 6469 6f2c  , images, audio,
+000019c0: 2074 6578 742c 2065 7463 2e0a 2d20 2a2a   text, etc..- **
+000019d0: 5375 7070 6f72 7465 6420 6368 6172 7420  Supported chart 
+000019e0: 7479 7065 732a 2a3a 206c 696e 6520 6772  types**: line gr
+000019f0: 6170 6873 2c20 6d65 6469 6120 6368 6172  aphs, media char
+00001a00: 7473 2028 696d 6167 6573 2c20 6175 6469  ts (images, audi
+00001a10: 6f2c 2074 6578 7429 2c20 6574 632e 0a2d  o, text), etc..-
+00001a20: 202a 2a41 7574 6f6d 6174 6963 206c 6f67   **Automatic log
+00001a30: 6769 6e67 2a2a 3a20 636f 6e73 6f6c 6520  ging**: console 
+00001a40: 6c6f 6767 696e 672c 2047 5055 2068 6172  logging, GPU har
+00001a50: 6477 6172 652c 2047 6974 2069 6e66 6f72  dware, Git infor
+00001a60: 6d61 7469 6f6e 2c20 5079 7468 6f6e 2069  mation, Python i
+00001a70: 6e74 6572 7072 6574 6572 2c20 6c69 7374  nterpreter, list
+00001a80: 206f 6620 5079 7468 6f6e 206c 6962 7261   of Python libra
+00001a90: 7269 6573 2c0a 2020 636f 6465 2064 6972  ries,.  code dir
+00001aa0: 6563 746f 7279 2e0a 0a2a 2a32 2e20 e29a  ectory...**2. ..
+00001ab0: a1ef b88f 2043 6f6d 7072 6568 656e 7369  .... Comprehensi
+00001ac0: 7665 2046 7261 6d65 776f 726b 2049 6e74  ve Framework Int
+00001ad0: 6567 7261 7469 6f6e 2a2a 3a20 5079 546f  egration**: PyTo
+00001ae0: 7263 68e3 8081 5465 6e73 6f72 666c 6f77  rch...Tensorflow
+00001af0: e380 8150 7954 6f72 6368 204c 6967 6874  ...PyTorch Light
+00001b00: 6e69 6e67 e380 81f0 9fa4 9748 7567 6769  ning.......Huggi
+00001b10: 6e67 4661 6365 e380 8154 7261 6e73 666f  ngFace...Transfo
+00001b20: 726d 6572 73e3 8081 4d4d 456e 6769 6e65  rmers...MMEngine
+00001b30: e380 8155 6c74 7261 6c79 7469 6373 e380  ...Ultralytics..
+00001b40: 8166 6173 7461 69e3 8081 5465 6e73 6f72  .fastai...Tensor
+00001b50: 626f 6172 64e3 8081 4f70 656e 4149 e380  board...OpenAI..
+00001b60: 815a 6869 7075 4149 e380 8148 7964 7261  .ZhipuAI...Hydra
+00001b70: e380 812e 2e2e 0a0a 2a2a 332e 20f0 9f93  ........**3. ...
+00001b80: a620 4f72 6761 6e69 7a69 6e67 2045 7870  . Organizing Exp
+00001b90: 6572 696d 656e 7473 2a2a 3a20 4365 6e74  eriments**: Cent
+00001ba0: 7261 6c69 7a65 6420 6461 7368 626f 6172  ralized dashboar
+00001bb0: 6420 666f 7220 6566 6669 6369 656e 746c  d for efficientl
+00001bc0: 7920 6d61 6e61 6769 6e67 206d 756c 7469  y managing multi
+00001bd0: 706c 6520 7072 6f6a 6563 7473 2061 6e64  ple projects and
+00001be0: 2065 7870 6572 696d 656e 7473 2c0a 7072   experiments,.pr
+00001bf0: 6f76 6964 696e 6720 616e 206f 7665 7276  oviding an overv
+00001c00: 6965 7720 6f66 2074 7261 696e 696e 6720  iew of training 
+00001c10: 6174 2061 2067 6c61 6e63 652e 0a0a 2a2a  at a glance...**
+00001c20: 342e 20f0 9f86 9a20 436f 6d70 6172 696e  4. .... Comparin
+00001c30: 6720 5265 7375 6c74 732a 2a3a 2055 7365  g Results**: Use
+00001c40: 206f 6e6c 696e 6520 7461 626c 6573 2061   online tables a
+00001c50: 6e64 2070 6169 7265 6420 6368 6172 7473  nd paired charts
+00001c60: 2074 6f20 636f 6d70 6172 6520 7468 6520   to compare the 
+00001c70: 6879 7065 7270 6172 616d 6574 6572 7320  hyperparameters 
+00001c80: 616e 6420 6f75 7463 6f6d 6573 206f 6620  and outcomes of 
+00001c90: 6469 6666 6572 656e 740a 6578 7065 7269  different.experi
+00001ca0: 6d65 6e74 732c 2064 6576 656c 6f70 696e  ments, developin
+00001cb0: 6720 6974 6572 6174 6976 6520 696e 7370  g iterative insp
+00001cc0: 6972 6174 696f 6e2e 0a0a 2a2a 352e 20f0  iration...**5. .
+00001cd0: 9f91 a520 4f6e 6c69 6e65 2043 6f6c 6c61  ... Online Colla
+00001ce0: 626f 7261 7469 6f6e 2a2a 3a20 436f 6c6c  boration**: Coll
+00001cf0: 6162 6f72 6174 6520 7769 7468 2079 6f75  aborate with you
+00001d00: 7220 7465 616d 206f 6e20 7472 6169 6e69  r team on traini
+00001d10: 6e67 2070 726f 6a65 6374 732c 2073 7570  ng projects, sup
+00001d20: 706f 7274 696e 6720 7265 616c 2d74 696d  porting real-tim
+00001d30: 6520 7379 6e63 6872 6f6e 697a 6174 696f  e synchronizatio
+00001d40: 6e20 6f66 0a65 7870 6572 696d 656e 7473  n of.experiments
+00001d50: 2075 6e64 6572 2074 6865 2073 616d 6520   under the same 
+00001d60: 7072 6f6a 6563 742c 2061 6c6c 6f77 696e  project, allowin
+00001d70: 6720 796f 7520 746f 2073 796e 6368 726f  g you to synchro
+00001d80: 6e69 7a65 2074 7261 696e 696e 6720 7265  nize training re
+00001d90: 636f 7264 7320 6f66 2074 6865 2074 6561  cords of the tea
+00001da0: 6d20 6f6e 6c69 6e65 2061 6e64 2073 6861  m online and sha
+00001db0: 7265 2069 6e73 6967 6874 730a 616e 6420  re insights.and 
+00001dc0: 7375 6767 6573 7469 6f6e 7320 6261 7365  suggestions base
+00001dd0: 6420 6f6e 2072 6573 756c 7473 2e0a 0a2a  d on results...*
+00001de0: 2a36 2e20 e29c 89ef b88f 2053 6861 7269  *6. ...... Shari
+00001df0: 6e67 2052 6573 756c 7473 2a2a 3a20 436f  ng Results**: Co
+00001e00: 7079 2061 6e64 2073 656e 6420 7065 7273  py and send pers
+00001e10: 6973 7465 6e74 2055 524c 7320 746f 2073  istent URLs to s
+00001e20: 6861 7265 2065 6163 6820 6578 7065 7269  hare each experi
+00001e30: 6d65 6e74 2c20 6566 6669 6369 656e 746c  ment, efficientl
+00001e40: 7920 7365 6e64 2074 6865 6d20 746f 2063  y send them to c
+00001e50: 6f6c 6c65 6167 7565 732c 0a6f 7220 656d  olleagues,.or em
+00001e60: 6265 6420 7468 656d 2069 6e20 6f6e 6c69  bed them in onli
+00001e70: 6e65 206e 6f74 6573 2e0a 0a2a 2a37 2e20  ne notes...**7. 
+00001e80: f09f 92bb 2053 656c 662d 686f 7374 696e  .... Self-hostin
+00001e90: 6720 5375 7070 6f72 742a 2a3a 2053 7570  g Support**: Sup
+00001ea0: 706f 7274 7320 6f66 666c 696e 6520 6d6f  ports offline mo
+00001eb0: 6465 2077 6974 6820 6120 7365 6c66 2d68  de with a self-h
+00001ec0: 6f73 7465 6420 636f 6d6d 756e 6974 7920  osted community 
+00001ed0: 7665 7273 696f 6e20 7468 6174 2061 6c73  version that als
+00001ee0: 6f20 616c 6c6f 7773 2066 6f72 2064 6173  o allows for das
+00001ef0: 6862 6f61 7264 0a76 6965 7769 6e67 2061  hboard.viewing a
+00001f00: 6e64 2065 7870 6572 696d 656e 7420 6d61  nd experiment ma
+00001f10: 6e61 6765 6d65 6e74 2e0a 0a3e 205c 5b21  nagement...> \[!
+00001f20: 494d 504f 5254 414e 545d 0a3e 0a3e 202a  IMPORTANT].>.> *
+00001f30: 2a53 7461 7220 5573 2a2a 2c20 596f 7520  *Star Us**, You 
+00001f40: 7769 6c6c 2072 6563 6569 7665 2061 6c6c  will receive all
+00001f50: 2072 656c 6561 7365 206e 6f74 6966 6963   release notific
+00001f60: 6174 696f 6e73 2066 726f 6d20 4769 7448  ations from GitH
+00001f70: 7562 2077 6974 686f 7574 2061 6e79 2064  ub without any d
+00001f80: 656c 6179 207e 20e2 ad90 efb8 8f0a 0a0a  elay ~ .........
+00001f90: 0a21 5b73 7461 722d 7573 5d28 6874 7470  .![star-us](http
+00001fa0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001fb0: 6572 636f 6e74 656e 742e 636f 6d2f 5377  ercontent.com/Sw
+00001fc0: 616e 4875 6258 2f73 7761 6e6c 6162 2f6d  anHubX/swanlab/m
+00001fd0: 6169 6e2f 7265 6164 6d65 5f66 696c 6573  ain/readme_files
+00001fe0: 2f73 7461 722d 7573 2e70 6e67 290a 0a3c  /star-us.png)..<
+00001ff0: 6272 3e0a 0a23 2320 f09f 8f81 2051 7569  br>..## .... Qui
+00002000: 636b 2053 7461 7274 0a0a 2323 2320 312e  ck Start..### 1.
+00002010: 496e 7374 616c 6c61 7469 6f6e 0a0a 6060  Installation..``
+00002020: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+00002030: 6c20 7377 616e 6c61 620a 6060 600a 0a23  l swanlab.```..#
+00002040: 2323 2032 2e4c 6f67 2069 6e20 616e 6420  ## 2.Log in and 
+00002050: 6765 7420 7468 6520 4150 4920 4b65 790a  get the API Key.
+00002060: 0a31 2e20 2a2a 4672 6565 205b 5369 676e  .1. **Free [Sign
+00002070: 2055 705d 2868 7474 7073 3a2f 2f73 7761   Up](https://swa
+00002080: 6e6c 6162 2e63 6e29 2a2a 0a0a 322e 202a  nlab.cn)**..2. *
+00002090: 2a4c 6f67 2069 6e20 746f 2079 6f75 7220  *Log in to your 
+000020a0: 6163 636f 756e 742a 2a2c 2067 6f20 746f  account**, go to
+000020b0: 2055 7365 7220 5365 7474 696e 6773 203e   User Settings >
+000020c0: 205b 4150 4920 4b65 795d 2868 7474 7073   [API Key](https
+000020d0: 3a2f 2f73 7761 6e6c 6162 2e63 6e2f 7365  ://swanlab.cn/se
+000020e0: 7474 696e 6773 2920 616e 6420 636f 7079  ttings) and copy
+000020f0: 2079 6f75 7220 4150 4920 4b65 792e 0a0a   your API Key...
+00002100: 332e 202a 2a4f 7065 6e20 796f 7572 2074  3. **Open your t
+00002110: 6572 6d69 6e61 6c20 616e 6420 656e 7465  erminal and ente
+00002120: 722a 2a3a 0a0a 6060 6062 6173 680a 7377  r**:..```bash.sw
+00002130: 616e 6c61 6220 6c6f 6769 6e0a 6060 600a  anlab login.```.
+00002140: 0a57 6865 6e20 7072 6f6d 7074 6564 2c20  .When prompted, 
+00002150: 656e 7465 7220 796f 7572 2041 5049 204b  enter your API K
+00002160: 6579 2061 6e64 2070 7265 7373 2045 6e74  ey and press Ent
+00002170: 6572 2074 6f20 636f 6d70 6c65 7465 2074  er to complete t
+00002180: 6865 206c 6f67 696e 2e0a 0a23 2323 2033  he login...### 3
+00002190: 2e20 496e 7465 6772 6174 6520 5377 616e  . Integrate Swan
+000021a0: 4c61 6220 7769 7468 2059 6f75 7220 436f  Lab with Your Co
+000021b0: 6465 0a0a 6060 6070 7974 686f 6e0a 696d  de..```python.im
+000021c0: 706f 7274 2073 7761 6e6c 6162 0a0a 2320  port swanlab..# 
+000021d0: 4372 6561 7465 2061 206e 6577 2053 7761  Create a new Swa
+000021e0: 6e4c 6162 2065 7870 6572 696d 656e 740a  nLab experiment.
+000021f0: 7377 616e 6c61 622e 696e 6974 280a 2020  swanlab.init(.  
+00002200: 2020 7072 6f6a 6563 743d 226d 792d 6669    project="my-fi
+00002210: 7273 742d 6d6c 222c 0a20 2020 2063 6f6e  rst-ml",.    con
+00002220: 6669 673d 7b27 6c65 6172 6e69 6e67 2d72  fig={'learning-r
+00002230: 6174 6527 3a20 302e 3030 337d 0a29 0a0a  ate': 0.003}.)..
+00002240: 2320 4c6f 6720 6d65 7472 6963 730a 666f  # Log metrics.fo
+00002250: 7220 6920 696e 2072 616e 6765 2831 3029  r i in range(10)
+00002260: 3a0a 2020 2020 7377 616e 6c61 622e 6c6f  :.    swanlab.lo
+00002270: 6728 7b22 6c6f 7373 223a 2069 7d29 0a60  g({"loss": i}).`
+00002280: 6060 0a0a 2a2a 416c 6c20 7365 7421 2a2a  ``..**All set!**
+00002290: 2056 6973 6974 205b 5377 616e 4c61 625d   Visit [SwanLab]
+000022a0: 2868 7474 7073 3a2f 2f73 7761 6e6c 6162  (https://swanlab
+000022b0: 2e63 6e29 2074 6f20 7365 6520 796f 7572  .cn) to see your
+000022c0: 2066 6972 7374 2053 7761 6e4c 6162 2065   first SwanLab e
+000022d0: 7870 6572 696d 656e 742e 0a0a 215b 4d4e  xperiment...![MN
+000022e0: 4953 545d 2868 7474 7073 3a2f 2f72 6177  IST](https://raw
+000022f0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00002300: 6e74 2e63 6f6d 2f53 7761 6e48 7562 582f  nt.com/SwanHubX/
+00002310: 7377 616e 6c61 622f 6d61 696e 2f72 6561  swanlab/main/rea
+00002320: 646d 655f 6669 6c65 732f 7265 6164 6d65  dme_files/readme
+00002330: 2d6d 6e69 7374 2e70 6e67 290a 0a3c 6272  -mnist.png)..<br
+00002340: 3e0a 0a23 2320 f09f 9383 204d 6f72 6520  >..## .... More 
+00002350: 4578 616d 706c 6573 0a0a 3c64 6574 6169  Examples..<detai
+00002360: 6c73 3e0a 3c73 756d 6d61 7279 3e4d 4e49  ls>.<summary>MNI
+00002370: 5354 3c2f 7375 6d6d 6172 793e 0a0a 6060  ST</summary>..``
+00002380: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
+00002390: 730a 696d 706f 7274 2074 6f72 6368 0a66  s.import torch.f
+000023a0: 726f 6d20 746f 7263 6820 696d 706f 7274  rom torch import
+000023b0: 206e 6e2c 206f 7074 696d 2c20 7574 696c   nn, optim, util
+000023c0: 730a 696d 706f 7274 2074 6f72 6368 2e6e  s.import torch.n
+000023d0: 6e2e 6675 6e63 7469 6f6e 616c 2061 7320  n.functional as 
+000023e0: 460a 6672 6f6d 2074 6f72 6368 7669 7369  F.from torchvisi
+000023f0: 6f6e 2e64 6174 6173 6574 7320 696d 706f  on.datasets impo
+00002400: 7274 204d 4e49 5354 0a66 726f 6d20 746f  rt MNIST.from to
+00002410: 7263 6876 6973 696f 6e2e 7472 616e 7366  rchvision.transf
+00002420: 6f72 6d73 2069 6d70 6f72 7420 546f 5465  orms import ToTe
+00002430: 6e73 6f72 0a69 6d70 6f72 7420 7377 616e  nsor.import swan
+00002440: 6c61 620a 0a0a 2320 434e 4ee7 bd91 e7bb  lab...# CNN.....
+00002450: 9ce6 9e84 e5bb ba0a 636c 6173 7320 436f  ........class Co
+00002460: 6e76 4e65 7428 6e6e 2e4d 6f64 756c 6529  nvNet(nn.Module)
+00002470: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00002480: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00002490: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+000024a0: 5f5f 2829 0a20 2020 2020 2020 2023 2031  __().        # 1
+000024b0: 2c32 3878 3238 0a20 2020 2020 2020 2073  ,28x28.        s
+000024c0: 656c 662e 636f 6e76 3120 3d20 6e6e 2e43  elf.conv1 = nn.C
+000024d0: 6f6e 7632 6428 312c 2031 302c 2035 2920  onv2d(1, 10, 5) 
+000024e0: 2023 2031 302c 2032 3478 3234 0a20 2020   # 10, 24x24.   
+000024f0: 2020 2020 2073 656c 662e 636f 6e76 3220       self.conv2 
+00002500: 3d20 6e6e 2e43 6f6e 7632 6428 3130 2c20  = nn.Conv2d(10, 
+00002510: 3230 2c20 3329 2020 2320 3132 382c 2031  20, 3)  # 128, 1
+00002520: 3078 3130 0a20 2020 2020 2020 2073 656c  0x10.        sel
+00002530: 662e 6663 3120 3d20 6e6e 2e4c 696e 6561  f.fc1 = nn.Linea
+00002540: 7228 3230 202a 2031 3020 2a20 3130 2c20  r(20 * 10 * 10, 
+00002550: 3530 3029 0a20 2020 2020 2020 2073 656c  500).        sel
+00002560: 662e 6663 3220 3d20 6e6e 2e4c 696e 6561  f.fc2 = nn.Linea
+00002570: 7228 3530 302c 2031 3029 0a0a 2020 2020  r(500, 10)..    
+00002580: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
+00002590: 2c20 7829 3a0a 2020 2020 2020 2020 696e  , x):.        in
+000025a0: 5f73 697a 6520 3d20 782e 7369 7a65 2830  _size = x.size(0
+000025b0: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
+000025c0: 7365 6c66 2e63 6f6e 7631 2878 2920 2023  self.conv1(x)  #
+000025d0: 2032 340a 2020 2020 2020 2020 6f75 7420   24.        out 
+000025e0: 3d20 462e 7265 6c75 286f 7574 290a 2020  = F.relu(out).  
+000025f0: 2020 2020 2020 6f75 7420 3d20 462e 6d61        out = F.ma
+00002600: 785f 706f 6f6c 3264 286f 7574 2c20 322c  x_pool2d(out, 2,
+00002610: 2032 2920 2023 2031 320a 2020 2020 2020   2)  # 12.      
+00002620: 2020 6f75 7420 3d20 7365 6c66 2e63 6f6e    out = self.con
+00002630: 7632 286f 7574 2920 2023 2031 300a 2020  v2(out)  # 10.  
+00002640: 2020 2020 2020 6f75 7420 3d20 462e 7265        out = F.re
+00002650: 6c75 286f 7574 290a 2020 2020 2020 2020  lu(out).        
+00002660: 6f75 7420 3d20 6f75 742e 7669 6577 2869  out = out.view(i
+00002670: 6e5f 7369 7a65 2c20 2d31 290a 2020 2020  n_size, -1).    
+00002680: 2020 2020 6f75 7420 3d20 7365 6c66 2e66      out = self.f
+00002690: 6331 286f 7574 290a 2020 2020 2020 2020  c1(out).        
+000026a0: 6f75 7420 3d20 462e 7265 6c75 286f 7574  out = F.relu(out
+000026b0: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
+000026c0: 7365 6c66 2e66 6332 286f 7574 290a 2020  self.fc2(out).  
+000026d0: 2020 2020 2020 6f75 7420 3d20 462e 6c6f        out = F.lo
+000026e0: 675f 736f 6674 6d61 7828 6f75 742c 2064  g_softmax(out, d
+000026f0: 696d 3d31 290a 2020 2020 2020 2020 7265  im=1).        re
+00002700: 7475 726e 206f 7574 0a0a 0a23 20e6 8d95  turn out...# ...
+00002710: e88e b7e5 b9b6 e58f afe8 a786 e58c 96e5  ................
+00002720: 898d 3230 e5bc a0e5 9bbe e583 8f0a 6465  ..20..........de
+00002730: 6620 6c6f 675f 696d 6167 6573 286c 6f61  f log_images(loa
+00002740: 6465 722c 206e 756d 5f69 6d61 6765 733d  der, num_images=
+00002750: 3136 293a 0a20 2020 2069 6d61 6765 735f  16):.    images_
+00002760: 6c6f 6767 6564 203d 2030 0a20 2020 206c  logged = 0.    l
+00002770: 6f67 6765 645f 696d 6167 6573 203d 205b  ogged_images = [
+00002780: 5d0a 2020 2020 666f 7220 696d 6167 6573  ].    for images
+00002790: 2c20 6c61 6265 6c73 2069 6e20 6c6f 6164  , labels in load
+000027a0: 6572 3a0a 2020 2020 2020 2020 2320 696d  er:.        # im
+000027b0: 6167 6573 3a20 6261 7463 6820 6f66 2069  ages: batch of i
+000027c0: 6d61 6765 732c 206c 6162 656c 733a 2062  mages, labels: b
+000027d0: 6174 6368 206f 6620 6c61 6265 6c73 0a20  atch of labels. 
+000027e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000027f0: 7261 6e67 6528 696d 6167 6573 2e73 6861  range(images.sha
+00002800: 7065 5b30 5d29 3a0a 2020 2020 2020 2020  pe[0]):.        
+00002810: 2020 2020 6966 2069 6d61 6765 735f 6c6f      if images_lo
+00002820: 6767 6564 203c 206e 756d 5f69 6d61 6765  gged < num_image
+00002830: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00002840: 2020 2023 20e4 bdbf e794 a873 7761 6e6c     # ......swanl
+00002850: 6162 2e49 6d61 6765 e5b0 86e5 9bbe e583  ab.Image........
+00002860: 8fe8 bdac e68d a2e4 b8ba 7761 6e64 62e5  ..........wandb.
+00002870: 8faf e8a7 86e5 8c96 e6a0 bce5 bc8f 0a20  ............... 
+00002880: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002890: 6f67 6765 645f 696d 6167 6573 2e61 7070  ogged_images.app
+000028a0: 656e 6428 7377 616e 6c61 622e 496d 6167  end(swanlab.Imag
+000028b0: 6528 696d 6167 6573 5b69 5d2c 2063 6170  e(images[i], cap
+000028c0: 7469 6f6e 3d66 224c 6162 656c 3a20 7b6c  tion=f"Label: {l
+000028d0: 6162 656c 735b 695d 7d22 2929 0a20 2020  abels[i]}")).   
+000028e0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+000028f0: 6765 735f 6c6f 6767 6564 202b 3d20 310a  ges_logged += 1.
+00002900: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002920: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00002930: 6966 2069 6d61 6765 735f 6c6f 6767 6564  if images_logged
+00002940: 203e 3d20 6e75 6d5f 696d 6167 6573 3a0a   >= num_images:.
+00002950: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00002960: 6b0a 2020 2020 7377 616e 6c61 622e 6c6f  k.    swanlab.lo
+00002970: 6728 7b22 4d4e 4953 542d 5072 6576 6965  g({"MNIST-Previe
+00002980: 7722 3a20 6c6f 6767 6564 5f69 6d61 6765  w": logged_image
+00002990: 737d 290a 0a0a 6966 205f 5f6e 616d 655f  s})...if __name_
+000029a0: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
+000029b0: 0a0a 2020 2020 2320 e588 9de5 a78b e58c  ..    # ........
+000029c0: 9673 7761 6e6c 6162 0a20 2020 2072 756e  .swanlab.    run
+000029d0: 203d 2073 7761 6e6c 6162 2e69 6e69 7428   = swanlab.init(
+000029e0: 0a20 2020 2020 2020 2070 726f 6a65 6374  .        project
+000029f0: 3d22 4d4e 4953 542d 6578 616d 706c 6522  ="MNIST-example"
+00002a00: 2c0a 2020 2020 2020 2020 6578 7065 7269  ,.        experi
+00002a10: 6d65 6e74 5f6e 616d 653d 2243 6f6e 764e  ment_name="ConvN
+00002a20: 6574 222c 0a20 2020 2020 2020 2064 6573  et",.        des
+00002a30: 6372 6970 7469 6f6e 3d22 5472 6169 6e20  cription="Train 
+00002a40: 436f 6e76 4e65 7420 6f6e 204d 4e49 5354  ConvNet on MNIST
+00002a50: 2064 6174 6173 6574 2e22 2c0a 2020 2020   dataset.",.    
+00002a60: 2020 2020 636f 6e66 6967 3d7b 0a20 2020      config={.   
+00002a70: 2020 2020 2020 2020 2022 6d6f 6465 6c22           "model"
+00002a80: 3a20 2243 4e4e 222c 0a20 2020 2020 2020  : "CNN",.       
+00002a90: 2020 2020 2022 6f70 7469 6d22 3a20 2241       "optim": "A
+00002aa0: 6461 6d22 2c0a 2020 2020 2020 2020 2020  dam",.          
+00002ab0: 2020 226c 7222 3a20 302e 3030 312c 0a20    "lr": 0.001,. 
+00002ac0: 2020 2020 2020 2020 2020 2022 6261 7463             "batc
+00002ad0: 685f 7369 7a65 223a 2035 3132 2c0a 2020  h_size": 512,.  
+00002ae0: 2020 2020 2020 2020 2020 226e 756d 5f65            "num_e
+00002af0: 706f 6368 7322 3a20 3130 2c0a 2020 2020  pochs": 10,.    
+00002b00: 2020 2020 2020 2020 2274 7261 696e 5f64          "train_d
+00002b10: 6174 6173 6574 5f6e 756d 223a 2035 3530  ataset_num": 550
+00002b20: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+00002b30: 2276 616c 5f64 6174 6173 6574 5f6e 756d  "val_dataset_num
+00002b40: 223a 2035 3030 302c 0a20 2020 2020 2020  ": 5000,.       
+00002b50: 207d 2c0a 2020 2020 290a 0a20 2020 2023   },.    )..    #
+00002b60: 20e8 aebe e7bd aee8 aead e7bb 83e6 9cba   ...............
+00002b70: e380 81e9 aa8c e8af 81e9 9b86 e592 8ce6  ................
+00002b80: b58b e8af 95e9 9b86 0a20 2020 2064 6174  .........    dat
+00002b90: 6173 6574 203d 204d 4e49 5354 286f 732e  aset = MNIST(os.
+00002ba0: 6765 7463 7764 2829 2c20 7472 6169 6e3d  getcwd(), train=
+00002bb0: 5472 7565 2c20 646f 776e 6c6f 6164 3d54  True, download=T
+00002bc0: 7275 652c 2074 7261 6e73 666f 726d 3d54  rue, transform=T
+00002bd0: 6f54 656e 736f 7228 2929 0a20 2020 2074  oTensor()).    t
+00002be0: 7261 696e 5f64 6174 6173 6574 2c20 7661  rain_dataset, va
+00002bf0: 6c5f 6461 7461 7365 7420 3d20 7574 696c  l_dataset = util
+00002c00: 732e 6461 7461 2e72 616e 646f 6d5f 7370  s.data.random_sp
+00002c10: 6c69 7428 0a20 2020 2020 2020 2064 6174  lit(.        dat
+00002c20: 6173 6574 2c20 5b72 756e 2e63 6f6e 6669  aset, [run.confi
+00002c30: 672e 7472 6169 6e5f 6461 7461 7365 745f  g.train_dataset_
+00002c40: 6e75 6d2c 2072 756e 2e63 6f6e 6669 672e  num, run.config.
+00002c50: 7661 6c5f 6461 7461 7365 745f 6e75 6d5d  val_dataset_num]
+00002c60: 0a20 2020 2029 0a0a 2020 2020 7472 6169  .    )..    trai
+00002c70: 6e5f 6c6f 6164 6572 203d 2075 7469 6c73  n_loader = utils
+00002c80: 2e64 6174 612e 4461 7461 4c6f 6164 6572  .data.DataLoader
+00002c90: 2874 7261 696e 5f64 6174 6173 6574 2c20  (train_dataset, 
+00002ca0: 6261 7463 685f 7369 7a65 3d72 756e 2e63  batch_size=run.c
+00002cb0: 6f6e 6669 672e 6261 7463 685f 7369 7a65  onfig.batch_size
+00002cc0: 2c20 7368 7566 666c 653d 5472 7565 290a  , shuffle=True).
+00002cd0: 2020 2020 7661 6c5f 6c6f 6164 6572 203d      val_loader =
+00002ce0: 2075 7469 6c73 2e64 6174 612e 4461 7461   utils.data.Data
+00002cf0: 4c6f 6164 6572 2876 616c 5f64 6174 6173  Loader(val_datas
+00002d00: 6574 2c20 6261 7463 685f 7369 7a65 3d31  et, batch_size=1
+00002d10: 2c20 7368 7566 666c 653d 4661 6c73 6529  , shuffle=False)
+00002d20: 0a0a 2020 2020 2320 e588 9de5 a78b e58c  ..    # ........
+00002d30: 96e6 a8a1 e59e 8be3 8081 e68d 9fe5 a4b1  ................
+00002d40: e587 bde6 95b0 e592 8ce4 bc98 e58c 96e5  ................
+00002d50: 99a8 0a20 2020 206d 6f64 656c 203d 2043  ...    model = C
+00002d60: 6f6e 764e 6574 2829 0a20 2020 2063 7269  onvNet().    cri
+00002d70: 7465 7269 6f6e 203d 206e 6e2e 4372 6f73  terion = nn.Cros
+00002d80: 7345 6e74 726f 7079 4c6f 7373 2829 0a20  sEntropyLoss(). 
+00002d90: 2020 206f 7074 696d 697a 6572 203d 206f     optimizer = o
+00002da0: 7074 696d 2e41 6461 6d28 6d6f 6465 6c2e  ptim.Adam(model.
+00002db0: 7061 7261 6d65 7465 7273 2829 2c20 6c72  parameters(), lr
+00002dc0: 3d72 756e 2e63 6f6e 6669 672e 6c72 290a  =run.config.lr).
+00002dd0: 0a20 2020 2023 20ef bc88 e58f afe9 8089  .    # .........
+00002de0: efbc 89e7 9c8b e4b8 80e4 b88b e695 b0e6  ................
+00002df0: 8dae e99b 86e7 9a84 e589 8d31 36e5 bca0  ...........16...
+00002e00: e59b bee5 838f 0a20 2020 206c 6f67 5f69  .......    log_i
+00002e10: 6d61 6765 7328 7472 6169 6e5f 6c6f 6164  mages(train_load
+00002e20: 6572 2c20 3136 290a 0a20 2020 2023 20e5  er, 16)..    # .
+00002e30: bc80 e5a7 8be8 aead e7bb 830a 2020 2020  ............    
+00002e40: 666f 7220 6570 6f63 6820 696e 2072 616e  for epoch in ran
+00002e50: 6765 2831 2c20 7275 6e2e 636f 6e66 6967  ge(1, run.config
+00002e60: 2e6e 756d 5f65 706f 6368 7329 3a0a 2020  .num_epochs):.  
+00002e70: 2020 2020 2020 7377 616e 6c61 622e 6c6f        swanlab.lo
+00002e80: 6728 7b22 7472 6169 6e2f 6570 6f63 6822  g({"train/epoch"
+00002e90: 3a20 6570 6f63 687d 290a 2020 2020 2020  : epoch}).      
+00002ea0: 2020 2320 e8ae ade7 bb83 e5be aae7 8eaf    # ............
+00002eb0: 0a20 2020 2020 2020 2066 6f72 2069 7465  .        for ite
+00002ec0: 722c 2062 6174 6368 2069 6e20 656e 756d  r, batch in enum
+00002ed0: 6572 6174 6528 7472 6169 6e5f 6c6f 6164  erate(train_load
+00002ee0: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+00002ef0: 2078 2c20 7920 3d20 6261 7463 680a 2020   x, y = batch.  
+00002f00: 2020 2020 2020 2020 2020 6f70 7469 6d69            optimi
+00002f10: 7a65 722e 7a65 726f 5f67 7261 6428 290a  zer.zero_grad().
+00002f20: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00002f30: 7574 203d 206d 6f64 656c 2878 290a 2020  ut = model(x).  
+00002f40: 2020 2020 2020 2020 2020 6c6f 7373 203d            loss =
+00002f50: 2063 7269 7465 7269 6f6e 286f 7574 7075   criterion(outpu
+00002f60: 742c 2079 290a 2020 2020 2020 2020 2020  t, y).          
+00002f70: 2020 6c6f 7373 2e62 6163 6b77 6172 6428    loss.backward(
+00002f80: 290a 2020 2020 2020 2020 2020 2020 6f70  ).            op
+00002f90: 7469 6d69 7a65 722e 7374 6570 2829 0a0a  timizer.step()..
+00002fa0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00002fb0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00002fc0: 2020 2066 2245 706f 6368 205b 7b65 706f     f"Epoch [{epo
+00002fd0: 6368 7d2f 7b72 756e 2e63 6f6e 6669 672e  ch}/{run.config.
+00002fe0: 6e75 6d5f 6570 6f63 6873 7d5d 2c20 4974  num_epochs}], It
+00002ff0: 6572 6174 696f 6e20 5b7b 6974 6572 202b  eration [{iter +
+00003000: 2031 7d2f 7b6c 656e 2874 7261 696e 5f6c   1}/{len(train_l
+00003010: 6f61 6465 7229 7d5d 2c20 4c6f 7373 3a20  oader)}], Loss: 
+00003020: 7b6c 6f73 732e 6974 656d 2829 7d22 0a20  {loss.item()}". 
+00003030: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00003040: 2020 2020 2020 2020 2020 6966 2069 7465            if ite
+00003050: 7220 2520 3230 203d 3d20 303a 0a20 2020  r % 20 == 0:.   
+00003060: 2020 2020 2020 2020 2020 2020 2073 7761               swa
+00003070: 6e6c 6162 2e6c 6f67 287b 2274 7261 696e  nlab.log({"train
+00003080: 2f6c 6f73 7322 3a20 6c6f 7373 2e69 7465  /loss": loss.ite
+00003090: 6d28 297d 2c20 7374 6570 3d28 6570 6f63  m()}, step=(epoc
+000030a0: 6820 2d20 3129 202a 206c 656e 2874 7261  h - 1) * len(tra
+000030b0: 696e 5f6c 6f61 6465 7229 202b 2069 7465  in_loader) + ite
+000030c0: 7229 0a0a 2020 2020 2020 2020 2320 e6af  r)..        # ..
+000030d0: 8f34 e4b8 aa65 706f 6368 e9aa 8ce8 af81  .4...epoch......
+000030e0: e4b8 80e6 aca1 0a20 2020 2020 2020 2069  .......        i
+000030f0: 6620 6570 6f63 6820 2520 3220 3d3d 2030  f epoch % 2 == 0
+00003100: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+00003110: 6465 6c2e 6576 616c 2829 0a20 2020 2020  del.eval().     
+00003120: 2020 2020 2020 2063 6f72 7265 6374 203d         correct =
+00003130: 2030 0a20 2020 2020 2020 2020 2020 2074   0.            t
+00003140: 6f74 616c 203d 2030 0a20 2020 2020 2020  otal = 0.       
+00003150: 2020 2020 2077 6974 6820 746f 7263 682e       with torch.
+00003160: 6e6f 5f67 7261 6428 293a 0a20 2020 2020  no_grad():.     
+00003170: 2020 2020 2020 2020 2020 2066 6f72 2062             for b
+00003180: 6174 6368 2069 6e20 7661 6c5f 6c6f 6164  atch in val_load
+00003190: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+000031a0: 2020 2020 2020 2020 782c 2079 203d 2062          x, y = b
+000031b0: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
+000031c0: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+000031d0: 3d20 6d6f 6465 6c28 7829 0a20 2020 2020  = model(x).     
+000031e0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+000031f0: 2c20 7072 6564 6963 7465 6420 3d20 746f  , predicted = to
+00003200: 7263 682e 6d61 7828 6f75 7470 7574 2c20  rch.max(output, 
+00003210: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+00003220: 2020 2020 2020 2074 6f74 616c 202b 3d20         total += 
+00003230: 792e 7369 7a65 2830 290a 2020 2020 2020  y.size(0).      
+00003240: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00003250: 7272 6563 7420 2b3d 2028 7072 6564 6963  rrect += (predic
+00003260: 7465 6420 3d3d 2079 292e 7375 6d28 292e  ted == y).sum().
+00003270: 6974 656d 2829 0a0a 2020 2020 2020 2020  item()..        
+00003280: 2020 2020 6163 6375 7261 6379 203d 2063      accuracy = c
+00003290: 6f72 7265 6374 202f 2074 6f74 616c 0a20  orrect / total. 
+000032a0: 2020 2020 2020 2020 2020 2073 7761 6e6c             swanl
+000032b0: 6162 2e6c 6f67 287b 2276 616c 2f61 6363  ab.log({"val/acc
+000032c0: 7572 6163 7922 3a20 6163 6375 7261 6379  uracy": accuracy
+000032d0: 7d29 0a60 6060 0a0a 3c2f 6465 7461 696c  }).```..</detail
+000032e0: 733e 0a0a 5b42 4552 542d 494d 4442 5d28  s>..[BERT-IMDB](
+000032f0: 6874 7470 733a 2f2f 646f 6373 2e73 7761  https://docs.swa
+00003300: 6e6c 6162 2e63 6e2f 7a68 2f65 7861 6d70  nlab.cn/zh/examp
+00003310: 6c65 732f 6265 7274 2e68 746d 6c29 0a0a  les/bert.html)..
+00003320: 5b59 4f4c 4f5d 2868 7474 7073 3a2f 2f64  [YOLO](https://d
+00003330: 6f63 732e 7377 616e 6c61 622e 636e 2f7a  ocs.swanlab.cn/z
+00003340: 682f 6578 616d 706c 6573 2f79 6f6c 6f2e  h/examples/yolo.
+00003350: 6874 6d6c 290a 0a3c 6272 3e0a 0a23 2320  html)..<br>..## 
+00003360: f09f 92bb 2053 656c 662d 686f 7374 6564  .... Self-hosted
+00003370: 0a0a 5468 6520 636f 6d6d 756e 6974 7920  ..The community 
+00003380: 6564 6974 696f 6e20 7375 7070 6f72 7473  edition supports
+00003390: 206f 6666 6c69 6e65 2076 6965 7769 6e67   offline viewing
+000033a0: 206f 6620 5377 616e 4c61 6220 6461 7368   of SwanLab dash
+000033b0: 626f 6172 6473 2e0a 0a23 2323 204f 6666  boards...### Off
+000033c0: 6c69 6e65 2045 7870 6572 696d 656e 7420  line Experiment 
+000033d0: 5472 6163 6b69 6e67 0a0a 5365 7420 7468  Tracking..Set th
+000033e0: 6520 7061 7261 6d65 7465 7273 2060 6c6f  e parameters `lo
+000033f0: 6769 7260 2061 6e64 2060 6d6f 6465 6020  gir` and `mode` 
+00003400: 696e 2073 7761 6e6c 6162 2e69 6e69 7420  in swanlab.init 
+00003410: 746f 2074 7261 636b 2065 7870 6572 696d  to track experim
+00003420: 656e 7473 206f 6666 6c69 6e65 3a0a 0a60  ents offline:..`
+00003430: 6060 7079 7468 6f6e 0a2e 2e2e 0a0a 7377  ``python......sw
+00003440: 616e 6c61 622e 696e 6974 280a 2020 2020  anlab.init(.    
+00003450: 6c6f 6764 6972 3d27 2e2f 6c6f 6773 272c  logdir='./logs',
+00003460: 0a20 2020 206d 6f64 653d 276c 6f63 616c  .    mode='local
+00003470: 272c 0a29 0a0a 2e2e 2e0a 6060 600a 0a2d  ',.)......```..-
+00003480: 2054 6865 2070 6172 616d 6574 6572 2060   The parameter `
+00003490: 6d6f 6465 6020 6973 2073 6574 2074 6f20  mode` is set to 
+000034a0: 606c 6f63 616c 602c 2077 6869 6368 2064  `local`, which d
+000034b0: 6973 6162 6c65 7320 7379 6e63 6872 6f6e  isables synchron
+000034c0: 697a 696e 6720 7468 6520 6578 7065 7269  izing the experi
+000034d0: 6d65 6e74 2074 6f20 7468 6520 636c 6f75  ment to the clou
+000034e0: 642e 0a0a 2d20 5468 6520 7365 7474 696e  d...- The settin
+000034f0: 6720 6f66 2074 6865 2070 6172 616d 6574  g of the paramet
+00003500: 6572 2060 6c6f 6764 6972 6020 6973 206f  er `logdir` is o
+00003510: 7074 696f 6e61 6c2c 2061 6e64 2069 7420  ptional, and it 
+00003520: 7370 6563 6966 6965 7320 7468 6520 6c6f  specifies the lo
+00003530: 6361 7469 6f6e 2066 6f72 2073 6176 696e  cation for savin
+00003540: 6720 5377 616e 4c61 6220 6c6f 6720 6669  g SwanLab log fi
+00003550: 6c65 7320 2862 790a 2020 6465 6661 756c  les (by.  defaul
+00003560: 7420 7361 7665 6420 696e 2074 6865 2060  t saved in the `
+00003570: 7377 616e 6c6f 6760 2066 6f6c 6465 7229  swanlog` folder)
+00003580: 2e0a 0a2d 204c 6f67 2066 696c 6573 2077  ...- Log files w
+00003590: 696c 6c20 6265 2063 7265 6174 6564 2061  ill be created a
+000035a0: 6e64 2075 7064 6174 6564 2064 7572 696e  nd updated durin
+000035b0: 6720 7472 6163 6b69 6e67 206f 6620 6578  g tracking of ex
+000035c0: 7065 7269 6d65 6e74 732c 2061 6e64 206c  periments, and l
+000035d0: 6175 6e63 6869 6e67 206f 6666 6c69 6e65  aunching offline
+000035e0: 2064 6173 6862 6f61 7264 7320 7769 6c6c   dashboards will
+000035f0: 2061 6c73 6f20 6265 0a20 2062 6173 6564   also be.  based
+00003600: 206f 6e20 7468 6573 6520 6c6f 6720 6669   on these log fi
+00003610: 6c65 732e 0a0a 4f74 6865 7220 7061 7274  les...Other part
+00003620: 7320 6172 6520 636f 6d70 6c65 7465 6c79  s are completely
+00003630: 2063 6f6e 7369 7374 656e 7420 7769 7468   consistent with
+00003640: 2063 6c6f 7564 2075 7361 6765 2e0a 0a23   cloud usage...#
+00003650: 2323 204f 7065 6e20 4f66 666c 696e 6520  ## Open Offline 
+00003660: 426f 6172 640a 0a4f 7065 6e20 7468 6520  Board..Open the 
+00003670: 7465 726d 696e 616c 2061 6e64 2075 7365  terminal and use
+00003680: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00003690: 6f6d 6d61 6e64 2074 6f20 6f70 656e 2061  ommand to open a
+000036a0: 2053 7761 6e4c 6162 2064 6173 6862 6f61   SwanLab dashboa
+000036b0: 7264 3a0a 0a60 6060 6261 7368 0a73 7761  rd:..```bash.swa
+000036c0: 6e6c 6162 2077 6174 6368 202d 6c20 2e2f  nlab watch -l ./
+000036d0: 6c6f 6773 0a60 6060 0a0a 4166 7465 7220  logs.```..After 
+000036e0: 7468 6520 6f70 6572 6174 696f 6e20 6973  the operation is
+000036f0: 2063 6f6d 706c 6574 6564 2c20 5377 616e   completed, Swan
+00003700: 4c61 6220 7769 6c6c 2070 726f 7669 6465  Lab will provide
+00003710: 2079 6f75 2077 6974 6820 6120 6c6f 6361   you with a loca
+00003720: 6c20 5552 4c20 6c69 6e6b 2028 6465 6661  l URL link (defa
+00003730: 756c 740a 6973 205b 6874 7470 3a2f 2f31  ult.is [http://1
+00003740: 3237 2e30 2e30 2e31 3a35 3039 325d 2868  27.0.0.1:5092](h
+00003750: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
+00003760: 3530 3932 2929 2e0a 0a56 6973 6974 2074  5092))...Visit t
+00003770: 6869 7320 6c69 6e6b 2074 6f20 7669 6577  his link to view
+00003780: 2074 6865 2065 7870 6572 696d 656e 7420   the experiment 
+00003790: 6f66 666c 696e 6520 696e 2074 6865 2062  offline in the b
+000037a0: 726f 7773 6572 2064 6173 6862 6f61 7264  rowser dashboard
+000037b0: 2e0a 0a3c 6272 3e0a 0a23 2320 f09f 9a97  ...<br>..## ....
+000037c0: 2049 6e74 6567 7261 7469 6f6e 0a0a 436f   Integration..Co
+000037d0: 6d62 696e 6520 796f 7572 2066 6176 6f72  mbine your favor
+000037e0: 6974 6520 6672 616d 6577 6f72 6b20 7769  ite framework wi
+000037f0: 7468 0a53 7761 6e4c 6162 2c20 5b4d 6f72  th.SwanLab, [Mor
+00003800: 6520 496e 7465 6772 6174 696f 6e5d 2868  e Integration](h
+00003810: 7474 7073 3a2f 2f64 6f63 732e 7377 616e  ttps://docs.swan
+00003820: 6c61 622e 636e 2f7a 682f 6775 6964 655f  lab.cn/zh/guide_
+00003830: 636c 6f75 642f 696e 7465 6772 6174 696f  cloud/integratio
+00003840: 6e2f 696e 7465 6772 6174 696f 6e2d 7079  n/integration-py
+00003850: 746f 7263 682d 6c69 6768 746e 696e 672e  torch-lightning.
+00003860: 6874 6d6c 292e 0a0a 3c64 6574 6169 6c73  html)...<details
+00003870: 3e0a 2020 3c73 756d 6d61 7279 3e0a 2020  >.  <summary>.  
+00003880: 2020 3c73 7472 6f6e 673e e29a a1ef b88f    <strong>......
+00003890: 2050 7954 6f72 6368 204c 6967 6874 6e69   PyTorch Lightni
+000038a0: 6e67 3c2f 7374 726f 6e67 3e0a 2020 3c2f  ng</strong>.  </
+000038b0: 7375 6d6d 6172 793e 0a20 203c 6272 3e0a  summary>.  <br>.
+000038c0: 0a43 7265 6174 6520 616e 2069 6e73 7461  .Create an insta
+000038d0: 6e63 6520 7573 696e 6720 6053 7761 6e4c  nce using `SwanL
+000038e0: 6162 4c6f 6767 6572 6020 616e 6420 7061  abLogger` and pa
+000038f0: 7373 2069 7420 696e 746f 2074 6865 2060  ss it into the `
+00003900: 6c6f 6767 6572 6020 7061 7261 6d65 7465  logger` paramete
+00003910: 7220 6f66 2060 5472 6169 6e65 7260 2074  r of `Trainer` t
+00003920: 6f20 656e 6162 6c65 2053 7761 6e4c 6162  o enable SwanLab
+00003930: 2074 6f0a 7265 636f 7264 2074 7261 696e   to.record train
+00003940: 696e 6720 6d65 7472 6963 732e 0a0a 6060  ing metrics...``
+00003950: 6070 7974 686f 6e0a 6672 6f6d 2073 7761  `python.from swa
+00003960: 6e6c 6162 2e69 6e74 6567 7261 7469 6f6e  nlab.integration
+00003970: 2e70 7974 6f72 6368 5f6c 6967 6874 6e69  .pytorch_lightni
+00003980: 6e67 2069 6d70 6f72 7420 5377 616e 4c61  ng import SwanLa
+00003990: 624c 6f67 6765 720a 696d 706f 7274 2069  bLogger.import i
+000039a0: 6d70 6f72 746c 6962 2e75 7469 6c0a 696d  mportlib.util.im
+000039b0: 706f 7274 206f 730a 696d 706f 7274 2070  port os.import p
+000039c0: 7974 6f72 6368 5f6c 6967 6874 6e69 6e67  ytorch_lightning
+000039d0: 2061 7320 706c 0a66 726f 6d20 746f 7263   as pl.from torc
+000039e0: 6820 696d 706f 7274 206e 6e2c 206f 7074  h import nn, opt
+000039f0: 696d 2c20 7574 696c 730a 6672 6f6d 2074  im, utils.from t
+00003a00: 6f72 6368 7669 7369 6f6e 2e64 6174 6173  orchvision.datas
+00003a10: 6574 7320 696d 706f 7274 204d 4e49 5354  ets import MNIST
+00003a20: 0a66 726f 6d20 746f 7263 6876 6973 696f  .from torchvisio
+00003a30: 6e2e 7472 616e 7366 6f72 6d73 2069 6d70  n.transforms imp
+00003a40: 6f72 7420 546f 5465 6e73 6f72 0a0a 656e  ort ToTensor..en
+00003a50: 636f 6465 7220 3d20 6e6e 2e53 6571 7565  coder = nn.Seque
+00003a60: 6e74 6961 6c28 6e6e 2e4c 696e 6561 7228  ntial(nn.Linear(
+00003a70: 3238 202a 2032 382c 2031 3238 292c 206e  28 * 28, 128), n
+00003a80: 6e2e 5265 4c55 2829 2c20 6e6e 2e4c 696e  n.ReLU(), nn.Lin
+00003a90: 6561 7228 3132 382c 2033 2929 0a64 6563  ear(128, 3)).dec
+00003aa0: 6f64 6572 203d 206e 6e2e 5365 7175 656e  oder = nn.Sequen
+00003ab0: 7469 616c 286e 6e2e 4c69 6e65 6172 2833  tial(nn.Linear(3
+00003ac0: 2c20 3132 3829 2c20 6e6e 2e52 654c 5528  , 128), nn.ReLU(
+00003ad0: 292c 206e 6e2e 4c69 6e65 6172 2831 3238  ), nn.Linear(128
+00003ae0: 2c20 3238 202a 2032 3829 290a 0a0a 636c  , 28 * 28))...cl
+00003af0: 6173 7320 4c69 7441 7574 6f45 6e63 6f64  ass LitAutoEncod
+00003b00: 6572 2870 6c2e 4c69 6768 746e 696e 674d  er(pl.LightningM
+00003b10: 6f64 756c 6529 3a0a 2020 2020 6465 6620  odule):.    def 
+00003b20: 5f5f 696e 6974 5f5f 2873 656c 662c 2065  __init__(self, e
+00003b30: 6e63 6f64 6572 2c20 6465 636f 6465 7229  ncoder, decoder)
+00003b40: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+00003b50: 292e 5f5f 696e 6974 5f5f 2829 0a20 2020  ).__init__().   
+00003b60: 2020 2020 2073 656c 662e 656e 636f 6465       self.encode
+00003b70: 7220 3d20 656e 636f 6465 720a 2020 2020  r = encoder.    
+00003b80: 2020 2020 7365 6c66 2e64 6563 6f64 6572      self.decoder
+00003b90: 203d 2064 6563 6f64 6572 0a0a 2020 2020   = decoder..    
+00003ba0: 6465 6620 7472 6169 6e69 6e67 5f73 7465  def training_ste
+00003bb0: 7028 7365 6c66 2c20 6261 7463 682c 2062  p(self, batch, b
+00003bc0: 6174 6368 5f69 6478 293a 0a20 2020 2020  atch_idx):.     
+00003bd0: 2020 2023 2074 7261 696e 696e 675f 7374     # training_st
+00003be0: 6570 2064 6566 696e 6573 2074 6865 2074  ep defines the t
+00003bf0: 7261 696e 206c 6f6f 702e 0a20 2020 2020  rain loop..     
+00003c00: 2020 2023 2069 7420 6973 2069 6e64 6570     # it is indep
+00003c10: 656e 6465 6e74 206f 6620 666f 7277 6172  endent of forwar
+00003c20: 640a 2020 2020 2020 2020 782c 2079 203d  d.        x, y =
+00003c30: 2062 6174 6368 0a20 2020 2020 2020 2078   batch.        x
+00003c40: 203d 2078 2e76 6965 7728 782e 7369 7a65   = x.view(x.size
+00003c50: 2830 292c 202d 3129 0a20 2020 2020 2020  (0), -1).       
+00003c60: 207a 203d 2073 656c 662e 656e 636f 6465   z = self.encode
+00003c70: 7228 7829 0a20 2020 2020 2020 2078 5f68  r(x).        x_h
+00003c80: 6174 203d 2073 656c 662e 6465 636f 6465  at = self.decode
+00003c90: 7228 7a29 0a20 2020 2020 2020 206c 6f73  r(z).        los
+00003ca0: 7320 3d20 6e6e 2e66 756e 6374 696f 6e61  s = nn.functiona
+00003cb0: 6c2e 6d73 655f 6c6f 7373 2878 5f68 6174  l.mse_loss(x_hat
+00003cc0: 2c20 7829 0a20 2020 2020 2020 2023 204c  , x).        # L
+00003cd0: 6f67 6769 6e67 2074 6f20 5465 6e73 6f72  ogging to Tensor
+00003ce0: 426f 6172 6420 2869 6620 696e 7374 616c  Board (if instal
+00003cf0: 6c65 6429 2062 7920 6465 6661 756c 740a  led) by default.
+00003d00: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00003d10: 2822 7472 6169 6e5f 6c6f 7373 222c 206c  ("train_loss", l
+00003d20: 6f73 7329 0a20 2020 2020 2020 2072 6574  oss).        ret
+00003d30: 7572 6e20 6c6f 7373 0a0a 2020 2020 6465  urn loss..    de
+00003d40: 6620 7465 7374 5f73 7465 7028 7365 6c66  f test_step(self
+00003d50: 2c20 6261 7463 682c 2062 6174 6368 5f69  , batch, batch_i
+00003d60: 6478 293a 0a20 2020 2020 2020 2023 2074  dx):.        # t
+00003d70: 6573 745f 7374 6570 2064 6566 696e 6573  est_step defines
+00003d80: 2074 6865 2074 6573 7420 6c6f 6f70 2e0a   the test loop..
+00003d90: 2020 2020 2020 2020 2320 6974 2069 7320          # it is 
+00003da0: 696e 6465 7065 6e64 656e 7420 6f66 2066  independent of f
+00003db0: 6f72 7761 7264 0a20 2020 2020 2020 2078  orward.        x
+00003dc0: 2c20 7920 3d20 6261 7463 680a 2020 2020  , y = batch.    
+00003dd0: 2020 2020 7820 3d20 782e 7669 6577 2878      x = x.view(x
+00003de0: 2e73 697a 6528 3029 2c20 2d31 290a 2020  .size(0), -1).  
+00003df0: 2020 2020 2020 7a20 3d20 7365 6c66 2e65        z = self.e
+00003e00: 6e63 6f64 6572 2878 290a 2020 2020 2020  ncoder(x).      
+00003e10: 2020 785f 6861 7420 3d20 7365 6c66 2e64    x_hat = self.d
+00003e20: 6563 6f64 6572 287a 290a 2020 2020 2020  ecoder(z).      
+00003e30: 2020 6c6f 7373 203d 206e 6e2e 6675 6e63    loss = nn.func
+00003e40: 7469 6f6e 616c 2e6d 7365 5f6c 6f73 7328  tional.mse_loss(
+00003e50: 785f 6861 742c 2078 290a 2020 2020 2020  x_hat, x).      
+00003e60: 2020 2320 4c6f 6767 696e 6720 746f 2054    # Logging to T
+00003e70: 656e 736f 7242 6f61 7264 2028 6966 2069  ensorBoard (if i
+00003e80: 6e73 7461 6c6c 6564 2920 6279 2064 6566  nstalled) by def
+00003e90: 6175 6c74 0a20 2020 2020 2020 2073 656c  ault.        sel
+00003ea0: 662e 6c6f 6728 2274 6573 745f 6c6f 7373  f.log("test_loss
+00003eb0: 222c 206c 6f73 7329 0a20 2020 2020 2020  ", loss).       
+00003ec0: 2072 6574 7572 6e20 6c6f 7373 0a0a 2020   return loss..  
+00003ed0: 2020 6465 6620 636f 6e66 6967 7572 655f    def configure_
+00003ee0: 6f70 7469 6d69 7a65 7273 2873 656c 6629  optimizers(self)
+00003ef0: 3a0a 2020 2020 2020 2020 6f70 7469 6d69  :.        optimi
+00003f00: 7a65 7220 3d20 6f70 7469 6d2e 4164 616d  zer = optim.Adam
+00003f10: 2873 656c 662e 7061 7261 6d65 7465 7273  (self.parameters
+00003f20: 2829 2c20 6c72 3d31 652d 3329 0a20 2020  (), lr=1e-3).   
+00003f30: 2020 2020 2072 6574 7572 6e20 6f70 7469       return opti
+00003f40: 6d69 7a65 720a 0a0a 2320 696e 6974 2074  mizer...# init t
+00003f50: 6865 2061 7574 6f65 6e63 6f64 6572 0a61  he autoencoder.a
+00003f60: 7574 6f65 6e63 6f64 6572 203d 204c 6974  utoencoder = Lit
+00003f70: 4175 746f 456e 636f 6465 7228 656e 636f  AutoEncoder(enco
+00003f80: 6465 722c 2064 6563 6f64 6572 290a 0a23  der, decoder)..#
+00003f90: 2073 6574 7570 2064 6174 610a 6461 7461   setup data.data
+00003fa0: 7365 7420 3d20 4d4e 4953 5428 6f73 2e67  set = MNIST(os.g
+00003fb0: 6574 6377 6428 292c 2074 7261 696e 3d54  etcwd(), train=T
+00003fc0: 7275 652c 2064 6f77 6e6c 6f61 643d 5472  rue, download=Tr
+00003fd0: 7565 2c20 7472 616e 7366 6f72 6d3d 546f  ue, transform=To
+00003fe0: 5465 6e73 6f72 2829 290a 7472 6169 6e5f  Tensor()).train_
+00003ff0: 6461 7461 7365 742c 2076 616c 5f64 6174  dataset, val_dat
+00004000: 6173 6574 203d 2075 7469 6c73 2e64 6174  aset = utils.dat
+00004010: 612e 7261 6e64 6f6d 5f73 706c 6974 2864  a.random_split(d
+00004020: 6174 6173 6574 2c20 5b35 3530 3030 2c20  ataset, [55000, 
+00004030: 3530 3030 5d29 0a74 6573 745f 6461 7461  5000]).test_data
+00004040: 7365 7420 3d20 4d4e 4953 5428 6f73 2e67  set = MNIST(os.g
+00004050: 6574 6377 6428 292c 2074 7261 696e 3d46  etcwd(), train=F
+00004060: 616c 7365 2c20 646f 776e 6c6f 6164 3d54  alse, download=T
+00004070: 7275 652c 2074 7261 6e73 666f 726d 3d54  rue, transform=T
+00004080: 6f54 656e 736f 7228 2929 0a0a 7472 6169  oTensor())..trai
+00004090: 6e5f 6c6f 6164 6572 203d 2075 7469 6c73  n_loader = utils
+000040a0: 2e64 6174 612e 4461 7461 4c6f 6164 6572  .data.DataLoader
+000040b0: 2874 7261 696e 5f64 6174 6173 6574 290a  (train_dataset).
+000040c0: 7661 6c5f 6c6f 6164 6572 203d 2075 7469  val_loader = uti
+000040d0: 6c73 2e64 6174 612e 4461 7461 4c6f 6164  ls.data.DataLoad
+000040e0: 6572 2876 616c 5f64 6174 6173 6574 290a  er(val_dataset).
+000040f0: 7465 7374 5f6c 6f61 6465 7220 3d20 7574  test_loader = ut
+00004100: 696c 732e 6461 7461 2e44 6174 614c 6f61  ils.data.DataLoa
+00004110: 6465 7228 7465 7374 5f64 6174 6173 6574  der(test_dataset
+00004120: 290a 0a73 7761 6e6c 6162 5f6c 6f67 6765  )..swanlab_logge
+00004130: 7220 3d20 5377 616e 4c61 624c 6f67 6765  r = SwanLabLogge
+00004140: 7228 0a20 2020 2070 726f 6a65 6374 3d22  r(.    project="
+00004150: 7377 616e 6c61 625f 6578 616d 706c 6522  swanlab_example"
+00004160: 2c0a 2020 2020 6578 7065 7269 6d65 6e74  ,.    experiment
+00004170: 5f6e 616d 653d 2265 7861 6d70 6c65 5f65  _name="example_e
+00004180: 7870 6572 696d 656e 7422 2c0a 2020 2020  xperiment",.    
+00004190: 636c 6f75 643d 4661 6c73 652c 0a29 0a0a  cloud=False,.)..
+000041a0: 7472 6169 6e65 7220 3d20 706c 2e54 7261  trainer = pl.Tra
+000041b0: 696e 6572 286c 696d 6974 5f74 7261 696e  iner(limit_train
+000041c0: 5f62 6174 6368 6573 3d31 3030 2c20 6d61  _batches=100, ma
+000041d0: 785f 6570 6f63 6873 3d35 2c20 6c6f 6767  x_epochs=5, logg
+000041e0: 6572 3d73 7761 6e6c 6162 5f6c 6f67 6765  er=swanlab_logge
+000041f0: 7229 0a0a 7472 6169 6e65 722e 6669 7428  r)..trainer.fit(
+00004200: 6d6f 6465 6c3d 6175 746f 656e 636f 6465  model=autoencode
+00004210: 722c 2074 7261 696e 5f64 6174 616c 6f61  r, train_dataloa
+00004220: 6465 7273 3d74 7261 696e 5f6c 6f61 6465  ders=train_loade
+00004230: 722c 2076 616c 5f64 6174 616c 6f61 6465  r, val_dataloade
+00004240: 7273 3d76 616c 5f6c 6f61 6465 7229 0a74  rs=val_loader).t
+00004250: 7261 696e 6572 2e74 6573 7428 6461 7461  rainer.test(data
+00004260: 6c6f 6164 6572 733d 7465 7374 5f6c 6f61  loaders=test_loa
+00004270: 6465 7229 0a0a 6060 600a 0a3c 2f64 6574  der)..```..</det
+00004280: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
+00004290: 0a3c 7375 6d6d 6172 793e 0a20 203c 7374  .<summary>.  <st
+000042a0: 726f 6e67 3e20 f09f a497 4875 6767 696e  rong> ....Huggin
+000042b0: 6746 6163 6520 5472 616e 7366 6f72 6d65  gFace Transforme
+000042c0: 7273 3c2f 7374 726f 6e67 3e0a 3c2f 7375  rs</strong>.</su
+000042d0: 6d6d 6172 793e 0a0a 3c62 723e 0a0a 4372  mmary>..<br>..Cr
+000042e0: 6561 7465 2061 6e20 696e 7374 616e 6365  eate an instance
+000042f0: 2075 7369 6e67 2060 5377 616e 4c61 6243   using `SwanLabC
+00004300: 616c 6c62 6163 6b60 2061 6e64 2070 6173  allback` and pas
+00004310: 7320 6974 2069 6e74 6f20 7468 6520 6063  s it into the `c
+00004320: 616c 6c62 6163 6b73 6020 7061 7261 6d65  allbacks` parame
+00004330: 7465 7220 6f66 2060 5472 6169 6e65 7260  ter of `Trainer`
+00004340: 2074 6f20 656e 6162 6c65 2053 7761 6e4c   to enable SwanL
+00004350: 6162 2074 6f0a 7265 636f 7264 2074 7261  ab to.record tra
+00004360: 696e 696e 6720 6d65 7472 6963 732e 0a0a  ining metrics...
+00004370: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00004380: 2065 7661 6c75 6174 650a 696d 706f 7274   evaluate.import
+00004390: 206e 756d 7079 2061 7320 6e70 0a69 6d70   numpy as np.imp
+000043a0: 6f72 7420 7377 616e 6c61 620a 6672 6f6d  ort swanlab.from
+000043b0: 2073 7761 6e6c 6162 2e69 6e74 6567 7261   swanlab.integra
+000043c0: 7469 6f6e 2e68 7567 6769 6e67 6661 6365  tion.huggingface
+000043d0: 2069 6d70 6f72 7420 5377 616e 4c61 6243   import SwanLabC
+000043e0: 616c 6c62 6163 6b0a 6672 6f6d 2064 6174  allback.from dat
+000043f0: 6173 6574 7320 696d 706f 7274 206c 6f61  asets import loa
+00004400: 645f 6461 7461 7365 740a 6672 6f6d 2074  d_dataset.from t
+00004410: 7261 6e73 666f 726d 6572 7320 696d 706f  ransformers impo
+00004420: 7274 2041 7574 6f4d 6f64 656c 466f 7253  rt AutoModelForS
+00004430: 6571 7565 6e63 6543 6c61 7373 6966 6963  equenceClassific
+00004440: 6174 696f 6e2c 2041 7574 6f54 6f6b 656e  ation, AutoToken
+00004450: 697a 6572 2c20 5472 6169 6e65 722c 2054  izer, Trainer, T
+00004460: 7261 696e 696e 6741 7267 756d 656e 7473  rainingArguments
+00004470: 0a0a 0a64 6566 2074 6f6b 656e 697a 655f  ...def tokenize_
+00004480: 6675 6e63 7469 6f6e 2865 7861 6d70 6c65  function(example
+00004490: 7329 3a0a 2020 2020 7265 7475 726e 2074  s):.    return t
+000044a0: 6f6b 656e 697a 6572 2865 7861 6d70 6c65  okenizer(example
+000044b0: 735b 2274 6578 7422 5d2c 2070 6164 6469  s["text"], paddi
+000044c0: 6e67 3d22 6d61 785f 6c65 6e67 7468 222c  ng="max_length",
+000044d0: 2074 7275 6e63 6174 696f 6e3d 5472 7565   truncation=True
+000044e0: 290a 0a0a 6465 6620 636f 6d70 7574 655f  )...def compute_
+000044f0: 6d65 7472 6963 7328 6576 616c 5f70 7265  metrics(eval_pre
+00004500: 6429 3a0a 2020 2020 6c6f 6769 7473 2c20  d):.    logits, 
+00004510: 6c61 6265 6c73 203d 2065 7661 6c5f 7072  labels = eval_pr
+00004520: 6564 0a20 2020 2070 7265 6469 6374 696f  ed.    predictio
+00004530: 6e73 203d 206e 702e 6172 676d 6178 286c  ns = np.argmax(l
+00004540: 6f67 6974 732c 2061 7869 733d 2d31 290a  ogits, axis=-1).
+00004550: 2020 2020 7265 7475 726e 206d 6574 7269      return metri
+00004560: 632e 636f 6d70 7574 6528 7072 6564 6963  c.compute(predic
+00004570: 7469 6f6e 733d 7072 6564 6963 7469 6f6e  tions=prediction
+00004580: 732c 2072 6566 6572 656e 6365 733d 6c61  s, references=la
+00004590: 6265 6c73 290a 0a0a 6461 7461 7365 7420  bels)...dataset 
+000045a0: 3d20 6c6f 6164 5f64 6174 6173 6574 2822  = load_dataset("
+000045b0: 7965 6c70 5f72 6576 6965 775f 6675 6c6c  yelp_review_full
+000045c0: 2229 0a0a 746f 6b65 6e69 7a65 7220 3d20  ")..tokenizer = 
+000045d0: 4175 746f 546f 6b65 6e69 7a65 722e 6672  AutoTokenizer.fr
+000045e0: 6f6d 5f70 7265 7472 6169 6e65 6428 2262  om_pretrained("b
+000045f0: 6572 742d 6261 7365 2d63 6173 6564 2229  ert-base-cased")
+00004600: 0a0a 746f 6b65 6e69 7a65 645f 6461 7461  ..tokenized_data
+00004610: 7365 7473 203d 2064 6174 6173 6574 2e6d  sets = dataset.m
+00004620: 6170 2874 6f6b 656e 697a 655f 6675 6e63  ap(tokenize_func
+00004630: 7469 6f6e 2c20 6261 7463 6865 643d 5472  tion, batched=Tr
+00004640: 7565 290a 0a73 6d61 6c6c 5f74 7261 696e  ue)..small_train
+00004650: 5f64 6174 6173 6574 203d 2074 6f6b 656e  _dataset = token
+00004660: 697a 6564 5f64 6174 6173 6574 735b 2274  ized_datasets["t
+00004670: 7261 696e 225d 2e73 6875 6666 6c65 2873  rain"].shuffle(s
+00004680: 6565 643d 3432 292e 7365 6c65 6374 2872  eed=42).select(r
+00004690: 616e 6765 2831 3030 3029 290a 736d 616c  ange(1000)).smal
+000046a0: 6c5f 6576 616c 5f64 6174 6173 6574 203d  l_eval_dataset =
+000046b0: 2074 6f6b 656e 697a 6564 5f64 6174 6173   tokenized_datas
+000046c0: 6574 735b 2274 6573 7422 5d2e 7368 7566  ets["test"].shuf
+000046d0: 666c 6528 7365 6564 3d34 3229 2e73 656c  fle(seed=42).sel
+000046e0: 6563 7428 7261 6e67 6528 3130 3030 2929  ect(range(1000))
+000046f0: 0a0a 6d65 7472 6963 203d 2065 7661 6c75  ..metric = evalu
+00004700: 6174 652e 6c6f 6164 2822 6163 6375 7261  ate.load("accura
+00004710: 6379 2229 0a0a 6d6f 6465 6c20 3d20 4175  cy")..model = Au
+00004720: 746f 4d6f 6465 6c46 6f72 5365 7175 656e  toModelForSequen
+00004730: 6365 436c 6173 7369 6669 6361 7469 6f6e  ceClassification
+00004740: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+00004750: 2822 6265 7274 2d62 6173 652d 6361 7365  ("bert-base-case
+00004760: 6422 2c20 6e75 6d5f 6c61 6265 6c73 3d35  d", num_labels=5
+00004770: 290a 0a74 7261 696e 696e 675f 6172 6773  )..training_args
+00004780: 203d 2054 7261 696e 696e 6741 7267 756d   = TrainingArgum
+00004790: 656e 7473 280a 2020 2020 6f75 7470 7574  ents(.    output
+000047a0: 5f64 6972 3d22 7465 7374 5f74 7261 696e  _dir="test_train
+000047b0: 6572 222c 0a20 2020 2072 6570 6f72 745f  er",.    report_
+000047c0: 746f 3d22 6e6f 6e65 222c 0a20 2020 206e  to="none",.    n
+000047d0: 756d 5f74 7261 696e 5f65 706f 6368 733d  um_train_epochs=
+000047e0: 332c 0a20 2020 206c 6f67 6769 6e67 5f73  3,.    logging_s
+000047f0: 7465 7073 3d35 302c 0a29 0a0a 7377 616e  teps=50,.)..swan
+00004800: 6c61 625f 6361 6c6c 6261 636b 203d 2053  lab_callback = S
+00004810: 7761 6e4c 6162 4361 6c6c 6261 636b 2865  wanLabCallback(e
+00004820: 7870 6572 696d 656e 745f 6e61 6d65 3d22  xperiment_name="
+00004830: 5472 616e 7366 6f72 6d65 7273 5465 7374  TransformersTest
+00004840: 222c 2063 6c6f 7564 3d46 616c 7365 290a  ", cloud=False).
+00004850: 0a74 7261 696e 6572 203d 2054 7261 696e  .trainer = Train
+00004860: 6572 280a 2020 2020 6d6f 6465 6c3d 6d6f  er(.    model=mo
+00004870: 6465 6c2c 0a20 2020 2061 7267 733d 7472  del,.    args=tr
+00004880: 6169 6e69 6e67 5f61 7267 732c 0a20 2020  aining_args,.   
+00004890: 2074 7261 696e 5f64 6174 6173 6574 3d73   train_dataset=s
+000048a0: 6d61 6c6c 5f74 7261 696e 5f64 6174 6173  mall_train_datas
+000048b0: 6574 2c0a 2020 2020 6576 616c 5f64 6174  et,.    eval_dat
+000048c0: 6173 6574 3d73 6d61 6c6c 5f65 7661 6c5f  aset=small_eval_
+000048d0: 6461 7461 7365 742c 0a20 2020 2063 6f6d  dataset,.    com
+000048e0: 7075 7465 5f6d 6574 7269 6373 3d63 6f6d  pute_metrics=com
+000048f0: 7075 7465 5f6d 6574 7269 6373 2c0a 2020  pute_metrics,.  
+00004900: 2020 6361 6c6c 6261 636b 733d 5b73 7761    callbacks=[swa
+00004910: 6e6c 6162 5f63 616c 6c62 6163 6b5d 2c0a  nlab_callback],.
+00004920: 290a 0a74 7261 696e 6572 2e74 7261 696e  )..trainer.train
+00004930: 2829 0a60 6060 0a0a 3c2f 6465 7461 696c  ().```..</detail
+00004940: 733e 0a0a 3c64 6574 6169 6c73 3e0a 3c73  s>..<details>.<s
+00004950: 756d 6d61 7279 3e0a 2020 3c73 7472 6f6e  ummary>.  <stron
+00004960: 673e 204d 4d45 6e67 696e 6528 4d4d 4465  g> MMEngine(MMDe
+00004970: 7465 6374 696f 6e20 6574 632e 293c 2f73  tection etc.)</s
+00004980: 7472 6f6e 673e 0a3c 2f73 756d 6d61 7279  trong>.</summary
+00004990: 3e0a 3c62 723e 0a0a 496e 7465 6772 6174  >.<br>..Integrat
+000049a0: 6520 6053 7761 6e6c 6162 5669 7342 6163  e `SwanlabVisBac
+000049b0: 6b65 6e64 6020 696e 746f 204d 4d45 6e67  kend` into MMEng
+000049c0: 696e 6520 746f 2065 6e61 626c 6520 6175  ine to enable au
+000049d0: 746f 6d61 7469 6320 6c6f 6767 696e 6720  tomatic logging 
+000049e0: 6f66 2074 7261 696e 696e 6720 6d65 7472  of training metr
+000049f0: 6963 7320 6279 2053 7761 6e4c 6162 2e0a  ics by SwanLab..
+00004a00: 0a41 6464 2074 6865 2066 6f6c 6c6f 7769  .Add the followi
+00004a10: 6e67 2063 6f64 6520 736e 6970 7065 7420  ng code snippet 
+00004a20: 746f 2079 6f75 7220 4d4d 2063 6f6e 6669  to your MM confi
+00004a30: 6720 6669 6c65 2074 6f20 7374 6172 7420  g file to start 
+00004a40: 7472 6169 6e69 6e67 3a0a 0a60 6060 7079  training:..```py
+00004a50: 7468 6f6e 0a63 7573 746f 6d5f 696d 706f  thon.custom_impo
+00004a60: 7274 7320 3d20 6469 6374 2869 6d70 6f72  rts = dict(impor
+00004a70: 7473 3d5b 2273 7761 6e6c 6162 2e69 6e74  ts=["swanlab.int
+00004a80: 6567 7261 7469 6f6e 2e6d 6d65 6e67 696e  egration.mmengin
+00004a90: 6522 5d2c 2061 6c6c 6f77 5f66 6169 6c65  e"], allow_faile
+00004aa0: 645f 696d 706f 7274 733d 4661 6c73 6529  d_imports=False)
+00004ab0: 0a0a 7669 735f 6261 636b 656e 6473 203d  ..vis_backends =
+00004ac0: 205b 0a20 2020 2064 6963 7428 0a20 2020   [.    dict(.   
+00004ad0: 2020 2020 2074 7970 653d 2253 7761 6e6c       type="Swanl
+00004ae0: 6162 5669 7342 6163 6b65 6e64 222c 0a20  abVisBackend",. 
+00004af0: 2020 2020 2020 2073 6176 655f 6469 723d         save_dir=
+00004b00: 2272 756e 732f 7377 616e 6c61 6222 2c0a  "runs/swanlab",.
+00004b10: 2020 2020 2020 2020 696e 6974 5f6b 7761          init_kwa
+00004b20: 7267 733d 7b0a 2020 2020 2020 2020 2020  rgs={.          
+00004b30: 2020 2270 726f 6a65 6374 223a 2022 7377    "project": "sw
+00004b40: 616e 6c61 622d 6d6d 656e 6769 6e65 222c  anlab-mmengine",
+00004b50: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00004b60: 292c 0a5d 0a0a 7669 7375 616c 697a 6572  ),.]..visualizer
+00004b70: 203d 2064 6963 7428 0a20 2020 2074 7970   = dict(.    typ
+00004b80: 653d 2256 6973 7561 6c69 7a65 7222 2c0a  e="Visualizer",.
+00004b90: 2020 2020 7669 735f 6261 636b 656e 6473      vis_backends
+00004ba0: 3d76 6973 5f62 6163 6b65 6e64 732c 0a29  =vis_backends,.)
+00004bb0: 0a60 6060 0a3c 2f64 6574 6169 6c73 3e0a  .```.</details>.
+00004bc0: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
+00004bd0: 6172 793e 0a20 203c 7374 726f 6e67 3e20  ary>.  <strong> 
+00004be0: 556c 7472 616c 7974 6963 733c 2f73 7472  Ultralytics</str
+00004bf0: 6f6e 673e 0a3c 2f73 756d 6d61 7279 3e0a  ong>.</summary>.
+00004c00: 3c62 723e 0a0a 496e 7465 6772 6174 696e  <br>..Integratin
+00004c10: 6720 5377 616e 4c61 6220 696e 746f 2055  g SwanLab into U
+00004c20: 6c74 7261 6c79 7469 6373 2069 7320 7665  ltralytics is ve
+00004c30: 7279 2073 696d 706c 653b 2079 6f75 2063  ry simple; you c
+00004c40: 616e 2075 7365 2074 6865 2060 6164 645f  an use the `add_
+00004c50: 7377 616e 6c61 625f 6361 6c6c 6261 636b  swanlab_callback
+00004c60: 6020 6675 6e63 7469 6f6e 3a0a 0a60 6060  ` function:..```
+00004c70: 7079 7468 6f6e 0a66 726f 6d20 756c 7472  python.from ultr
+00004c80: 616c 7974 6963 7320 696d 706f 7274 2059  alytics import Y
+00004c90: 4f4c 4f0a 6672 6f6d 2073 7761 6e6c 6162  OLO.from swanlab
+00004ca0: 2e69 6e74 6567 7261 7469 6f6e 2e75 6c74  .integration.ult
+00004cb0: 7261 6c79 7469 6373 2069 6d70 6f72 7420  ralytics import 
+00004cc0: 6164 645f 7377 616e 6c61 625f 6361 6c6c  add_swanlab_call
+00004cd0: 6261 636b 0a0a 6d6f 6465 6c20 3d20 594f  back..model = YO
+00004ce0: 4c4f 2822 796f 6c6f 7638 6e2e 7961 6d6c  LO("yolov8n.yaml
+00004cf0: 2229 0a6d 6f64 656c 2e6c 6f61 6428 290a  ").model.load().
+00004d00: 0a61 6464 5f73 7761 6e6c 6162 5f63 616c  .add_swanlab_cal
+00004d10: 6c62 6163 6b28 6d6f 6465 6c29 0a0a 6d6f  lback(model)..mo
+00004d20: 6465 6c2e 7472 6169 6e28 0a20 2020 2064  del.train(.    d
+00004d30: 6174 613d 222e 2f63 6f63 6f2e 7961 6d6c  ata="./coco.yaml
+00004d40: 222c 0a20 2020 2065 706f 6368 733d 3530  ",.    epochs=50
+00004d50: 2c20 0a20 2020 2069 6d67 737a 3d33 3230  , .    imgsz=320
+00004d60: 2c0a 290a 6060 600a 0a3c 2f64 6574 6169  ,.).```..</detai
+00004d70: 6c73 3e0a 0a0a 0a3c 6272 3e0a 0a23 2320  ls>....<br>..## 
+00004d80: f09f 869a 2043 6f6d 7061 7269 736f 6e20  .... Comparison 
+00004d90: 7769 7468 2066 616d 696c 6961 7220 746f  with familiar to
+00004da0: 6f6c 730a 0a23 2323 2054 656e 736f 7262  ols..### Tensorb
+00004db0: 6f61 7264 2076 7320 5377 616e 4c61 620a  oard vs SwanLab.
+00004dc0: 0a2d 202a 2ae2 9881 efb8 8f20 4f6e 6c69  .- **...... Onli
+00004dd0: 6e65 2055 7361 6765 2053 7570 706f 7274  ne Usage Support
+00004de0: 2a2a 3a0a 2020 5769 7468 2053 7761 6e4c  **:.  With SwanL
+00004df0: 6162 2c20 7472 6169 6e69 6e67 2065 7870  ab, training exp
+00004e00: 6572 696d 656e 7473 2063 616e 2062 6520  eriments can be 
+00004e10: 636f 6e76 656e 6965 6e74 6c79 2073 796e  conveniently syn
+00004e20: 6368 726f 6e69 7a65 6420 616e 6420 7361  chronized and sa
+00004e30: 7665 6420 696e 2074 6865 2063 6c6f 7564  ved in the cloud
+00004e40: 2c20 616c 6c6f 7769 6e67 2066 6f72 2072  , allowing for r
+00004e50: 656d 6f74 650a 2020 6d6f 6e69 746f 7269  emote.  monitori
+00004e60: 6e67 206f 6620 7472 6169 6e69 6e67 2070  ng of training p
+00004e70: 726f 6772 6573 732c 206d 616e 6167 696e  rogress, managin
+00004e80: 6720 6869 7374 6f72 6963 616c 2070 726f  g historical pro
+00004e90: 6a65 6374 732c 2073 6861 7269 6e67 2065  jects, sharing e
+00004ea0: 7870 6572 696d 656e 7420 6c69 6e6b 732c  xperiment links,
+00004eb0: 2073 656e 6469 6e67 2072 6561 6c2d 7469   sending real-ti
+00004ec0: 6d65 0a20 206e 6f74 6966 6963 6174 696f  me.  notificatio
+00004ed0: 6e20 6d65 7373 6167 6573 2c20 616e 6420  n messages, and 
+00004ee0: 7669 6577 696e 6720 6578 7065 7269 6d65  viewing experime
+00004ef0: 6e74 7320 6163 726f 7373 206d 756c 7469  nts across multi
+00004f00: 706c 6520 6465 7669 6365 732e 2049 6e20  ple devices. In 
+00004f10: 636f 6e74 7261 7374 2c20 5465 6e73 6f72  contrast, Tensor
+00004f20: 426f 6172 6420 6973 2061 6e20 6f66 666c  Board is an offl
+00004f30: 696e 650a 2020 6578 7065 7269 6d65 6e74  ine.  experiment
+00004f40: 2074 7261 636b 696e 6720 746f 6f6c 2e0a   tracking tool..
+00004f50: 0a2d 202a 2af0 9f91 a520 436f 6c6c 6162  .- **.... Collab
+00004f60: 6f72 6174 6976 6520 4d75 6c74 692d 7573  orative Multi-us
+00004f70: 6572 2045 6e76 6972 6f6e 6d65 6e74 2a2a  er Environment**
+00004f80: 3a0a 2020 5377 616e 4c61 6220 6661 6369  :.  SwanLab faci
+00004f90: 6c69 7461 7465 7320 6561 7379 206d 616e  litates easy man
+00004fa0: 6167 656d 656e 7420 6f66 206d 756c 7469  agement of multi
+00004fb0: 2d70 6572 736f 6e20 7472 6169 6e69 6e67  -person training
+00004fc0: 2070 726f 6a65 6374 7320 616e 6420 7368   projects and sh
+00004fd0: 6172 696e 6720 6f66 2065 7870 6572 696d  aring of experim
+00004fe0: 656e 7420 6c69 6e6b 7320 666f 720a 2020  ent links for.  
+00004ff0: 636f 6c6c 6162 6f72 6174 6976 6520 6d61  collaborative ma
+00005000: 6368 696e 6520 6c65 6172 6e69 6e67 2061  chine learning a
+00005010: 6372 6f73 7320 7465 616d 732e 2049 7420  cross teams. It 
+00005020: 616c 736f 2065 6e61 626c 6573 2063 726f  also enables cro
+00005030: 7373 2d73 7061 6365 2063 6f6d 6d75 6e69  ss-space communi
+00005040: 6361 7469 6f6e 2061 6e64 2064 6973 6375  cation and discu
+00005050: 7373 696f 6e2e 204f 6e20 7468 6520 6f74  ssion. On the ot
+00005060: 6865 720a 2020 6861 6e64 2c20 5465 6e73  her.  hand, Tens
+00005070: 6f72 426f 6172 6420 6973 2070 7269 6d61  orBoard is prima
+00005080: 7269 6c79 2064 6573 6967 6e65 6420 666f  rily designed fo
+00005090: 7220 696e 6469 7669 6475 616c 2075 7365  r individual use
+000050a0: 2c20 6d61 6b69 6e67 2069 7420 6469 6666  , making it diff
+000050b0: 6963 756c 7420 746f 2063 6f6c 6c61 626f  icult to collabo
+000050c0: 7261 7465 2061 6e64 2073 6861 7265 2065  rate and share e
+000050d0: 7870 6572 696d 656e 7473 0a20 2077 6974  xperiments.  wit
+000050e0: 6820 6d75 6c74 6970 6c65 2075 7365 7273  h multiple users
+000050f0: 2e0a 0a2d 202a 2af0 9f92 bb20 5065 7273  ...- **.... Pers
+00005100: 6973 7465 6e74 2c20 4365 6e74 7261 6c69  istent, Centrali
+00005110: 7a65 6420 4461 7368 626f 6172 642a 2a3a  zed Dashboard**:
+00005120: 0a20 2052 6567 6172 646c 6573 7320 6f66  .  Regardless of
+00005130: 2077 6865 7265 2079 6f75 2061 7265 2074   where you are t
+00005140: 7261 696e 696e 6720 796f 7572 206d 6f64  raining your mod
+00005150: 656c 732c 2062 6520 6974 206f 6e20 6120  els, be it on a 
+00005160: 6c6f 6361 6c20 636f 6d70 7574 6572 2c20  local computer, 
+00005170: 6120 6c61 6220 636c 7573 7465 722c 206f  a lab cluster, o
+00005180: 7220 6f6e 2070 7562 6c69 6320 636c 6f75  r on public clou
+00005190: 6420 4750 550a 2020 696e 7374 616e 6365  d GPU.  instance
+000051a0: 732c 2079 6f75 7220 7265 7375 6c74 7320  s, your results 
+000051b0: 6172 6520 6c6f 6767 6564 2074 6f20 7468  are logged to th
+000051c0: 6520 7361 6d65 2063 656e 7472 616c 697a  e same centraliz
+000051d0: 6564 2064 6173 6862 6f61 7264 2e20 5573  ed dashboard. Us
+000051e0: 696e 6720 5465 6e73 6f72 426f 6172 642c  ing TensorBoard,
+000051f0: 206f 6e20 7468 6520 6f74 6865 7220 6861   on the other ha
+00005200: 6e64 2c20 7265 7175 6972 6573 0a20 2073  nd, requires.  s
+00005210: 7065 6e64 696e 6720 7469 6d65 2063 6f70  pending time cop
+00005220: 7969 6e67 2061 6e64 206d 616e 6167 696e  ying and managin
+00005230: 6720 5446 4576 656e 7420 6669 6c65 7320  g TFEvent files 
+00005240: 6672 6f6d 2064 6966 6665 7265 6e74 206d  from different m
+00005250: 6163 6869 6e65 732e 0a0a 2d20 2a2a f09f  achines...- **..
+00005260: 92aa 204d 6f72 6520 506f 7765 7266 756c  .. More Powerful
+00005270: 2054 6162 6c65 732a 2a3a 0a20 2053 7761   Tables**:.  Swa
+00005280: 6e4c 6162 2074 6162 6c65 7320 616c 6c6f  nLab tables allo
+00005290: 7720 796f 7520 746f 2076 6965 772c 2073  w you to view, s
+000052a0: 6561 7263 682c 2061 6e64 2066 696c 7465  earch, and filte
+000052b0: 7220 7265 7375 6c74 7320 6672 6f6d 2076  r results from v
+000052c0: 6172 696f 7573 2065 7870 6572 696d 656e  arious experimen
+000052d0: 7473 2c20 6d61 6b69 6e67 2069 7420 6561  ts, making it ea
+000052e0: 7379 2074 6f20 7265 7669 6577 0a20 2074  sy to review.  t
+000052f0: 686f 7573 616e 6473 206f 6620 6d6f 6465  housands of mode
+00005300: 6c20 7665 7273 696f 6e73 2074 6f20 6669  l versions to fi
+00005310: 6e64 2074 6865 2062 6573 742d 7065 7266  nd the best-perf
+00005320: 6f72 6d69 6e67 206d 6f64 656c 7320 666f  orming models fo
+00005330: 7220 6469 6666 6572 656e 7420 7461 736b  r different task
+00005340: 732e 2054 656e 736f 7242 6f61 7264 2069  s. TensorBoard i
+00005350: 7320 6e6f 7420 7765 6c6c 2d73 7569 7465  s not well-suite
+00005360: 6420 666f 720a 2020 6c61 7267 652d 7363  d for.  large-sc
+00005370: 616c 6520 7072 6f6a 6563 7473 2e0a 0a23  ale projects...#
+00005380: 2323 2057 6569 6768 7473 2061 6e64 2042  ## Weights and B
+00005390: 6961 7365 7320 7673 2053 7761 6e4c 6162  iases vs SwanLab
+000053a0: 0a0a 2d20 5765 6967 6874 7320 616e 6420  ..- Weights and 
+000053b0: 4269 6173 6573 2069 7320 616e 206f 6e6c  Biases is an onl
+000053c0: 696e 652d 6f6e 6c79 2c20 7072 6f70 7269  ine-only, propri
+000053d0: 6574 6172 7920 4d4c 4f70 7320 706c 6174  etary MLOps plat
+000053e0: 666f 726d 2e0a 0a2d 204e 6f74 206f 6e6c  form...- Not onl
+000053f0: 7920 646f 6573 2053 7761 6e4c 6162 2073  y does SwanLab s
+00005400: 7570 706f 7274 206f 6e6c 696e 6520 7573  upport online us
+00005410: 6167 652c 2062 7574 2069 7420 616c 736f  age, but it also
+00005420: 206f 6666 6572 7320 616e 206f 7065 6e2d   offers an open-
+00005430: 736f 7572 6365 2c20 6672 6565 2c20 616e  source, free, an
+00005440: 6420 7365 6c66 2d68 6f73 7465 6420 7665  d self-hosted ve
+00005450: 7273 696f 6e2e 0a0a 3c62 723e 0a0a 2323  rsion...<br>..##
+00005460: 20f0 9f9b a3ef b88f 2052 6f61 646d 6170   ....... Roadmap
+00005470: 0a0a 546f 6f6c 7320 6576 6f6c 7665 2069  ..Tools evolve i
+00005480: 6e20 6974 6572 6174 696f 6e20 616e 6420  n iteration and 
+00005490: 6665 6564 6261 636b 7e2c 2077 656c 636f  feedback~, welco
+000054a0: 6d65 0a74 6f20 5b73 7562 6d69 7420 6665  me.to [submit fe
+000054b0: 6174 7572 6520 7375 6767 6573 7469 6f6e  ature suggestion
+000054c0: 735d 2868 7474 7073 3a2f 2f67 6565 6b74  s](https://geekt
+000054d0: 6563 6873 7475 6469 6f2e 6665 6973 6875  echstudio.feishu
+000054e0: 2e63 6e2f 7368 6172 652f 6261 7365 2f66  .cn/share/base/f
+000054f0: 6f72 6d2f 7368 7263 6e79 426c 4b38 4f4d  orm/shrcnyBlK8OM
+00005500: 4430 6577 656f 4663 6332 5376 574b 6329  D0eweoFcc2SvWKc)
+00005510: 0a0a 2323 2320 496e 2050 726f 6772 6573  ..### In Progres
+00005520: 7320 4e6f 770a 0a2d 2060 5461 626c 6560  s Now..- `Table`
+00005530: 3a20 4d6f 7265 2066 6c65 7869 626c 6520  : More flexible 
+00005540: 6d75 6c74 6964 696d 656e 7369 6f6e 616c  multidimensional
+00005550: 2074 6162 6c65 2063 6861 7274 732c 2073   table charts, s
+00005560: 7569 7461 626c 6520 666f 7220 4c4c 4d2c  uitable for LLM,
+00005570: 2041 4947 432c 206d 6f64 656c 2065 7661   AIGC, model eva
+00005580: 6c75 6174 696f 6e20 616e 6420 6f74 6865  luation and othe
+00005590: 7220 7363 656e 6172 696f 732e 0a0a 2d20  r scenarios...- 
+000055a0: 2a2a 456d 6169 6c20 6e6f 7469 6669 6361  **Email notifica
+000055b0: 7469 6f6e f09f 93a7 2a2a 3a20 5768 656e  tion....**: When
+000055c0: 2074 7261 696e 696e 6720 6973 2069 6e74   training is int
+000055d0: 6572 7275 7074 6564 2075 6e65 7870 6563  errupted unexpec
+000055e0: 7465 646c 792c 2077 6865 6e20 7472 6169  tedly, when trai
+000055f0: 6e69 6e67 2069 7320 636f 6d70 6c65 7465  ning is complete
+00005600: 642c 2061 6e64 2077 6865 6e20 6375 7374  d, and when cust
+00005610: 6f6d 0a20 2073 6974 7561 7469 6f6e 7320  om.  situations 
+00005620: 6f63 6375 722c 2073 656e 6420 6e6f 7469  occur, send noti
+00005630: 6669 6361 7469 6f6e 2065 6d61 696c 732e  fication emails.
+00005640: 0a0a 2323 2320 4e65 7874 2050 6c61 6e6e  ..### Next Plann
+00005650: 6564 0a0a 2d20 604d 6f6c 6563 756c 6560  ed..- `Molecule`
+00005660: 3a20 5669 7375 616c 697a 6174 696f 6e20  : Visualization 
+00005670: 6368 6172 7473 206f 6620 6269 6f63 6865  charts of bioche
+00005680: 6d69 7374 7279 206d 6f6c 6563 756c 6573  mistry molecules
+00005690: 0a0a 2d20 6050 6c6f 7460 3a20 4672 6565  ..- `Plot`: Free
+000056a0: 2063 6861 7274 2064 7261 7769 6e67 206d   chart drawing m
+000056b0: 6574 686f 640a 0a2d 2060 4170 6960 3a20  ethod..- `Api`: 
+000056c0: 4163 6365 7373 2053 7761 6e4c 6162 2064  Access SwanLab d
+000056d0: 6174 6120 7468 726f 7567 6820 4150 492e  ata through API.
+000056e0: 0a0a 2d20 2a2a 5379 7374 656d 2068 6172  ..- **System har
+000056f0: 6477 6172 6520 7265 636f 7264 732a 2a3a  dware records**:
+00005700: 2052 6563 6f72 6420 6120 7365 7269 6573   Record a series
+00005710: 206f 6620 6861 7264 7761 7265 2063 6f6e   of hardware con
+00005720: 6469 7469 6f6e 7320 7375 6368 2061 7320  ditions such as 
+00005730: 4750 552c 2043 5055 2c20 6469 736b 2c20  GPU, CPU, disk, 
+00005740: 6e65 7477 6f72 6b2c 2065 7463 2e0a 0a2d  network, etc...-
+00005750: 202a 2a43 6f64 6520 7265 636f 7264 732a   **Code records*
+00005760: 2a3a 2052 6563 6f72 6420 7472 6169 6e69  *: Record traini
+00005770: 6e67 2063 6f64 650a 0a2d 202a 2a4d 6f72  ng code..- **Mor
+00005780: 6520 696e 7465 6772 6174 696f 6e73 2a2a  e integrations**
+00005790: 3a20 4c69 6768 7447 424d 2c20 5847 426f  : LightGBM, XGBo
+000057a0: 6f73 742c 206f 7065 6e61 692c 2063 6861  ost, openai, cha
+000057b0: 7467 6c6d 2c20 6d6d 2073 6572 6965 732c  tglm, mm series,
+000057c0: 2e2e 2e0a 2d20 2e2e 2e0a 0a23 2323 204c  ....- .....### L
+000057d0: 6f6e 672d 7465 726d 2043 6f6e 6365 726e  ong-term Concern
+000057e0: 0a0a 2d20 5468 6520 6d6f 7374 2062 656e  ..- The most ben
+000057f0: 6566 6963 6961 6c20 636f 6c6c 6162 6f72  eficial collabor
+00005800: 6174 6976 6520 7761 7920 666f 7220 4149  ative way for AI
+00005810: 2074 6561 6d20 696e 6e6f 7661 7469 6f6e   team innovation
+00005820: 0a0a 2d20 5468 6520 6d6f 7374 2075 7365  ..- The most use
+00005830: 722d 6672 6965 6e64 6c79 2055 4920 696e  r-friendly UI in
+00005840: 7465 7261 6374 696f 6e0a 0a2d 2056 6965  teraction..- Vie
+00005850: 7769 6e67 2065 7870 6572 696d 656e 7473  wing experiments
+00005860: 206f 6e20 6d6f 6269 6c65 0a0a 3c62 723e   on mobile..<br>
+00005870: 0a0a 2323 20f0 9f91 a520 436f 6d6d 756e  ..## .... Commun
+00005880: 6974 790a 0a23 2323 2043 6f6d 6d75 6e69  ity..### Communi
+00005890: 7479 2061 6e64 2073 7570 706f 7274 0a0a  ty and support..
+000058a0: 2d20 5b47 6974 4875 6220 4973 7375 6573  - [GitHub Issues
+000058b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000058c0: 2e63 6f6d 2f53 7761 6e48 7562 582f 5377  .com/SwanHubX/Sw
+000058d0: 616e 4c61 622f 6973 7375 6573 29ef bc9a  anLab/issues)...
+000058e0: 4572 726f 7273 2061 6e64 2069 7373 7565  Errors and issue
+000058f0: 7320 656e 636f 756e 7465 7265 6420 7768  s encountered wh
+00005900: 656e 2075 7369 6e67 2053 7761 6e4c 6162  en using SwanLab
+00005910: 0a2d 205b 456d 6169 6c20 7375 7070 6f72  .- [Email suppor
+00005920: 745d 287a 6579 692e 6c69 6e40 7377 616e  t](zeyi.lin@swan
+00005930: 6875 622e 636f 29ef bc9a 4665 6564 6261  hub.co)...Feedba
+00005940: 636b 206f 6e20 6973 7375 6573 2077 6974  ck on issues wit
+00005950: 6820 7573 696e 6720 5377 616e 4c61 620a  h using SwanLab.
+00005960: 2d20 3c61 2068 7265 663d 2268 7474 7073  - <a href="https
+00005970: 3a2f 2f67 6565 6b74 6563 6873 7475 6469  ://geektechstudi
+00005980: 6f2e 6665 6973 6875 2e63 6e2f 7769 6b69  o.feishu.cn/wiki
+00005990: 2f4e 495a 3977 7035 4c52 6953 7151 796b  /NIZ9wp5LRiSqQyk
+000059a0: 697a 6247 6356 7a55 4b6e 6963 223e 5765  izbGcVzUKnic">We
+000059b0: 4368 6174 3c2f 613e efbc 9a44 6973 6375  Chat</a>...Discu
+000059c0: 7373 2069 7373 7565 7320 7573 696e 6720  ss issues using 
+000059d0: 5377 616e 4c61 622c 0a20 2073 6861 7265  SwanLab,.  share
+000059e0: 2074 6865 206c 6174 6573 7420 4149 2074   the latest AI t
+000059f0: 6563 686e 6f6c 6f67 792e 0a0a 2323 2320  echnology...### 
+00005a00: 5377 616e 4c61 6220 5245 4144 4d45 2042  SwanLab README B
+00005a10: 6164 6765 0a0a 4966 2079 6f75 206c 696b  adge..If you lik
+00005a20: 6520 746f 2075 7365 2053 7761 6e4c 6162  e to use SwanLab
+00005a30: 2069 6e20 796f 7572 2077 6f72 6b2c 2070   in your work, p
+00005a40: 6c65 6173 6520 6164 6420 7468 6520 5377  lease add the Sw
+00005a50: 616e 4c61 6220 6261 6467 6520 746f 2079  anLab badge to y
+00005a60: 6f75 7220 5245 4144 4d45 3a0a 0a5b 215b  our README:..[![
+00005a70: 7377 616e 6c61 625d 2868 7474 7073 3a2f  swanlab](https:/
+00005a80: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00005a90: 6261 6467 652f 706f 7765 7265 6425 3230  badge/powered%20
+00005aa0: 6279 2d53 7761 6e4c 6162 2d34 3338 3434  by-SwanLab-43844
+00005ab0: 3029 5d28 6874 7470 733a 2f2f 6769 7468  0)](https://gith
+00005ac0: 7562 2e63 6f6d 2f73 7761 6e68 7562 782f  ub.com/swanhubx/
+00005ad0: 7377 616e 6c61 6229 0a0a 6060 600a 5b21  swanlab)..```.[!
+00005ae0: 5b73 7761 6e6c 6162 5d28 6874 7470 733a  [swanlab](https:
+00005af0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00005b00: 2f62 6164 6765 2f70 6f77 6572 6564 2532  /badge/powered%2
+00005b10: 3062 792d 5377 616e 4c61 622d 3433 3834  0by-SwanLab-4384
+00005b20: 3430 295d 2868 7474 7073 3a2f 2f67 6974  40)](https://git
+00005b30: 6875 622e 636f 6d2f 7377 616e 6875 6278  hub.com/swanhubx
+00005b40: 2f73 7761 6e6c 6162 290a 6060 600a 0a23  /swanlab).```..#
+00005b50: 2323 2043 6974 696e 6720 5377 616e 4c61  ## Citing SwanLa
+00005b60: 6220 696e 2074 6865 2070 6170 6572 0a0a  b in the paper..
+00005b70: 4966 2079 6f75 2066 696e 6420 5377 616e  If you find Swan
+00005b80: 4c61 6220 6865 6c70 6675 6c20 666f 7220  Lab helpful for 
+00005b90: 796f 7572 2072 6573 6561 7263 6820 6a6f  your research jo
+00005ba0: 7572 6e65 792c 2070 6c65 6173 6520 636f  urney, please co
+00005bb0: 6e73 6964 6572 2063 6974 696e 6720 696e  nsider citing in
+00005bc0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
+00005bd0: 6f72 6d61 743a 0a0a 6060 6062 6962 7465  ormat:..```bibte
+00005be0: 780a 4073 6f66 7477 6172 657b 5a65 7969  x.@software{Zeyi
+00005bf0: 6c69 6e5f 5377 616e 4c61 625f 3230 3233  lin_SwanLab_2023
+00005c00: 2c0a 2020 6175 7468 6f72 203d 207b 5a65  ,.  author = {Ze
+00005c10: 7969 204c 696e 2c20 5368 616f 686f 6e67  yi Lin, Shaohong
+00005c20: 2043 6865 6e2c 204b 616e 6720 4c69 2c20   Chen, Kang Li, 
+00005c30: 5169 7573 6861 6e20 4a69 616e 672c 205a  Qiushan Jiang, Z
+00005c40: 6972 7569 2043 6169 2c20 204b 6169 6661  irui Cai,  Kaifa
+00005c50: 6e67 204a 6920 616e 6420 7b54 6865 2053  ng Ji and {The S
+00005c60: 7761 6e4c 6162 2074 6561 6d7d 7d2c 0a20  wanLab team}},. 
+00005c70: 2064 6f69 203d 207b 3130 2e35 3238 312f   doi = {10.5281/
+00005c80: 7a65 6e6f 646f 2e31 3131 3030 3535 307d  zenodo.11100550}
+00005c90: 2c0a 2020 6c69 6365 6e73 6520 3d20 7b41  ,.  license = {A
+00005ca0: 7061 6368 652d 322e 307d 2c0a 2020 7469  pache-2.0},.  ti
+00005cb0: 746c 6520 3d20 7b7b 5377 616e 4c61 627d  tle = {{SwanLab}
+00005cc0: 7d2c 0a20 2075 726c 203d 207b 6874 7470  },.  url = {http
+00005cd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00005ce0: 7761 6e68 7562 782f 7377 616e 6c61 627d  wanhubx/swanlab}
+00005cf0: 2c0a 2020 7965 6172 203d 207b 3230 3233  ,.  year = {2023
+00005d00: 7d0a 7d0a 6060 600a 0a23 2323 2043 6f6e  }.}.```..### Con
+00005d10: 7472 6962 7574 6520 746f 2053 7761 6e4c  tribute to SwanL
+00005d20: 6162 0a0a 436f 6e73 6964 6572 696e 6720  ab..Considering 
+00005d30: 636f 6e74 7269 6275 7469 6e67 2074 6f20  contributing to 
+00005d40: 5377 616e 4c61 623f 2046 6972 7374 2c20  SwanLab? First, 
+00005d50: 706c 6561 7365 2074 616b 6520 736f 6d65  please take some
+00005d60: 2074 696d 6520 746f 2072 6561 640a 7468   time to read.th
+00005d70: 6520 5b43 6f6e 7472 6962 7574 696f 6e20  e [Contribution 
+00005d80: 4775 6964 656c 696e 6573 5d28 434f 4e54  Guidelines](CONT
+00005d90: 5249 4255 5449 4e47 2e6d 6429 2e0a 0a41  RIBUTING.md)...A
+00005da0: 7420 7468 6520 7361 6d65 2074 696d 652c  t the same time,
+00005db0: 2077 6520 7761 726d 6c79 2077 656c 636f   we warmly welco
+00005dc0: 6d65 2073 7570 706f 7274 2066 6f72 2053  me support for S
+00005dd0: 7761 6e4c 6162 2074 6872 6f75 6768 2073  wanLab through s
+00005de0: 6f63 6961 6c20 6d65 6469 612c 2065 7665  ocial media, eve
+00005df0: 6e74 732c 2061 6e64 2063 6f6e 6665 7265  nts, and confere
+00005e00: 6e63 6520 7368 6172 696e 672e 2054 6861  nce sharing. Tha
+00005e10: 6e6b 2079 6f75 210a 0a3c 6272 3e0a 0a2a  nk you!..<br>..*
+00005e20: 2a43 6f6e 7472 6962 7574 6f72 732a 2a0a  *Contributors**.
+00005e30: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00005e40: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7761  //github.com/swa
+00005e50: 6e68 7562 782f 7377 616e 6c61 622f 6772  nhubx/swanlab/gr
+00005e60: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
+00005e70: 7322 3e0a 2020 3c69 6d67 2073 7263 3d22  s">.  <img src="
+00005e80: 6874 7470 733a 2f2f 636f 6e74 7269 622e  https://contrib.
+00005e90: 726f 636b 732f 696d 6167 653f 7265 706f  rocks/image?repo
+00005ea0: 3d73 7761 6e68 7562 782f 7377 616e 6c61  =swanhubx/swanla
+00005eb0: 6222 202f 3e0a 3c2f 613e 0a0a 2323 2320  b" />.</a>..### 
+00005ec0: 446f 776e 6c6f 6164 2049 636f 6e0a 0a5b  Download Icon..[
+00005ed0: 5377 616e 4c61 622d 4963 6f6e 2d53 5647  SwanLab-Icon-SVG
+00005ee0: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
+00005ef0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00005f00: 636f 6d2f 5377 616e 4875 6258 2f73 7761  com/SwanHubX/swa
+00005f10: 6e6c 6162 2f6d 6169 6e2f 7265 6164 6d65  nlab/main/readme
+00005f20: 5f66 696c 6573 2f73 7761 6e6c 6162 2d6c  _files/swanlab-l
+00005f30: 6f67 6f2e 7376 6729 0a0a 3c62 723e 0a0a  ogo.svg)..<br>..
+00005f40: 2323 20f0 9f93 8320 4c69 6365 6e73 650a  ## .... License.
+00005f50: 0a54 6869 7320 7265 706f 7369 746f 7279  .This repository
+00005f60: 2066 6f6c 6c6f 7773 2074 6865 205b 4170   follows the [Ap
+00005f70: 6163 6865 2032 2e30 204c 6963 656e 7365  ache 2.0 License
+00005f80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00005f90: 2e63 6f6d 2f53 7761 6e48 7562 582f 5377  .com/SwanHubX/Sw
+00005fa0: 616e 4c61 622f 626c 6f62 2f6d 6169 6e2f  anLab/blob/main/
+00005fb0: 4c49 4345 4e53 4529 206f 7065 6e20 736f  LICENSE) open so
+00005fc0: 7572 6365 0a6c 6963 656e 7365 2e0a       urce.license..
```

### Comparing `swanlab-0.3.6/package-lock.json` & `swanlab-0.3.7/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998587845721054%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'@headlessui/vue': '^1.7.22', 'terser': '^5.31.0', 'vue': "*

 * *               "'^3.3.11'}, 'devDependencies': {'@vitejs/plugin-vue': '^4.5.2', 'eslint': "*

 * *               "'^8.55.0', 'eslint-config-prettier': '^8.10.0', 'eslint-plugin-vue': '^9.19.2', "*

 * *               "'husky': '^8.0.3', 'postcss': '^8.4.32', 'prettier': '^2.8.8', 'tailwindcss': "*

 * *               "'^3.3.6', 'unplugin-auto-import': '^0.15.3', 'vite': '^5.0.6', 'vitest': "*

 * *               "'^1.6.0'}}, 'node_mo […]*

```diff
@@ -1,44 +1,44 @@
 {
     "lockfileVersion": 3,
     "name": "swanlab-ui",
     "packages": {
         "": {
             "dependencies": {
                 "@antv/g2plot": "^2.4.31",
-                "@headlessui/vue": "^1.7.16",
+                "@headlessui/vue": "^1.7.22",
                 "axios": "^1.6.2",
                 "html2canvas": "^1.4.1",
                 "moment": "^2.29.4",
                 "pinia": "^2.1.7",
                 "sass": "^1.69.5",
-                "terser": "^5.26.0",
+                "terser": "^5.31.0",
                 "tippy.js": "^6.3.7",
-                "vue": "^3.3.8",
+                "vue": "^3.3.11",
                 "vue-i18n": "^9.8.0",
                 "vue-router": "^4.2.5",
                 "vue-tippy": "^6.3.1"
             },
             "devDependencies": {
-                "@vitejs/plugin-vue": "^4.5.0",
+                "@vitejs/plugin-vue": "^4.5.2",
                 "autoprefixer": "^10.4.16",
-                "eslint": "^8.36.0",
-                "eslint-config-prettier": "^8.7.0",
+                "eslint": "^8.55.0",
+                "eslint-config-prettier": "^8.10.0",
                 "eslint-plugin-prettier": "^4.2.1",
-                "eslint-plugin-vue": "^9.9.0",
-                "husky": "^8.0.0",
+                "eslint-plugin-vue": "^9.19.2",
+                "husky": "^8.0.3",
                 "mockjs": "^1.1.0",
-                "postcss": "^8.4.31",
-                "prettier": "^2.8.5",
-                "tailwindcss": "^3.3.5",
-                "unplugin-auto-import": "^0.15.2",
+                "postcss": "^8.4.32",
+                "prettier": "^2.8.8",
+                "tailwindcss": "^3.3.6",
+                "unplugin-auto-import": "^0.15.3",
                 "unplugin-vue-components": "^0.24.1",
-                "vite": "^5.0.0",
+                "vite": "^5.0.6",
                 "vite-plugin-json5": "^1.1.2",
-                "vitest": "^1.1.3"
+                "vitest": "^1.6.0"
             },
             "name": "swanlab-ui",
             "version": "0.0.0"
         },
         "node_modules/@alloc/quick-lru": {
             "dev": true,
             "engines": {
@@ -1928,17 +1928,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-X/XhAVKlpIxWPpgRTnlgZssJrF0m6YtRA0QDWgsBNT12uZM6LPRydR7ip405Y3t1LamD8cP2TZFEDZFBf5ApcA==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001623.tgz",
-            "version": "1.0.30001623"
+            "integrity": "sha512-4KE9N2gcRH+HQhpeiRZXd+1niLB/XNLAhSy4z7fI8EzcbcPoAqjNInxVHTiTwWfTIV4w096XG8OtCOCQQKPv3w==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001625.tgz",
+            "version": "1.0.30001625"
         },
         "node_modules/center-align": {
             "dependencies": {
                 "align-text": "^0.1.3",
                 "lazy-cache": "^1.0.3"
             },
             "engines": {
@@ -2222,22 +2222,22 @@
             "dependencies": {
                 "ms": "2.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0"
             },
-            "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
+            "integrity": "sha512-pt0bNEmneDIvdL1Xsd9oDQ/wrQRkXDT4AUWlNZNPKvW5x/jyO9VFXkJUP07vQ2upmw5PlaITaPKc31jK13V+jg==",
             "peerDependenciesMeta": {
                 "supports-color": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
-            "version": "4.3.4"
+            "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.5.tgz",
+            "version": "4.3.5"
         },
         "node_modules/decamelize": {
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-z2S+W9X73hAUUki+N+9Za2lBlun89zigOyGrsax+KUQ6wKW4ZoWpEYBkGhQjwAjjDCkWxhY0VKEhk8wzY7F5cA==",
             "resolved": "https://registry.npmjs.org/decamelize/-/decamelize-1.2.0.tgz",
@@ -2381,17 +2381,17 @@
             "dev": true,
             "integrity": "sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==",
             "resolved": "https://registry.npmjs.org/eastasianwidth/-/eastasianwidth-0.2.0.tgz",
             "version": "0.2.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-bT0jEz/Xz1fahQpbZ1D7LgmPYZ3iHVY39NcWWro1+hA2IvjiPeaXtfSqrQ+nXjApMvQRE2ASt1itSLRrebHMRQ==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.783.tgz",
-            "version": "1.4.783"
+            "integrity": "sha512-d0EFmtLPjctczO3LogReyM2pbBiiZbnsKnGF+cdZhsYzHm/A0GV7W94kqzLD8SN4O3f3iHlgLUChqghgyznvCQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.787.tgz",
+            "version": "1.4.787"
         },
         "node_modules/emoji-regex": {
             "dev": true,
             "integrity": "sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-9.2.2.tgz",
             "version": "9.2.2"
         },
@@ -4447,26 +4447,26 @@
             "engines": {
                 "node": ">=12"
             },
             "funding": {
                 "url": "https://github.com/sponsors/antfu"
             },
             "hasInstallScript": true,
-            "integrity": "sha512-EOG8KXDQNwkJILkx/gPcoL/7vH+hORoBaKgGe+6W7VFMvCYJfmF2dGbvgDroVnI8LU7/kTu8mbjRZGBU1z9NTA==",
+            "integrity": "sha512-Uuqnk9YE9SsWeReYqK2alDI5YzciATE0r2SkA6iMAtuXvNTMNACJLJEXNXaEy94ECuBe4Sk6RzRU80kjdbIo1Q==",
             "peerDependencies": {
                 "@vue/composition-api": "^1.0.0-rc.1",
                 "vue": "^3.0.0-0 || ^2.6.0"
             },
             "peerDependenciesMeta": {
                 "@vue/composition-api": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vue-demi/-/vue-demi-0.14.7.tgz",
-            "version": "0.14.7"
+            "resolved": "https://registry.npmjs.org/vue-demi/-/vue-demi-0.14.8.tgz",
+            "version": "0.14.8"
         },
         "node_modules/pirates": {
             "dev": true,
             "engines": {
                 "node": ">= 6"
             },
             "integrity": "sha512-saLsH7WeYYPiD25LDuLRRY/i+6HaPYr6G1OUlN39otzkSTxKnubR9RTxS3/Kk50s1g2JTgFwWQDQyplC5/SHZg==",
@@ -4989,17 +4989,17 @@
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-eb4GZt1C3avsX3heBNlrc7I09nyT00IUuo4eFhAbeXWU2fvA7oXI53SxODVAA+zgZCk9aunAZgO+losjR3fAwA==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.77.2.tgz",
-            "version": "1.77.2"
+            "integrity": "sha512-vcF3Ckow6g939GMA4PeU7b2K/9FALXk2KF9J87txdHzXbUF9XRQRwSxcAs/fGaTnJeBFd7UoV22j3lzMLdM0Pw==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.77.4.tgz",
+            "version": "1.77.4"
         },
         "node_modules/scule": {
             "dev": true,
             "integrity": "sha512-6FtHJEvt+pVMIB9IBY+IcCJ6Z5f1iQnytgyfKMhDKgmzYG+TeH/wx1y3l27rshSbLiSanrR9ffZDrEsmjlQF2g==",
             "resolved": "https://registry.npmjs.org/scule/-/scule-1.3.0.tgz",
             "version": "1.3.0"
         },
@@ -6029,15 +6029,15 @@
             "dev": true,
             "engines": {
                 "node": "^18.0.0 || >=20.0.0"
             },
             "funding": {
                 "url": "https://github.com/vitejs/vite?sponsor=1"
             },
-            "integrity": "sha512-HndV31LWW05i1BLPMUCE1B9E9GFbOu1MbenhS58FuK6owSO5qHm7GiCotrNY1YE5rMeQSFBGmT5ZaLEjFizgiQ==",
+            "integrity": "sha512-/gC8GxzxMK5ntBwb48pR32GGhENnjtY30G4A0jemunsBkiEZFw60s8InGpN8gkhHEkjnRK1aSAxeQgwvFhUHAA==",
             "optionalDependencies": {
                 "fsevents": "~2.3.3"
             },
             "peerDependencies": {
                 "@types/node": "^18.0.0 || >=20.0.0",
                 "less": "*",
                 "lightningcss": "^1.21.0",
@@ -6065,16 +6065,16 @@
                 "sugarss": {
                     "optional": true
                 },
                 "terser": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vite/-/vite-5.2.11.tgz",
-            "version": "5.2.11"
+            "resolved": "https://registry.npmjs.org/vite/-/vite-5.2.12.tgz",
+            "version": "5.2.12"
         },
         "node_modules/vite-node": {
             "bin": {
                 "vite-node": "vite-node.mjs"
             },
             "dependencies": {
                 "cac": "^6.7.14",
```

### Comparing `swanlab-0.3.6/package.json` & `swanlab-0.3.7/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672046703296704%*

 * *Differences: {"'dependencies'": "{'@headlessui/vue': '^1.7.22', 'terser': '^5.31.0', 'vue': '^3.3.11'}",*

 * * "'devDependencies'": "{'@vitejs/plugin-vue': '^4.5.2', 'eslint': '^8.55.0', "*

 * *                      "'eslint-config-prettier': '^8.10.0', 'eslint-plugin-vue': '^9.19.2', "*

 * *                      "'husky': '^8.0.3', 'postcss': '^8.4.32', 'prettier': '^2.8.8', "*

 * *                      "'tailwindcss': '^3.3.6', 'unplugin-auto-import': '^0.15.3', 'vite': "*

 * *                      "'^5.0.6', 'vitest': '^1.6.0'}"}*

```diff
@@ -1,40 +1,40 @@
 {
     "dependencies": {
         "@antv/g2plot": "^2.4.31",
-        "@headlessui/vue": "^1.7.16",
+        "@headlessui/vue": "^1.7.22",
         "axios": "^1.6.2",
         "html2canvas": "^1.4.1",
         "moment": "^2.29.4",
         "pinia": "^2.1.7",
         "sass": "^1.69.5",
-        "terser": "^5.26.0",
+        "terser": "^5.31.0",
         "tippy.js": "^6.3.7",
-        "vue": "^3.3.8",
+        "vue": "^3.3.11",
         "vue-i18n": "^9.8.0",
         "vue-router": "^4.2.5",
         "vue-tippy": "^6.3.1"
     },
     "devDependencies": {
-        "@vitejs/plugin-vue": "^4.5.0",
+        "@vitejs/plugin-vue": "^4.5.2",
         "autoprefixer": "^10.4.16",
-        "eslint": "^8.36.0",
-        "eslint-config-prettier": "^8.7.0",
+        "eslint": "^8.55.0",
+        "eslint-config-prettier": "^8.10.0",
         "eslint-plugin-prettier": "^4.2.1",
-        "eslint-plugin-vue": "^9.9.0",
-        "husky": "^8.0.0",
+        "eslint-plugin-vue": "^9.19.2",
+        "husky": "^8.0.3",
         "mockjs": "^1.1.0",
-        "postcss": "^8.4.31",
-        "prettier": "^2.8.5",
-        "tailwindcss": "^3.3.5",
-        "unplugin-auto-import": "^0.15.2",
+        "postcss": "^8.4.32",
+        "prettier": "^2.8.8",
+        "tailwindcss": "^3.3.6",
+        "unplugin-auto-import": "^0.15.3",
         "unplugin-vue-components": "^0.24.1",
-        "vite": "^5.0.0",
+        "vite": "^5.0.6",
         "vite-plugin-json5": "^1.1.2",
-        "vitest": "^1.1.3"
+        "vitest": "^1.6.0"
     },
     "name": "swanlab-ui",
     "private": true,
     "scripts": {
         "build": "vite build",
         "build.release": "vite build --mode release",
         "dev": "vite",
```

### Comparing `swanlab-0.3.6/.vscode/extensions.json` & `swanlab-0.3.7/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/.vscode/launch.json` & `swanlab-0.3.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/.vscode/settings.json` & `swanlab-0.3.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/.vscode/tailwind.json` & `swanlab-0.3.7/.vscode/tailwind.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/.package-lock.json` & `swanlab-0.3.7/node_modules/.package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998537204850593%*

 * *Differences: {"'packages'": "{'node_modules/caniuse-lite': {'version': '1.0.30001625', 'resolved': "*

 * *               "'https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001625.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-4KE9N2gcRH+HQhpeiRZXd+1niLB/XNLAhSy4z7fI8EzcbcPoAqjNInxVHTiTwWfTIV4w096XG8OtCOCQQKPv3w=='}, "*

 * *               "'node_modules/debug': {'version': '4.3.5', 'resolved': "*

 * *               "'https://registry.npmjs.org/debug/-/debug-4.3.5.tgz', 'integrity': "*

 * *               "'sha512- […]*

```diff
@@ -1357,17 +1357,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-X/XhAVKlpIxWPpgRTnlgZssJrF0m6YtRA0QDWgsBNT12uZM6LPRydR7ip405Y3t1LamD8cP2TZFEDZFBf5ApcA==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001623.tgz",
-            "version": "1.0.30001623"
+            "integrity": "sha512-4KE9N2gcRH+HQhpeiRZXd+1niLB/XNLAhSy4z7fI8EzcbcPoAqjNInxVHTiTwWfTIV4w096XG8OtCOCQQKPv3w==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001625.tgz",
+            "version": "1.0.30001625"
         },
         "node_modules/center-align": {
             "dependencies": {
                 "align-text": "^0.1.3",
                 "lazy-cache": "^1.0.3"
             },
             "engines": {
@@ -1651,22 +1651,22 @@
             "dependencies": {
                 "ms": "2.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0"
             },
-            "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
+            "integrity": "sha512-pt0bNEmneDIvdL1Xsd9oDQ/wrQRkXDT4AUWlNZNPKvW5x/jyO9VFXkJUP07vQ2upmw5PlaITaPKc31jK13V+jg==",
             "peerDependenciesMeta": {
                 "supports-color": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
-            "version": "4.3.4"
+            "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.5.tgz",
+            "version": "4.3.5"
         },
         "node_modules/decamelize": {
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-z2S+W9X73hAUUki+N+9Za2lBlun89zigOyGrsax+KUQ6wKW4ZoWpEYBkGhQjwAjjDCkWxhY0VKEhk8wzY7F5cA==",
             "resolved": "https://registry.npmjs.org/decamelize/-/decamelize-1.2.0.tgz",
@@ -1810,17 +1810,17 @@
             "dev": true,
             "integrity": "sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==",
             "resolved": "https://registry.npmjs.org/eastasianwidth/-/eastasianwidth-0.2.0.tgz",
             "version": "0.2.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-bT0jEz/Xz1fahQpbZ1D7LgmPYZ3iHVY39NcWWro1+hA2IvjiPeaXtfSqrQ+nXjApMvQRE2ASt1itSLRrebHMRQ==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.783.tgz",
-            "version": "1.4.783"
+            "integrity": "sha512-d0EFmtLPjctczO3LogReyM2pbBiiZbnsKnGF+cdZhsYzHm/A0GV7W94kqzLD8SN4O3f3iHlgLUChqghgyznvCQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.787.tgz",
+            "version": "1.4.787"
         },
         "node_modules/emoji-regex": {
             "dev": true,
             "integrity": "sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-9.2.2.tgz",
             "version": "9.2.2"
         },
@@ -3863,26 +3863,26 @@
             "engines": {
                 "node": ">=12"
             },
             "funding": {
                 "url": "https://github.com/sponsors/antfu"
             },
             "hasInstallScript": true,
-            "integrity": "sha512-EOG8KXDQNwkJILkx/gPcoL/7vH+hORoBaKgGe+6W7VFMvCYJfmF2dGbvgDroVnI8LU7/kTu8mbjRZGBU1z9NTA==",
+            "integrity": "sha512-Uuqnk9YE9SsWeReYqK2alDI5YzciATE0r2SkA6iMAtuXvNTMNACJLJEXNXaEy94ECuBe4Sk6RzRU80kjdbIo1Q==",
             "peerDependencies": {
                 "@vue/composition-api": "^1.0.0-rc.1",
                 "vue": "^3.0.0-0 || ^2.6.0"
             },
             "peerDependenciesMeta": {
                 "@vue/composition-api": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vue-demi/-/vue-demi-0.14.7.tgz",
-            "version": "0.14.7"
+            "resolved": "https://registry.npmjs.org/vue-demi/-/vue-demi-0.14.8.tgz",
+            "version": "0.14.8"
         },
         "node_modules/pirates": {
             "dev": true,
             "engines": {
                 "node": ">= 6"
             },
             "integrity": "sha512-saLsH7WeYYPiD25LDuLRRY/i+6HaPYr6G1OUlN39otzkSTxKnubR9RTxS3/Kk50s1g2JTgFwWQDQyplC5/SHZg==",
@@ -4405,17 +4405,17 @@
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-eb4GZt1C3avsX3heBNlrc7I09nyT00IUuo4eFhAbeXWU2fvA7oXI53SxODVAA+zgZCk9aunAZgO+losjR3fAwA==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.77.2.tgz",
-            "version": "1.77.2"
+            "integrity": "sha512-vcF3Ckow6g939GMA4PeU7b2K/9FALXk2KF9J87txdHzXbUF9XRQRwSxcAs/fGaTnJeBFd7UoV22j3lzMLdM0Pw==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.77.4.tgz",
+            "version": "1.77.4"
         },
         "node_modules/scule": {
             "dev": true,
             "integrity": "sha512-6FtHJEvt+pVMIB9IBY+IcCJ6Z5f1iQnytgyfKMhDKgmzYG+TeH/wx1y3l27rshSbLiSanrR9ffZDrEsmjlQF2g==",
             "resolved": "https://registry.npmjs.org/scule/-/scule-1.3.0.tgz",
             "version": "1.3.0"
         },
@@ -5445,15 +5445,15 @@
             "dev": true,
             "engines": {
                 "node": "^18.0.0 || >=20.0.0"
             },
             "funding": {
                 "url": "https://github.com/vitejs/vite?sponsor=1"
             },
-            "integrity": "sha512-HndV31LWW05i1BLPMUCE1B9E9GFbOu1MbenhS58FuK6owSO5qHm7GiCotrNY1YE5rMeQSFBGmT5ZaLEjFizgiQ==",
+            "integrity": "sha512-/gC8GxzxMK5ntBwb48pR32GGhENnjtY30G4A0jemunsBkiEZFw60s8InGpN8gkhHEkjnRK1aSAxeQgwvFhUHAA==",
             "optionalDependencies": {
                 "fsevents": "~2.3.3"
             },
             "peerDependencies": {
                 "@types/node": "^18.0.0 || >=20.0.0",
                 "less": "*",
                 "lightningcss": "^1.21.0",
@@ -5481,16 +5481,16 @@
                 "sugarss": {
                     "optional": true
                 },
                 "terser": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vite/-/vite-5.2.11.tgz",
-            "version": "5.2.11"
+            "resolved": "https://registry.npmjs.org/vite/-/vite-5.2.12.tgz",
+            "version": "5.2.12"
         },
         "node_modules/vite-node": {
             "bin": {
                 "vite-node": "vite-node.mjs"
             },
             "dependencies": {
                 "cac": "^6.7.14",
```

### Comparing `swanlab-0.3.6/node_modules/@alloc/quick-lru/package.json` & `swanlab-0.3.7/node_modules/@alloc/quick-lru/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antfu/utils/package.json` & `swanlab-0.3.7/node_modules/@antfu/utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/adjust/package.json` & `swanlab-0.3.7/node_modules/@antv/adjust/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/adjust/node_modules/tslib/package.json` & `swanlab-0.3.7/node_modules/@antv/adjust/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/attr/package.json` & `swanlab-0.3.7/node_modules/@antv/attr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/color-util/package.json` & `swanlab-0.3.7/node_modules/@antv/color-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/component/package.json` & `swanlab-0.3.7/node_modules/@antv/component/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/component/node_modules/@antv/path-util/package.json` & `swanlab-0.3.7/node_modules/@antv/component/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.7/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/coord/package.json` & `swanlab-0.3.7/node_modules/@antv/coord/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/dom-util/package.json` & `swanlab-0.3.7/node_modules/@antv/dom-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/event-emitter/package.json` & `swanlab-0.3.7/node_modules/@antv/event-emitter/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-base/package.json` & `swanlab-0.3.7/node_modules/@antv/g-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json` & `swanlab-0.3.7/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.7/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-canvas/package.json` & `swanlab-0.3.7/node_modules/@antv/g-canvas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json` & `swanlab-0.3.7/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.7/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-math/package.json` & `swanlab-0.3.7/node_modules/@antv/g-math/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g-svg/package.json` & `swanlab-0.3.7/node_modules/@antv/g-svg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g2/package.json` & `swanlab-0.3.7/node_modules/@antv/g2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g2/node_modules/@antv/path-util/package.json` & `swanlab-0.3.7/node_modules/@antv/g2/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.7/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/g2plot/package.json` & `swanlab-0.3.7/node_modules/@antv/g2plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.7/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/path-util/package.json` & `swanlab-0.3.7/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/scale/package.json` & `swanlab-0.3.7/node_modules/@antv/scale/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@antv/util/package.json` & `swanlab-0.3.7/node_modules/@antv/util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@babel/parser/package.json` & `swanlab-0.3.7/node_modules/@babel/parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@eslint/eslintrc/package.json` & `swanlab-0.3.7/node_modules/@eslint/eslintrc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@eslint/js/package.json` & `swanlab-0.3.7/node_modules/@eslint/js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@eslint-community/eslint-utils/package.json` & `swanlab-0.3.7/node_modules/@eslint-community/eslint-utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@eslint-community/regexpp/package.json` & `swanlab-0.3.7/node_modules/@eslint-community/regexpp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@headlessui/vue/package.json` & `swanlab-0.3.7/node_modules/@headlessui/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@humanwhocodes/config-array/package.json` & `swanlab-0.3.7/node_modules/@humanwhocodes/config-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@humanwhocodes/module-importer/package.json` & `swanlab-0.3.7/node_modules/@humanwhocodes/module-importer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@humanwhocodes/object-schema/package.json` & `swanlab-0.3.7/node_modules/@humanwhocodes/object-schema/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@intlify/core-base/package.json` & `swanlab-0.3.7/node_modules/@intlify/core-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@intlify/message-compiler/package.json` & `swanlab-0.3.7/node_modules/@intlify/message-compiler/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@intlify/shared/package.json` & `swanlab-0.3.7/node_modules/@intlify/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@isaacs/cliui/package.json` & `swanlab-0.3.7/node_modules/@isaacs/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json` & `swanlab-0.3.7/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json` & `swanlab-0.3.7/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@jest/schemas/package.json` & `swanlab-0.3.7/node_modules/@jest/schemas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@jridgewell/gen-mapping/package.json` & `swanlab-0.3.7/node_modules/@jridgewell/gen-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@jridgewell/resolve-uri/package.json` & `swanlab-0.3.7/node_modules/@jridgewell/resolve-uri/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@jridgewell/set-array/package.json` & `swanlab-0.3.7/node_modules/@jridgewell/set-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@jridgewell/source-map/package.json` & `swanlab-0.3.7/node_modules/@jridgewell/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@jridgewell/sourcemap-codec/package.json` & `swanlab-0.3.7/node_modules/@jridgewell/sourcemap-codec/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@jridgewell/trace-mapping/package.json` & `swanlab-0.3.7/node_modules/@jridgewell/trace-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@ljharb/resumer/package.json` & `swanlab-0.3.7/node_modules/@ljharb/resumer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@ljharb/through/package.json` & `swanlab-0.3.7/node_modules/@ljharb/through/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@nodelib/fs.scandir/package.json` & `swanlab-0.3.7/node_modules/@nodelib/fs.scandir/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@nodelib/fs.stat/package.json` & `swanlab-0.3.7/node_modules/@nodelib/fs.stat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@nodelib/fs.walk/package.json` & `swanlab-0.3.7/node_modules/@nodelib/fs.walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@pkgjs/parseargs/package.json` & `swanlab-0.3.7/node_modules/@pkgjs/parseargs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@popperjs/core/package.json` & `swanlab-0.3.7/node_modules/@popperjs/core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@rollup/pluginutils/package.json` & `swanlab-0.3.7/node_modules/@rollup/pluginutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@sinclair/typebox/package.json` & `swanlab-0.3.7/node_modules/@sinclair/typebox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@tanstack/virtual-core/package.json` & `swanlab-0.3.7/node_modules/@tanstack/virtual-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@tanstack/vue-virtual/package.json` & `swanlab-0.3.7/node_modules/@tanstack/vue-virtual/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@types/d3-timer/package.json` & `swanlab-0.3.7/node_modules/@types/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@types/estree/package.json` & `swanlab-0.3.7/node_modules/@types/estree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@ungap/structured-clone/package.json` & `swanlab-0.3.7/node_modules/@ungap/structured-clone/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitejs/plugin-vue/package.json` & `swanlab-0.3.7/node_modules/@vitejs/plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/expect/package.json` & `swanlab-0.3.7/node_modules/@vitest/expect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/runner/package.json` & `swanlab-0.3.7/node_modules/@vitest/runner/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/runner/node_modules/p-limit/package.json` & `swanlab-0.3.7/node_modules/@vitest/runner/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/runner/node_modules/yocto-queue/package.json` & `swanlab-0.3.7/node_modules/@vitest/runner/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/snapshot/package.json` & `swanlab-0.3.7/node_modules/@vitest/snapshot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/spy/package.json` & `swanlab-0.3.7/node_modules/@vitest/spy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/utils/package.json` & `swanlab-0.3.7/node_modules/@vitest/utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vitest/utils/node_modules/estree-walker/package.json` & `swanlab-0.3.7/node_modules/@vitest/utils/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/compiler-core/package.json` & `swanlab-0.3.7/node_modules/@vue/compiler-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/compiler-dom/package.json` & `swanlab-0.3.7/node_modules/@vue/compiler-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/compiler-sfc/package.json` & `swanlab-0.3.7/node_modules/@vue/compiler-sfc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/compiler-ssr/package.json` & `swanlab-0.3.7/node_modules/@vue/compiler-ssr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/devtools-api/package.json` & `swanlab-0.3.7/node_modules/@vue/devtools-api/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/reactivity/package.json` & `swanlab-0.3.7/node_modules/@vue/reactivity/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/runtime-core/package.json` & `swanlab-0.3.7/node_modules/@vue/runtime-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/runtime-dom/package.json` & `swanlab-0.3.7/node_modules/@vue/runtime-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/server-renderer/package.json` & `swanlab-0.3.7/node_modules/@vue/server-renderer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/@vue/shared/package.json` & `swanlab-0.3.7/node_modules/@vue/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/acorn/package.json` & `swanlab-0.3.7/node_modules/acorn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/acorn-jsx/package.json` & `swanlab-0.3.7/node_modules/acorn-jsx/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/acorn-walk/package.json` & `swanlab-0.3.7/node_modules/acorn-walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ajv/package.json` & `swanlab-0.3.7/node_modules/ajv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ajv/lib/refs/data.json` & `swanlab-0.3.7/node_modules/ajv/lib/refs/data.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-draft-04.json` & `swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-draft-04.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-draft-06.json` & `swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-draft-06.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-draft-07.json` & `swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-draft-07.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ajv/lib/refs/json-schema-secure.json` & `swanlab-0.3.7/node_modules/ajv/lib/refs/json-schema-secure.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/align-text/package.json` & `swanlab-0.3.7/node_modules/align-text/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ansi-regex/package.json` & `swanlab-0.3.7/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ansi-styles/package.json` & `swanlab-0.3.7/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/any-promise/package.json` & `swanlab-0.3.7/node_modules/any-promise/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/anymatch/package.json` & `swanlab-0.3.7/node_modules/anymatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/arg/package.json` & `swanlab-0.3.7/node_modules/arg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/argparse/package.json` & `swanlab-0.3.7/node_modules/argparse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/array-buffer-byte-length/package.json` & `swanlab-0.3.7/node_modules/array-buffer-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/array-buffer-byte-length/tsconfig.json` & `swanlab-0.3.7/node_modules/array-buffer-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/arraybuffer.prototype.slice/package.json` & `swanlab-0.3.7/node_modules/arraybuffer.prototype.slice/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/assertion-error/package.json` & `swanlab-0.3.7/node_modules/assertion-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/asynckit/package.json` & `swanlab-0.3.7/node_modules/asynckit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/autoprefixer/package.json` & `swanlab-0.3.7/node_modules/autoprefixer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/available-typed-arrays/package.json` & `swanlab-0.3.7/node_modules/available-typed-arrays/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/available-typed-arrays/tsconfig.json` & `swanlab-0.3.7/node_modules/available-typed-arrays/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/axios/package.json` & `swanlab-0.3.7/node_modules/axios/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/balanced-match/package.json` & `swanlab-0.3.7/node_modules/balanced-match/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/base64-arraybuffer/package.json` & `swanlab-0.3.7/node_modules/base64-arraybuffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/binary-extensions/binary-extensions.json` & `swanlab-0.3.7/node_modules/binary-extensions/binary-extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/binary-extensions/package.json` & `swanlab-0.3.7/node_modules/binary-extensions/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/boolbase/package.json` & `swanlab-0.3.7/node_modules/boolbase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/brace-expansion/package.json` & `swanlab-0.3.7/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/braces/package.json` & `swanlab-0.3.7/node_modules/braces/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/browserslist/package.json` & `swanlab-0.3.7/node_modules/browserslist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/cac/package.json` & `swanlab-0.3.7/node_modules/cac/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/call-bind/package.json` & `swanlab-0.3.7/node_modules/call-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/callsites/package.json` & `swanlab-0.3.7/node_modules/callsites/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/camelcase/package.json` & `swanlab-0.3.7/node_modules/camelcase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/camelcase-css/package.json` & `swanlab-0.3.7/node_modules/camelcase-css/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/caniuse-lite/package.json` & `swanlab-0.3.7/node_modules/caniuse-lite/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'1.0.30001625'"}*

```diff
@@ -26,9 +26,9 @@
     "keywords": [
         "support"
     ],
     "license": "CC-BY-4.0",
     "main": "dist/unpacker/index.js",
     "name": "caniuse-lite",
     "repository": "browserslist/caniuse-lite",
-    "version": "1.0.30001623"
+    "version": "1.0.30001625"
 }
```

### Comparing `swanlab-0.3.6/node_modules/center-align/package.json` & `swanlab-0.3.7/node_modules/center-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/chai/package.json` & `swanlab-0.3.7/node_modules/chai/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/chalk/package.json` & `swanlab-0.3.7/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/check-error/package.json` & `swanlab-0.3.7/node_modules/check-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/chokidar/package.json` & `swanlab-0.3.7/node_modules/chokidar/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/chokidar/node_modules/glob-parent/package.json` & `swanlab-0.3.7/node_modules/chokidar/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/cliui/package.json` & `swanlab-0.3.7/node_modules/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/color-convert/package.json` & `swanlab-0.3.7/node_modules/color-convert/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/color-name/package.json` & `swanlab-0.3.7/node_modules/color-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/combined-stream/package.json` & `swanlab-0.3.7/node_modules/combined-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/commander/package.json` & `swanlab-0.3.7/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/concat-map/package.json` & `swanlab-0.3.7/node_modules/concat-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/confbox/package.json` & `swanlab-0.3.7/node_modules/confbox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/contour_plot/package.json` & `swanlab-0.3.7/node_modules/contour_plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/cross-spawn/package.json` & `swanlab-0.3.7/node_modules/cross-spawn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/css-line-break/package.json` & `swanlab-0.3.7/node_modules/css-line-break/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/cssesc/package.json` & `swanlab-0.3.7/node_modules/cssesc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/csstype/package.json` & `swanlab-0.3.7/node_modules/csstype/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/d3-color/package.json` & `swanlab-0.3.7/node_modules/d3-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/d3-ease/package.json` & `swanlab-0.3.7/node_modules/d3-ease/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/d3-hierarchy/package.json` & `swanlab-0.3.7/node_modules/d3-hierarchy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/d3-interpolate/package.json` & `swanlab-0.3.7/node_modules/d3-interpolate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/d3-regression/package.json` & `swanlab-0.3.7/node_modules/d3-regression/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/d3-timer/package.json` & `swanlab-0.3.7/node_modules/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/data-view-buffer/package.json` & `swanlab-0.3.7/node_modules/data-view-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/data-view-buffer/tsconfig.json` & `swanlab-0.3.7/node_modules/data-view-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/data-view-byte-length/package.json` & `swanlab-0.3.7/node_modules/data-view-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/data-view-byte-offset/package.json` & `swanlab-0.3.7/node_modules/data-view-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/data-view-byte-offset/tsconfig.json` & `swanlab-0.3.7/node_modules/data-view-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/debug/package.json` & `swanlab-0.3.7/node_modules/debug/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9317708333333333%*

 * *Differences: {"'author'": "'Josh Junon (https://github.com/qix-)'",*

 * * "'devDependencies'": "{'sinon': '^14.0.0'}",*

 * * "'scripts'": "{'test:node': 'istanbul cover _mocha -- test.js test.node.js'}",*

 * * "'version'": "'4.3.5'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "author": "Josh Junon <josh.junon@protonmail.com>",
+    "author": "Josh Junon (https://github.com/qix-)",
     "browser": "./src/browser.js",
     "contributors": [
         "TJ Holowaychuk <tj@vision-media.ca>",
         "Nathan Rajlich <nathan@tootallnate.net> (http://n8.io)",
         "Andrew Rhyne <rhyneandrew@gmail.com>"
     ],
     "dependencies": {
@@ -17,14 +17,15 @@
         "istanbul": "^0.4.5",
         "karma": "^3.1.4",
         "karma-browserify": "^6.0.0",
         "karma-chrome-launcher": "^2.2.0",
         "karma-mocha": "^1.3.0",
         "mocha": "^5.2.0",
         "mocha-lcov-reporter": "^1.2.0",
+        "sinon": "^14.0.0",
         "xo": "^0.23.0"
     },
     "engines": {
         "node": ">=6.0"
     },
     "files": [
         "src",
@@ -49,11 +50,11 @@
         "url": "git://github.com/debug-js/debug.git"
     },
     "scripts": {
         "lint": "xo",
         "test": "npm run test:node && npm run test:browser && npm run lint",
         "test:browser": "karma start --single-run",
         "test:coverage": "cat ./coverage/lcov.info | coveralls",
-        "test:node": "istanbul cover _mocha -- test.js"
+        "test:node": "istanbul cover _mocha -- test.js test.node.js"
     },
-    "version": "4.3.4"
+    "version": "4.3.5"
 }
```

### Comparing `swanlab-0.3.6/node_modules/decamelize/package.json` & `swanlab-0.3.7/node_modules/decamelize/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/deep-eql/package.json` & `swanlab-0.3.7/node_modules/deep-eql/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/deep-equal/package.json` & `swanlab-0.3.7/node_modules/deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/deep-is/package.json` & `swanlab-0.3.7/node_modules/deep-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/define-data-property/package.json` & `swanlab-0.3.7/node_modules/define-data-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/define-data-property/tsconfig.json` & `swanlab-0.3.7/node_modules/define-data-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/define-properties/package.json` & `swanlab-0.3.7/node_modules/define-properties/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/defined/package.json` & `swanlab-0.3.7/node_modules/defined/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/delayed-stream/package.json` & `swanlab-0.3.7/node_modules/delayed-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/detect-browser/package.json` & `swanlab-0.3.7/node_modules/detect-browser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/didyoumean/package.json` & `swanlab-0.3.7/node_modules/didyoumean/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/diff-sequences/package.json` & `swanlab-0.3.7/node_modules/diff-sequences/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/dlv/package.json` & `swanlab-0.3.7/node_modules/dlv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/doctrine/package.json` & `swanlab-0.3.7/node_modules/doctrine/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/dotignore/package.json` & `swanlab-0.3.7/node_modules/dotignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/electron-to-chromium/chromium-versions.json` & `swanlab-0.3.7/node_modules/electron-to-chromium/chromium-versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/electron-to-chromium/full-chromium-versions.json` & `swanlab-0.3.7/node_modules/electron-to-chromium/full-chromium-versions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974690745711285%*

 * *Differences: {"'122.0.6261.156'": "{insert: [(7, '29.4.2')]}",*

 * * "'124.0.6367.233'": "['30.0.9']",*

 * * "'126.0.6445.0'": "{insert: [(6, '31.0.0-beta.7'), (17, '32.0.0-nightly.20240529'), (18, "*

 * *                   "'32.0.0-nightly.20240530')]}"}*

```diff
@@ -1245,15 +1245,16 @@
     "122.0.6261.156": [
         "29.2.0",
         "29.3.0",
         "29.3.1",
         "29.3.2",
         "29.3.3",
         "29.4.0",
-        "29.4.1"
+        "29.4.1",
+        "29.4.2"
     ],
     "122.0.6261.18": [
         "29.0.0-beta.5",
         "29.0.0-beta.6",
         "29.0.0-beta.7",
         "29.0.0-beta.8",
         "29.0.0-beta.9",
@@ -1371,14 +1372,17 @@
     ],
     "124.0.6367.221": [
         "30.0.7"
     ],
     "124.0.6367.230": [
         "30.0.8"
     ],
+    "124.0.6367.233": [
+        "30.0.9"
+    ],
     "124.0.6367.29": [
         "30.0.0-beta.7",
         "30.0.0-beta.8"
     ],
     "124.0.6367.49": [
         "30.0.0"
     ],
@@ -1419,24 +1423,27 @@
     "126.0.6445.0": [
         "31.0.0-beta.1",
         "31.0.0-beta.2",
         "31.0.0-beta.3",
         "31.0.0-beta.4",
         "31.0.0-beta.5",
         "31.0.0-beta.6",
+        "31.0.0-beta.7",
         "32.0.0-nightly.20240513",
         "32.0.0-nightly.20240514",
         "32.0.0-nightly.20240515",
         "32.0.0-nightly.20240516",
         "32.0.0-nightly.20240517",
         "32.0.0-nightly.20240520",
         "32.0.0-nightly.20240521",
         "32.0.0-nightly.20240522",
         "32.0.0-nightly.20240523",
-        "32.0.0-nightly.20240524"
+        "32.0.0-nightly.20240524",
+        "32.0.0-nightly.20240529",
+        "32.0.0-nightly.20240530"
     ],
     "39.0.2171.65": [
         "0.20.0",
         "0.20.1",
         "0.20.2",
         "0.20.3",
         "0.20.4",
```

### Comparing `swanlab-0.3.6/node_modules/electron-to-chromium/full-versions.json` & `swanlab-0.3.7/node_modules/electron-to-chromium/full-versions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979131886477463%*

 * *Differences: {"'29.4.2'": "'122.0.6261.156'",*

 * * "'30.0.9'": "'124.0.6367.233'",*

 * * "'31.0.0-beta.7'": "'126.0.6445.0'",*

 * * "'32.0.0-nightly.20240529'": "'126.0.6445.0'",*

 * * "'32.0.0-nightly.20240530'": "'126.0.6445.0'"}*

```diff
@@ -1829,14 +1829,15 @@
     "29.2.0": "122.0.6261.156",
     "29.3.0": "122.0.6261.156",
     "29.3.1": "122.0.6261.156",
     "29.3.2": "122.0.6261.156",
     "29.3.3": "122.0.6261.156",
     "29.4.0": "122.0.6261.156",
     "29.4.1": "122.0.6261.156",
+    "29.4.2": "122.0.6261.156",
     "3.0.0": "66.0.3359.181",
     "3.0.0-beta.1": "66.0.3359.181",
     "3.0.0-beta.10": "66.0.3359.181",
     "3.0.0-beta.11": "66.0.3359.181",
     "3.0.0-beta.12": "66.0.3359.181",
     "3.0.0-beta.13": "66.0.3359.181",
     "3.0.0-beta.2": "66.0.3359.181",
@@ -1951,25 +1952,27 @@
     "30.0.2": "124.0.6367.91",
     "30.0.3": "124.0.6367.119",
     "30.0.4": "124.0.6367.201",
     "30.0.5": "124.0.6367.207",
     "30.0.6": "124.0.6367.207",
     "30.0.7": "124.0.6367.221",
     "30.0.8": "124.0.6367.230",
+    "30.0.9": "124.0.6367.233",
     "31.0.0-alpha.1": "125.0.6412.0",
     "31.0.0-alpha.2": "125.0.6412.0",
     "31.0.0-alpha.3": "125.0.6412.0",
     "31.0.0-alpha.4": "125.0.6412.0",
     "31.0.0-alpha.5": "125.0.6412.0",
     "31.0.0-beta.1": "126.0.6445.0",
     "31.0.0-beta.2": "126.0.6445.0",
     "31.0.0-beta.3": "126.0.6445.0",
     "31.0.0-beta.4": "126.0.6445.0",
     "31.0.0-beta.5": "126.0.6445.0",
     "31.0.0-beta.6": "126.0.6445.0",
+    "31.0.0-beta.7": "126.0.6445.0",
     "31.0.0-nightly.20240222": "123.0.6312.5",
     "31.0.0-nightly.20240223": "123.0.6312.5",
     "31.0.0-nightly.20240226": "123.0.6312.5",
     "31.0.0-nightly.20240227": "123.0.6312.5",
     "31.0.0-nightly.20240228": "123.0.6312.5",
     "31.0.0-nightly.20240229": "124.0.6323.0",
     "31.0.0-nightly.20240301": "124.0.6323.0",
@@ -2022,14 +2025,16 @@
     "32.0.0-nightly.20240516": "126.0.6445.0",
     "32.0.0-nightly.20240517": "126.0.6445.0",
     "32.0.0-nightly.20240520": "126.0.6445.0",
     "32.0.0-nightly.20240521": "126.0.6445.0",
     "32.0.0-nightly.20240522": "126.0.6445.0",
     "32.0.0-nightly.20240523": "126.0.6445.0",
     "32.0.0-nightly.20240524": "126.0.6445.0",
+    "32.0.0-nightly.20240529": "126.0.6445.0",
+    "32.0.0-nightly.20240530": "126.0.6445.0",
     "4.0.0": "69.0.3497.106",
     "4.0.0-beta.1": "69.0.3497.106",
     "4.0.0-beta.10": "69.0.3497.106",
     "4.0.0-beta.11": "69.0.3497.106",
     "4.0.0-beta.2": "69.0.3497.106",
     "4.0.0-beta.3": "69.0.3497.106",
     "4.0.0-beta.4": "69.0.3497.106",
```

### Comparing `swanlab-0.3.6/node_modules/electron-to-chromium/package.json` & `swanlab-0.3.7/node_modules/electron-to-chromium/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.4.787'"}*

```diff
@@ -36,9 +36,9 @@
     },
     "scripts": {
         "build": "node build.mjs",
         "report": "nyc report --reporter=text-lcov > coverage.lcov && codecov",
         "test": "nyc ava --verbose",
         "update": "node automated-update.js"
     },
-    "version": "1.4.783"
+    "version": "1.4.787"
 }
```

### Comparing `swanlab-0.3.6/node_modules/electron-to-chromium/versions.json` & `swanlab-0.3.7/node_modules/electron-to-chromium/versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/emoji-regex/package.json` & `swanlab-0.3.7/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/entities/package.json` & `swanlab-0.3.7/node_modules/entities/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-abstract/package.json` & `swanlab-0.3.7/node_modules/es-abstract/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-abstract/helpers/caseFolding.json` & `swanlab-0.3.7/node_modules/es-abstract/helpers/caseFolding.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-abstract/node_modules/object-inspect/package.json` & `swanlab-0.3.7/node_modules/es-abstract/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-define-property/package.json` & `swanlab-0.3.7/node_modules/es-define-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-define-property/tsconfig.json` & `swanlab-0.3.7/node_modules/es-define-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-errors/package.json` & `swanlab-0.3.7/node_modules/es-errors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-errors/tsconfig.json` & `swanlab-0.3.7/node_modules/es-errors/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-object-atoms/package.json` & `swanlab-0.3.7/node_modules/es-object-atoms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-set-tostringtag/package.json` & `swanlab-0.3.7/node_modules/es-set-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-set-tostringtag/tsconfig.json` & `swanlab-0.3.7/node_modules/es-set-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/es-to-primitive/package.json` & `swanlab-0.3.7/node_modules/es-to-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/esbuild/package.json` & `swanlab-0.3.7/node_modules/esbuild/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/escalade/package.json` & `swanlab-0.3.7/node_modules/escalade/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.7/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint/package.json` & `swanlab-0.3.7/node_modules/eslint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint/conf/replacements.json` & `swanlab-0.3.7/node_modules/eslint/conf/replacements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint/conf/rule-type-list.json` & `swanlab-0.3.7/node_modules/eslint/conf/rule-type-list.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json` & `swanlab-0.3.7/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-prettier/package.json` & `swanlab-0.3.7/node_modules/eslint-plugin-prettier/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/package.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/html-elements.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/html-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json` & `swanlab-0.3.7/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-scope/package.json` & `swanlab-0.3.7/node_modules/eslint-scope/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/eslint-visitor-keys/package.json` & `swanlab-0.3.7/node_modules/eslint-visitor-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/espree/package.json` & `swanlab-0.3.7/node_modules/espree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/esquery/package.json` & `swanlab-0.3.7/node_modules/esquery/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/esrecurse/package.json` & `swanlab-0.3.7/node_modules/esrecurse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/estraverse/package.json` & `swanlab-0.3.7/node_modules/estraverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/estree-walker/package.json` & `swanlab-0.3.7/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/esutils/package.json` & `swanlab-0.3.7/node_modules/esutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/execa/package.json` & `swanlab-0.3.7/node_modules/execa/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fast-deep-equal/package.json` & `swanlab-0.3.7/node_modules/fast-deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fast-diff/package.json` & `swanlab-0.3.7/node_modules/fast-diff/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fast-glob/package.json` & `swanlab-0.3.7/node_modules/fast-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fast-glob/node_modules/glob-parent/package.json` & `swanlab-0.3.7/node_modules/fast-glob/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fast-json-stable-stringify/package.json` & `swanlab-0.3.7/node_modules/fast-json-stable-stringify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fast-json-stable-stringify/benchmark/test.json` & `swanlab-0.3.7/node_modules/fast-json-stable-stringify/benchmark/test.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fast-levenshtein/package.json` & `swanlab-0.3.7/node_modules/fast-levenshtein/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fastq/package.json` & `swanlab-0.3.7/node_modules/fastq/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fecha/package.json` & `swanlab-0.3.7/node_modules/fecha/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/file-entry-cache/package.json` & `swanlab-0.3.7/node_modules/file-entry-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fill-range/package.json` & `swanlab-0.3.7/node_modules/fill-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/find-up/package.json` & `swanlab-0.3.7/node_modules/find-up/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/flat-cache/package.json` & `swanlab-0.3.7/node_modules/flat-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/flatted/package.json` & `swanlab-0.3.7/node_modules/flatted/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fmin/package.json` & `swanlab-0.3.7/node_modules/fmin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/follow-redirects/package.json` & `swanlab-0.3.7/node_modules/follow-redirects/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/for-each/package.json` & `swanlab-0.3.7/node_modules/for-each/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/foreground-child/package.json` & `swanlab-0.3.7/node_modules/foreground-child/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/form-data/package.json` & `swanlab-0.3.7/node_modules/form-data/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fraction.js/package.json` & `swanlab-0.3.7/node_modules/fraction.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/fs.realpath/package.json` & `swanlab-0.3.7/node_modules/fs.realpath/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/function-bind/package.json` & `swanlab-0.3.7/node_modules/function-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/function.prototype.name/package.json` & `swanlab-0.3.7/node_modules/function.prototype.name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/functions-have-names/package.json` & `swanlab-0.3.7/node_modules/functions-have-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/get-func-name/package.json` & `swanlab-0.3.7/node_modules/get-func-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/get-intrinsic/package.json` & `swanlab-0.3.7/node_modules/get-intrinsic/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/get-stream/package.json` & `swanlab-0.3.7/node_modules/get-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/get-symbol-description/package.json` & `swanlab-0.3.7/node_modules/get-symbol-description/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/gl-matrix/package.json` & `swanlab-0.3.7/node_modules/gl-matrix/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/glob/package.json` & `swanlab-0.3.7/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/glob-parent/package.json` & `swanlab-0.3.7/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/globals/globals.json` & `swanlab-0.3.7/node_modules/globals/globals.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/globals/package.json` & `swanlab-0.3.7/node_modules/globals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/globalthis/package.json` & `swanlab-0.3.7/node_modules/globalthis/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/gopd/package.json` & `swanlab-0.3.7/node_modules/gopd/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/graphemer/package.json` & `swanlab-0.3.7/node_modules/graphemer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has/package.json` & `swanlab-0.3.7/node_modules/has/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-ansi/package.json` & `swanlab-0.3.7/node_modules/has-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.7/node_modules/has-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-bigints/package.json` & `swanlab-0.3.7/node_modules/has-bigints/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-flag/package.json` & `swanlab-0.3.7/node_modules/has-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-property-descriptors/package.json` & `swanlab-0.3.7/node_modules/has-property-descriptors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-proto/package.json` & `swanlab-0.3.7/node_modules/has-proto/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-proto/tsconfig.json` & `swanlab-0.3.7/node_modules/has-proto/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-symbols/package.json` & `swanlab-0.3.7/node_modules/has-symbols/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-tostringtag/package.json` & `swanlab-0.3.7/node_modules/has-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/has-tostringtag/tsconfig.json` & `swanlab-0.3.7/node_modules/has-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/hasown/package.json` & `swanlab-0.3.7/node_modules/hasown/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/html2canvas/package.json` & `swanlab-0.3.7/node_modules/html2canvas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/html2canvas/tsconfig.json` & `swanlab-0.3.7/node_modules/html2canvas/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/human-signals/package.json` & `swanlab-0.3.7/node_modules/human-signals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/husky/package.json` & `swanlab-0.3.7/node_modules/husky/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ignore/package.json` & `swanlab-0.3.7/node_modules/ignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/immutable/package.json` & `swanlab-0.3.7/node_modules/immutable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/import-fresh/package.json` & `swanlab-0.3.7/node_modules/import-fresh/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/imurmurhash/package.json` & `swanlab-0.3.7/node_modules/imurmurhash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/inflight/package.json` & `swanlab-0.3.7/node_modules/inflight/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/inherits/package.json` & `swanlab-0.3.7/node_modules/inherits/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/internal-slot/package.json` & `swanlab-0.3.7/node_modules/internal-slot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-arguments/package.json` & `swanlab-0.3.7/node_modules/is-arguments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-array-buffer/package.json` & `swanlab-0.3.7/node_modules/is-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-array-buffer/tsconfig.json` & `swanlab-0.3.7/node_modules/is-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-bigint/package.json` & `swanlab-0.3.7/node_modules/is-bigint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-binary-path/package.json` & `swanlab-0.3.7/node_modules/is-binary-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-boolean-object/package.json` & `swanlab-0.3.7/node_modules/is-boolean-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-buffer/package.json` & `swanlab-0.3.7/node_modules/is-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-callable/package.json` & `swanlab-0.3.7/node_modules/is-callable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-core-module/core.json` & `swanlab-0.3.7/node_modules/is-core-module/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-core-module/package.json` & `swanlab-0.3.7/node_modules/is-core-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-data-view/package.json` & `swanlab-0.3.7/node_modules/is-data-view/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-data-view/tsconfig.json` & `swanlab-0.3.7/node_modules/is-data-view/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-date-object/package.json` & `swanlab-0.3.7/node_modules/is-date-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-extglob/package.json` & `swanlab-0.3.7/node_modules/is-extglob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-fullwidth-code-point/package.json` & `swanlab-0.3.7/node_modules/is-fullwidth-code-point/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-glob/package.json` & `swanlab-0.3.7/node_modules/is-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-negative-zero/package.json` & `swanlab-0.3.7/node_modules/is-negative-zero/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-negative-zero/tsconfig.json` & `swanlab-0.3.7/node_modules/is-negative-zero/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-number/package.json` & `swanlab-0.3.7/node_modules/is-number/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-number-object/package.json` & `swanlab-0.3.7/node_modules/is-number-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-path-inside/package.json` & `swanlab-0.3.7/node_modules/is-path-inside/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-regex/package.json` & `swanlab-0.3.7/node_modules/is-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-shared-array-buffer/package.json` & `swanlab-0.3.7/node_modules/is-shared-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-shared-array-buffer/tsconfig.json` & `swanlab-0.3.7/node_modules/is-shared-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-stream/package.json` & `swanlab-0.3.7/node_modules/is-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-string/package.json` & `swanlab-0.3.7/node_modules/is-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-symbol/package.json` & `swanlab-0.3.7/node_modules/is-symbol/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-typed-array/package.json` & `swanlab-0.3.7/node_modules/is-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-typed-array/tsconfig.json` & `swanlab-0.3.7/node_modules/is-typed-array/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/is-weakref/package.json` & `swanlab-0.3.7/node_modules/is-weakref/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/isarray/package.json` & `swanlab-0.3.7/node_modules/isarray/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/isexe/package.json` & `swanlab-0.3.7/node_modules/isexe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/jackspeak/package.json` & `swanlab-0.3.7/node_modules/jackspeak/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/jiti/package.json` & `swanlab-0.3.7/node_modules/jiti/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/js-yaml/package.json` & `swanlab-0.3.7/node_modules/js-yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/json-buffer/package.json` & `swanlab-0.3.7/node_modules/json-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/json-schema-traverse/package.json` & `swanlab-0.3.7/node_modules/json-schema-traverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/json-stable-stringify-without-jsonify/package.json` & `swanlab-0.3.7/node_modules/json-stable-stringify-without-jsonify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/json2module/package.json` & `swanlab-0.3.7/node_modules/json2module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/json5/package.json` & `swanlab-0.3.7/node_modules/json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/keyv/package.json` & `swanlab-0.3.7/node_modules/keyv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/kind-of/package.json` & `swanlab-0.3.7/node_modules/kind-of/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/lazy-cache/package.json` & `swanlab-0.3.7/node_modules/lazy-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/levn/package.json` & `swanlab-0.3.7/node_modules/levn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/lilconfig/package.json` & `swanlab-0.3.7/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/lines-and-columns/package.json` & `swanlab-0.3.7/node_modules/lines-and-columns/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/local-pkg/package.json` & `swanlab-0.3.7/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/locate-path/package.json` & `swanlab-0.3.7/node_modules/locate-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/lodash/package.json` & `swanlab-0.3.7/node_modules/lodash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/lodash-es/package.json` & `swanlab-0.3.7/node_modules/lodash-es/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/lodash.merge/package.json` & `swanlab-0.3.7/node_modules/lodash.merge/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/longest/package.json` & `swanlab-0.3.7/node_modules/longest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/loupe/package.json` & `swanlab-0.3.7/node_modules/loupe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/lru-cache/package.json` & `swanlab-0.3.7/node_modules/lru-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/magic-string/package.json` & `swanlab-0.3.7/node_modules/magic-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/merge2/package.json` & `swanlab-0.3.7/node_modules/merge2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/micromatch/package.json` & `swanlab-0.3.7/node_modules/micromatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mime-db/db.json` & `swanlab-0.3.7/node_modules/mime-db/db.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mime-db/package.json` & `swanlab-0.3.7/node_modules/mime-db/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mime-types/package.json` & `swanlab-0.3.7/node_modules/mime-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mimic-fn/package.json` & `swanlab-0.3.7/node_modules/mimic-fn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/minimatch/package.json` & `swanlab-0.3.7/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/minimist/package.json` & `swanlab-0.3.7/node_modules/minimist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/minipass/package.json` & `swanlab-0.3.7/node_modules/minipass/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mlly/package.json` & `swanlab-0.3.7/node_modules/mlly/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mock-property/package.json` & `swanlab-0.3.7/node_modules/mock-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mockjs/package.json` & `swanlab-0.3.7/node_modules/mockjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/moment/package.json` & `swanlab-0.3.7/node_modules/moment/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ms/package.json` & `swanlab-0.3.7/node_modules/ms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/mz/package.json` & `swanlab-0.3.7/node_modules/mz/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/nanoid/package.json` & `swanlab-0.3.7/node_modules/nanoid/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/natural-compare/package.json` & `swanlab-0.3.7/node_modules/natural-compare/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/node-releases/data/processed/envs.json` & `swanlab-0.3.7/node_modules/node-releases/data/processed/envs.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/node-releases/data/release-schedule/release-schedule.json` & `swanlab-0.3.7/node_modules/node-releases/data/release-schedule/release-schedule.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/normalize-path/package.json` & `swanlab-0.3.7/node_modules/normalize-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/normalize-range/package.json` & `swanlab-0.3.7/node_modules/normalize-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/npm-run-path/package.json` & `swanlab-0.3.7/node_modules/npm-run-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/npm-run-path/node_modules/path-key/package.json` & `swanlab-0.3.7/node_modules/npm-run-path/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/nth-check/package.json` & `swanlab-0.3.7/node_modules/nth-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/object-assign/package.json` & `swanlab-0.3.7/node_modules/object-assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/object-hash/package.json` & `swanlab-0.3.7/node_modules/object-hash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/object-inspect/package.json` & `swanlab-0.3.7/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/object-is/package.json` & `swanlab-0.3.7/node_modules/object-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/object-keys/package.json` & `swanlab-0.3.7/node_modules/object-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/object.assign/package.json` & `swanlab-0.3.7/node_modules/object.assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/once/package.json` & `swanlab-0.3.7/node_modules/once/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/onetime/package.json` & `swanlab-0.3.7/node_modules/onetime/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/optionator/package.json` & `swanlab-0.3.7/node_modules/optionator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/p-limit/package.json` & `swanlab-0.3.7/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/p-locate/package.json` & `swanlab-0.3.7/node_modules/p-locate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/parent-module/package.json` & `swanlab-0.3.7/node_modules/parent-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/path-exists/package.json` & `swanlab-0.3.7/node_modules/path-exists/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/path-is-absolute/package.json` & `swanlab-0.3.7/node_modules/path-is-absolute/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/path-key/package.json` & `swanlab-0.3.7/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/path-parse/package.json` & `swanlab-0.3.7/node_modules/path-parse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/path-scurry/package.json` & `swanlab-0.3.7/node_modules/path-scurry/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pathe/package.json` & `swanlab-0.3.7/node_modules/pathe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pathval/package.json` & `swanlab-0.3.7/node_modules/pathval/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pdfast/package.json` & `swanlab-0.3.7/node_modules/pdfast/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/picocolors/package.json` & `swanlab-0.3.7/node_modules/picocolors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/picomatch/package.json` & `swanlab-0.3.7/node_modules/picomatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pify/package.json` & `swanlab-0.3.7/node_modules/pify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pinia/package.json` & `swanlab-0.3.7/node_modules/pinia/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pinia/node_modules/vue-demi/package.json` & `swanlab-0.3.7/node_modules/pinia/node_modules/vue-demi/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'0.14.8'"}*

```diff
@@ -39,9 +39,9 @@
     "repository": "https://github.com/antfu/vue-demi.git",
     "scripts": {
         "postinstall": "node -e \"try{require('./scripts/postinstall.js')}catch(e){}\"",
         "release": "npx bumpp --tag --commit --push && npm publish"
     },
     "types": "lib/index.d.ts",
     "unpkg": "lib/index.iife.js",
-    "version": "0.14.7"
+    "version": "0.14.8"
 }
```

### Comparing `swanlab-0.3.6/node_modules/pirates/package.json` & `swanlab-0.3.7/node_modules/pirates/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pkg-types/package.json` & `swanlab-0.3.7/node_modules/pkg-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/possible-typed-array-names/package.json` & `swanlab-0.3.7/node_modules/possible-typed-array-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/possible-typed-array-names/tsconfig.json` & `swanlab-0.3.7/node_modules/possible-typed-array-names/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss/package.json` & `swanlab-0.3.7/node_modules/postcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss-import/package.json` & `swanlab-0.3.7/node_modules/postcss-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss-js/package.json` & `swanlab-0.3.7/node_modules/postcss-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss-load-config/package.json` & `swanlab-0.3.7/node_modules/postcss-load-config/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss-load-config/node_modules/lilconfig/package.json` & `swanlab-0.3.7/node_modules/postcss-load-config/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss-nested/package.json` & `swanlab-0.3.7/node_modules/postcss-nested/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss-selector-parser/package.json` & `swanlab-0.3.7/node_modules/postcss-selector-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/postcss-value-parser/package.json` & `swanlab-0.3.7/node_modules/postcss-value-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/prelude-ls/package.json` & `swanlab-0.3.7/node_modules/prelude-ls/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/prettier-linter-helpers/package.json` & `swanlab-0.3.7/node_modules/prettier-linter-helpers/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pretty-format/package.json` & `swanlab-0.3.7/node_modules/pretty-format/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/pretty-format/node_modules/ansi-styles/package.json` & `swanlab-0.3.7/node_modules/pretty-format/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/proxy-from-env/package.json` & `swanlab-0.3.7/node_modules/proxy-from-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/punycode/package.json` & `swanlab-0.3.7/node_modules/punycode/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/queue-microtask/package.json` & `swanlab-0.3.7/node_modules/queue-microtask/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/read-cache/package.json` & `swanlab-0.3.7/node_modules/read-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/readdirp/package.json` & `swanlab-0.3.7/node_modules/readdirp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/regexp.prototype.flags/package.json` & `swanlab-0.3.7/node_modules/regexp.prototype.flags/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/repeat-string/package.json` & `swanlab-0.3.7/node_modules/repeat-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/resolve/package.json` & `swanlab-0.3.7/node_modules/resolve/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/resolve/lib/core.json` & `swanlab-0.3.7/node_modules/resolve/lib/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/resolve-from/package.json` & `swanlab-0.3.7/node_modules/resolve-from/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/reusify/package.json` & `swanlab-0.3.7/node_modules/reusify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/right-align/package.json` & `swanlab-0.3.7/node_modules/right-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rimraf/package.json` & `swanlab-0.3.7/node_modules/rimraf/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rollup/package.json` & `swanlab-0.3.7/node_modules/rollup/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rollup/node_modules/ansi-regex/package.json` & `swanlab-0.3.7/node_modules/rollup/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rollup/node_modules/ansi-styles/package.json` & `swanlab-0.3.7/node_modules/rollup/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rollup/node_modules/chalk/package.json` & `swanlab-0.3.7/node_modules/rollup/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rollup/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.7/node_modules/rollup/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rollup/node_modules/strip-ansi/package.json` & `swanlab-0.3.7/node_modules/rollup/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rollup/node_modules/supports-color/package.json` & `swanlab-0.3.7/node_modules/rollup/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/run-parallel/package.json` & `swanlab-0.3.7/node_modules/run-parallel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/rw/package.json` & `swanlab-0.3.7/node_modules/rw/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/safe-array-concat/package.json` & `swanlab-0.3.7/node_modules/safe-array-concat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/safe-regex-test/package.json` & `swanlab-0.3.7/node_modules/safe-regex-test/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/sass/package.json` & `swanlab-0.3.7/node_modules/sass/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'1.77.4'"}*

```diff
@@ -40,9 +40,9 @@
     "main": "sass.node.js",
     "name": "sass",
     "repository": {
         "type": "git",
         "url": "https://github.com/sass/dart-sass"
     },
     "types": "types/index.d.ts",
-    "version": "1.77.2"
+    "version": "1.77.4"
 }
```

### Comparing `swanlab-0.3.6/node_modules/scule/package.json` & `swanlab-0.3.7/node_modules/scule/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/semver/package.json` & `swanlab-0.3.7/node_modules/semver/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/set-function-length/package.json` & `swanlab-0.3.7/node_modules/set-function-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/set-function-name/package.json` & `swanlab-0.3.7/node_modules/set-function-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/set-function-name/tsconfig.json` & `swanlab-0.3.7/node_modules/set-function-name/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/shebang-command/package.json` & `swanlab-0.3.7/node_modules/shebang-command/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/shebang-regex/package.json` & `swanlab-0.3.7/node_modules/shebang-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/side-channel/package.json` & `swanlab-0.3.7/node_modules/side-channel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/side-channel/tsconfig.json` & `swanlab-0.3.7/node_modules/side-channel/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/side-channel/node_modules/object-inspect/package.json` & `swanlab-0.3.7/node_modules/side-channel/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/siginfo/package.json` & `swanlab-0.3.7/node_modules/siginfo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/signal-exit/package.json` & `swanlab-0.3.7/node_modules/signal-exit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/size-sensor/package.json` & `swanlab-0.3.7/node_modules/size-sensor/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/source-map/package.json` & `swanlab-0.3.7/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/source-map-js/package.json` & `swanlab-0.3.7/node_modules/source-map-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/source-map-support/package.json` & `swanlab-0.3.7/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/std-env/package.json` & `swanlab-0.3.7/node_modules/std-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string-width/package.json` & `swanlab-0.3.7/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string-width/node_modules/ansi-regex/package.json` & `swanlab-0.3.7/node_modules/string-width/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string-width/node_modules/strip-ansi/package.json` & `swanlab-0.3.7/node_modules/string-width/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string-width-cjs/package.json` & `swanlab-0.3.7/node_modules/string-width-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string-width-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.7/node_modules/string-width-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string.prototype.trim/package.json` & `swanlab-0.3.7/node_modules/string.prototype.trim/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string.prototype.trimend/package.json` & `swanlab-0.3.7/node_modules/string.prototype.trimend/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/string.prototype.trimstart/package.json` & `swanlab-0.3.7/node_modules/string.prototype.trimstart/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/strip-ansi/package.json` & `swanlab-0.3.7/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/strip-ansi-cjs/package.json` & `swanlab-0.3.7/node_modules/strip-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/strip-final-newline/package.json` & `swanlab-0.3.7/node_modules/strip-final-newline/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/strip-json-comments/package.json` & `swanlab-0.3.7/node_modules/strip-json-comments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/strip-literal/package.json` & `swanlab-0.3.7/node_modules/strip-literal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/sucrase/package.json` & `swanlab-0.3.7/node_modules/sucrase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/sucrase/node_modules/brace-expansion/package.json` & `swanlab-0.3.7/node_modules/sucrase/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/sucrase/node_modules/commander/package.json` & `swanlab-0.3.7/node_modules/sucrase/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/sucrase/node_modules/glob/package.json` & `swanlab-0.3.7/node_modules/sucrase/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/sucrase/node_modules/minimatch/package.json` & `swanlab-0.3.7/node_modules/sucrase/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/supports-color/package.json` & `swanlab-0.3.7/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/supports-preserve-symlinks-flag/package.json` & `swanlab-0.3.7/node_modules/supports-preserve-symlinks-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/tailwindcss/package.json` & `swanlab-0.3.7/node_modules/tailwindcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/tape/package.json` & `swanlab-0.3.7/node_modules/tape/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/terser/package.json` & `swanlab-0.3.7/node_modules/terser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/terser/node_modules/commander/package.json` & `swanlab-0.3.7/node_modules/terser/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/terser/node_modules/source-map/package.json` & `swanlab-0.3.7/node_modules/terser/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/terser/node_modules/source-map-support/package.json` & `swanlab-0.3.7/node_modules/terser/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/text-segmentation/package.json` & `swanlab-0.3.7/node_modules/text-segmentation/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/text-table/package.json` & `swanlab-0.3.7/node_modules/text-table/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/thenify/package.json` & `swanlab-0.3.7/node_modules/thenify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/thenify-all/package.json` & `swanlab-0.3.7/node_modules/thenify-all/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/tinybench/package.json` & `swanlab-0.3.7/node_modules/tinybench/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/tinypool/package.json` & `swanlab-0.3.7/node_modules/tinypool/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/tinyspy/package.json` & `swanlab-0.3.7/node_modules/tinyspy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/tippy.js/package.json` & `swanlab-0.3.7/node_modules/tippy.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/to-regex-range/package.json` & `swanlab-0.3.7/node_modules/to-regex-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ts-interface-checker/package.json` & `swanlab-0.3.7/node_modules/ts-interface-checker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/tslib/package.json` & `swanlab-0.3.7/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/type-check/package.json` & `swanlab-0.3.7/node_modules/type-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/type-detect/package.json` & `swanlab-0.3.7/node_modules/type-detect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/type-fest/package.json` & `swanlab-0.3.7/node_modules/type-fest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/typed-array-buffer/package.json` & `swanlab-0.3.7/node_modules/typed-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/typed-array-buffer/tsconfig.json` & `swanlab-0.3.7/node_modules/typed-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/typed-array-byte-length/package.json` & `swanlab-0.3.7/node_modules/typed-array-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/typed-array-byte-length/tsconfig.json` & `swanlab-0.3.7/node_modules/typed-array-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/typed-array-byte-offset/package.json` & `swanlab-0.3.7/node_modules/typed-array-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/typed-array-byte-offset/tsconfig.json` & `swanlab-0.3.7/node_modules/typed-array-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/typed-array-length/package.json` & `swanlab-0.3.7/node_modules/typed-array-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/ufo/package.json` & `swanlab-0.3.7/node_modules/ufo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/uglify-js/package.json` & `swanlab-0.3.7/node_modules/uglify-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/uglify-js/node_modules/source-map/package.json` & `swanlab-0.3.7/node_modules/uglify-js/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/uglify-js/tools/domprops.json` & `swanlab-0.3.7/node_modules/uglify-js/tools/domprops.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unbox-primitive/package.json` & `swanlab-0.3.7/node_modules/unbox-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unimport/package.json` & `swanlab-0.3.7/node_modules/unimport/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unimport/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.7/node_modules/unimport/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unimport/node_modules/estree-walker/package.json` & `swanlab-0.3.7/node_modules/unimport/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unimport/node_modules/local-pkg/package.json` & `swanlab-0.3.7/node_modules/unimport/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unplugin/package.json` & `swanlab-0.3.7/node_modules/unplugin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unplugin-auto-import/package.json` & `swanlab-0.3.7/node_modules/unplugin-auto-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json` & `swanlab-0.3.7/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unplugin-auto-import/node_modules/minimatch/package.json` & `swanlab-0.3.7/node_modules/unplugin-auto-import/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unplugin-vue-components/package.json` & `swanlab-0.3.7/node_modules/unplugin-vue-components/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json` & `swanlab-0.3.7/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/unplugin-vue-components/node_modules/minimatch/package.json` & `swanlab-0.3.7/node_modules/unplugin-vue-components/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/update-browserslist-db/.devcontainer.json` & `swanlab-0.3.7/node_modules/update-browserslist-db/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/update-browserslist-db/package.json` & `swanlab-0.3.7/node_modules/update-browserslist-db/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/uri-js/package.json` & `swanlab-0.3.7/node_modules/uri-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/util-deprecate/package.json` & `swanlab-0.3.7/node_modules/util-deprecate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/utrie/package.json` & `swanlab-0.3.7/node_modules/utrie/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vite/package.json` & `swanlab-0.3.7/node_modules/vite/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9781967213114754%*

 * *Differences: {"'devDependencies'": "{'@babel/parser': '^7.24.6', '@rollup/plugin-commonjs': '^25.0.8', "*

 * *                      "'artichokie': '^0.2.1', 'es-module-lexer': '^1.5.3', 'lightningcss': "*

 * *                      "'^1.25.1', 'micromatch': '^4.0.7', 'mlly': '^1.7.0', 'picocolors': "*

 * *                      "'^1.0.1', 'rollup-plugin-dts': '^6.1.1', 'rollup-plugin-license': '^3.4.0', "*

 * *                      "'sass': '^1.77.2'}",*

 * * "'version'": "'5.2.12'"}*

```diff
@@ -11,65 +11,65 @@
         "esbuild": "^0.20.1",
         "postcss": "^8.4.38",
         "rollup": "^4.13.0"
     },
     "description": "Native-ESM powered web dev build tool",
     "devDependencies": {
         "@ampproject/remapping": "^2.3.0",
-        "@babel/parser": "^7.24.5",
+        "@babel/parser": "^7.24.6",
         "@jridgewell/trace-mapping": "^0.3.25",
         "@polka/compression": "^1.0.0-next.25",
         "@rollup/plugin-alias": "^5.1.0",
-        "@rollup/plugin-commonjs": "^25.0.7",
+        "@rollup/plugin-commonjs": "^25.0.8",
         "@rollup/plugin-dynamic-import-vars": "^2.1.2",
         "@rollup/plugin-json": "^6.1.0",
         "@rollup/plugin-node-resolve": "15.2.3",
         "@rollup/plugin-typescript": "^11.1.6",
         "@rollup/pluginutils": "^5.1.0",
         "@types/escape-html": "^1.0.4",
         "@types/pnpapi": "^0.0.5",
         "acorn": "^8.11.3",
         "acorn-walk": "^8.3.2",
-        "artichokie": "^0.2.0",
+        "artichokie": "^0.2.1",
         "cac": "^6.7.14",
         "chokidar": "^3.6.0",
         "connect": "^3.7.0",
         "convert-source-map": "^2.0.0",
         "cors": "^2.8.5",
         "cross-spawn": "^7.0.3",
         "debug": "^4.3.4",
         "dep-types": "link:./src/types",
         "dotenv": "^16.4.5",
         "dotenv-expand": "^11.0.6",
-        "es-module-lexer": "^1.5.2",
+        "es-module-lexer": "^1.5.3",
         "escape-html": "^1.0.3",
         "estree-walker": "^3.0.3",
         "etag": "^1.8.1",
         "fast-glob": "^3.3.2",
         "http-proxy": "^1.18.1",
         "launch-editor-middleware": "^2.6.1",
-        "lightningcss": "^1.24.1",
+        "lightningcss": "^1.25.1",
         "magic-string": "^0.30.10",
-        "micromatch": "^4.0.5",
-        "mlly": "^1.6.1",
+        "micromatch": "^4.0.7",
+        "mlly": "^1.7.0",
         "mrmime": "^2.0.0",
         "open": "^8.4.2",
         "parse5": "^7.1.2",
         "pathe": "^1.1.2",
         "periscopic": "^4.0.2",
-        "picocolors": "^1.0.0",
+        "picocolors": "^1.0.1",
         "picomatch": "^2.3.1",
         "postcss-import": "^16.1.0",
         "postcss-load-config": "^4.0.2",
         "postcss-modules": "^6.0.0",
         "resolve.exports": "^2.0.2",
-        "rollup-plugin-dts": "^6.1.0",
+        "rollup-plugin-dts": "^6.1.1",
         "rollup-plugin-esbuild": "^6.1.1",
-        "rollup-plugin-license": "^3.3.1",
-        "sass": "^1.76.0",
+        "rollup-plugin-license": "^3.4.0",
+        "sass": "^1.77.2",
         "sirv": "^2.0.4",
         "source-map-support": "^0.5.21",
         "strip-ansi": "^7.1.0",
         "strip-literal": "^2.1.0",
         "tsconfck": "^3.0.3",
         "tslib": "^2.6.2",
         "types": "link:./types",
@@ -181,9 +181,9 @@
     "typesVersions": {
         "*": {
             "runtime": [
                 "dist/node/runtime.d.ts"
             ]
         }
     },
-    "version": "5.2.11"
+    "version": "5.2.12"
 }
```

### Comparing `swanlab-0.3.6/node_modules/vite/node_modules/rollup/package.json` & `swanlab-0.3.7/node_modules/vite/node_modules/rollup/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vite-node/package.json` & `swanlab-0.3.7/node_modules/vite-node/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vite-plugin-json5/package.json` & `swanlab-0.3.7/node_modules/vite-plugin-json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vitest/package.json` & `swanlab-0.3.7/node_modules/vitest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vitest/node_modules/local-pkg/package.json` & `swanlab-0.3.7/node_modules/vitest/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue/package.json` & `swanlab-0.3.7/node_modules/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-eslint-parser/package.json` & `swanlab-0.3.7/node_modules/vue-eslint-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-i18n/package.json` & `swanlab-0.3.7/node_modules/vue-i18n/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-i18n/vetur/attributes.json` & `swanlab-0.3.7/node_modules/vue-i18n/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-i18n/vetur/tags.json` & `swanlab-0.3.7/node_modules/vue-i18n/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-router/package.json` & `swanlab-0.3.7/node_modules/vue-router/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-router/vetur/attributes.json` & `swanlab-0.3.7/node_modules/vue-router/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-router/vetur/tags.json` & `swanlab-0.3.7/node_modules/vue-router/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-tippy/package.json` & `swanlab-0.3.7/node_modules/vue-tippy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-tippy/tsconfig.json` & `swanlab-0.3.7/node_modules/vue-tippy/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-tippy/vetur/attributes.json` & `swanlab-0.3.7/node_modules/vue-tippy/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/vue-tippy/vetur/tags.json` & `swanlab-0.3.7/node_modules/vue-tippy/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/webpack-sources/package.json` & `swanlab-0.3.7/node_modules/webpack-sources/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/webpack-virtual-modules/package.json` & `swanlab-0.3.7/node_modules/webpack-virtual-modules/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/which/package.json` & `swanlab-0.3.7/node_modules/which/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/which-boxed-primitive/package.json` & `swanlab-0.3.7/node_modules/which-boxed-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/which-typed-array/package.json` & `swanlab-0.3.7/node_modules/which-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/why-is-node-running/package.json` & `swanlab-0.3.7/node_modules/why-is-node-running/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/window-size/package.json` & `swanlab-0.3.7/node_modules/window-size/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/word-wrap/package.json` & `swanlab-0.3.7/node_modules/word-wrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wordwrap/package.json` & `swanlab-0.3.7/node_modules/wordwrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrap-ansi/package.json` & `swanlab-0.3.7/node_modules/wrap-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrap-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.7/node_modules/wrap-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrap-ansi/node_modules/ansi-styles/package.json` & `swanlab-0.3.7/node_modules/wrap-ansi/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrap-ansi/node_modules/strip-ansi/package.json` & `swanlab-0.3.7/node_modules/wrap-ansi/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrap-ansi-cjs/package.json` & `swanlab-0.3.7/node_modules/wrap-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.7/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json` & `swanlab-0.3.7/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/wrappy/package.json` & `swanlab-0.3.7/node_modules/wrappy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/xml-name-validator/package.json` & `swanlab-0.3.7/node_modules/xml-name-validator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/yaml/package.json` & `swanlab-0.3.7/node_modules/yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/yargs/package.json` & `swanlab-0.3.7/node_modules/yargs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/node_modules/yocto-queue/package.json` & `swanlab-0.3.7/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/env.py` & `swanlab-0.3.7/swanlab/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,21 @@
 """运行模式SWANLAB_MODE，有cloud、local、disabled等模式，针对Callback回调的不同实例化方式，具体效果为：
 1. disabled: 禁用模式，不会上传日志到云端，也不会记录日志，swanlab只会执行解析log的功能，不会输出任何内容到本地
 2. cloud: 云端模式，是云端与本地的混合模式，会上传日志到云端，也会记录日志到本地
 3. cloud-only: 云端模式，只会上传日志到云端，不会记录日志到本地，但是会生成一些临时文件
 4. local: 本地模式，不会上传日志到云端，使用swanlab本地版本
 此外，SWANLAB_MODE为disabled时，会开启非严格模式，非严格模式不再要求文件路径存在
 """
+PACKAGE = "SWANLAB_PACKAGE_PATH"
+"""swanlab包路径SWANLAB_PACKAGE_PATH，用于开发模式下指定swanlab包的路径
+当SWANLAB_DEV为TRUE时，必须指定此路径，否则会抛出异常，非开发模式下此环境变量无效
+"""
+HOME = "SWANLAB_HOME"
+"""存放.swanlab文件夹的路径，用于开发模式下的测试，非开发模式下此环境变量无效
+"""
 
 
 class SwanLabMode(enum.Enum):
     DISABLED = "disabled"
     CLOUD = "cloud"
     # CLOUD_ONLY = "cloud-only"
     LOCAL = "local"
@@ -157,14 +164,15 @@
     if not is_ipv4(_env.get(HOST)):
         raise ValueError('SWANLAB_SERVER_HOST must be an ipv4 address, now is "{host}"'.format(host=_env.get(HOST)))
     return _env.get(HOST)
 
 
 def is_dev(env: Optional[Env] = None) -> bool:
     """判断是否是开发模式
+    此函数会在一开始就被package.py调用，所以不需要判断是否已经初始化
 
     Returns
     -------
     bool
         是否是开发模式
     """
     if _env.get(DEV) is not None:
@@ -175,15 +183,15 @@
     _env[DEV] = env.get(DEV, default=False)
     return _env.get(DEV) == "TRUE"
 
 
 # ---------------------------------- 初始化基础环境变量 ----------------------------------
 
 # 所有的初始化函数
-function_list = [get_mode, get_swanlog_dir, get_server_port, get_server_host, is_dev]
+function_list = [get_mode, get_swanlog_dir, get_server_port, get_server_host]
 
 
 def init_env(env: Optional[Env] = None):
     """初始化环境变量
 
     Parameters
     ----------
@@ -251,31 +259,44 @@
     """获取用户家目录的.swanlab文件夹路径，如果不存在此文件夹就创建
 
     Returns
     -------
     str
         用户家目录的.swanlab文件夹路径
     """
+    if is_dev() and HOME in os.environ:
+        path = os.path.join(os.environ[HOME], ".swanlab")
+        if not assert_exist(path, target_type="folder", ra=False):
+            os.mkdir(path)
+        return path
+
     user_home = get_user_home()
     swanlab_folder = os.path.join(user_home, ".swanlab")
     try:
         if not assert_exist(swanlab_folder, ra=False, target_type="folder"):
             os.mkdir(swanlab_folder)
     except NotADirectoryError:
         os.remove(swanlab_folder)
         os.mkdir(swanlab_folder)
     return swanlab_folder
 
 
+def get_package_path() -> Optional[str]:
+    if is_dev() and PACKAGE in os.environ:
+        return os.environ[PACKAGE]
+    else:
+        return os.path.join(os.path.dirname(__file__), "package.json")
+
+
 def assert_exist(path: str, target_type: str = None, ra: bool = True, desc: str = None, t_desc: str = None) -> bool:
     """
     检查文件是否存在，严格模式下，文件不存在会抛出异常，或者可以手动通过参数控制，存在则返回True，否则返回False
     :param path: 文件路径
     :param target_type: 文件类型(folder, file)，如果文件类型与预期不符，会抛出异常，非严格模式下不检测，为None不检测文件类型
-    :param ra: 文件不存在时是否抛出异常，非严格模式下强制不抛出，此参数无效
+    :param ra: 文件不存在时是否抛出异常，非严格模式下强制不抛出，此参数无效，此参数只影响文件是否存在，不影响文件类型判断时抛出异常
     :param desc: 异常描述信息，非严格模式下强制不抛出，此参数无效
     :param t_desc: 文件类型描述信息，非严格模式下强制不抛出，此参数无效
     """
     if not is_strict_mode():
         return os.path.exists(path)
     if not os.path.exists(path):
         if ra:
```

### Comparing `swanlab-0.3.6/swanlab/error.py` & `swanlab-0.3.7/swanlab/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/package.py` & `swanlab-0.3.7/swanlab/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 @File: swanlab/utils/package.py
 @IDE: vscode
 @Description:
     用于管理swanlab的包管理器的模块，做一些封装
 """
 import json
 import os
-from .env import is_dev, get_swanlab_folder, is_strict_mode
+from .env import get_package_path, get_swanlab_folder, is_strict_mode
 from .utils.key import get_key
 from .error import KeyFileError
+from typing import Optional
+import requests
 
-package_path = None
-if is_dev():
-    # 当前运行时的位置
-    package_path = os.environ['SWANLAB_PACKAGE_PATH']
-else:
-    package_path = os.path.join(os.path.dirname(__file__), "package.json")
+package_path = get_package_path()
 
 
 def get_package_version(p=package_path) -> str:
     """获取swanlab的版本号
 
     Parameters
     ----------
@@ -35,14 +32,27 @@
         swanlab的版本号
     """
     # 读取package.json文件
     with open(p, "r") as f:
         return json.load(f)["version"]
 
 
+def get_package_latest_version(timeout=0.5) -> Optional[str]:
+    url = "https://pypi.org/pypi/swanlab/json"
+    try:
+        response = requests.get(url, timeout=timeout)
+        if response.status_code == 200:
+            data = response.json()
+            return data["info"]["version"]
+        else:
+            return None
+    except Exception as e:
+        return None
+
+
 def get_host_web(p: str = package_path) -> str:
     """获取swanlab网站网址
 
     Parameters
     ----------
     p : str, optional
         package.json文件路径，默认为项目的package.json
@@ -158,23 +168,27 @@
     if os.path.exists(os.path.join(path, "project.json")):
         with open(os.path.join(path, "project.json"), "r") as f:
             project = json.load(f)
             # print(project.get("version"))
             if project.get("version") is not None:
                 # 报错，当前目录只允许v0.1.5之前的版本，请降级到v0.1.4
                 if mode == "watch":
-                    info = ("The version of logdir is old (Created by swanlab<=0.1.4), the current version of "
-                            "SwanLab doesn't support this logfile. If you need to watch this logfile, please use the "
-                            "transfer script: https://github.com/SwanHubX/SwanLab/blob/main/script/transfer_logfile_0"
-                            ".1.4.py'")
+                    info = (
+                        "The version of logdir is old (Created by swanlab<=0.1.4), the current version of "
+                        "SwanLab doesn't support this logfile. If you need to watch this logfile, please use the "
+                        "transfer script: https://github.com/SwanHubX/SwanLab/blob/main/script/transfer_logfile_0"
+                        ".1.4.py'"
+                    )
                 elif mode == "init":
-                    info = ("The version of logdir is old (Created by swanlab<=0.1.4), the current version of "
-                            "SwanLab doesn't support this logfile. If you need to continue train in this logdir, "
-                            "please use the transfer script: "
-                            "https://github.com/SwanHubX/SwanLab/blob/main/script/transfer_logfile_0.1.4.py'")
+                    info = (
+                        "The version of logdir is old (Created by swanlab<=0.1.4), the current version of "
+                        "SwanLab doesn't support this logfile. If you need to continue train in this logdir, "
+                        "please use the transfer script: "
+                        "https://github.com/SwanHubX/SwanLab/blob/main/script/transfer_logfile_0.1.4.py'"
+                    )
                 else:
                     info = "version_limit function only support mode in ['watch', 'init']"
                 raise ValueError(info)
     return
 
 
 def is_login() -> bool:
```

### Comparing `swanlab-0.3.6/swanlab/api/cos.py` & `swanlab-0.3.7/swanlab/api/cos.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 """
 # noinspection PyPackageRequirements
 from qcloud_cos import CosConfig
 # noinspection PyPackageRequirements
 from qcloud_cos import CosS3Client
 # noinspection PyPackageRequirements
 from qcloud_cos.cos_threadpool import SimpleThreadPool
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import List, Dict, Union
 
 
 class CosClient:
     REFRESH_TIME = 60 * 60 * 1.5  # 1.5小时
 
     def __init__(self, data):
+        """
+        初始化cos客户端
+        """
         self.__expired_time = datetime.fromtimestamp(data["expiredTime"])
         self.__prefix = data["prefix"]
         self.__bucket = data["bucket"]
         credentials = data["credentials"]
         config = CosConfig(
             Region=data["region"],
             SecretId=credentials['tmpSecretId'],
@@ -62,8 +65,13 @@
             pool.add_task(self.upload, key, local_path)
         pool.wait_completion()
         result = pool.get_result()
         return result
 
     @property
     def should_refresh(self):
-        return (self.__expired_time - datetime.utcnow()).seconds < self.REFRESH_TIME
+        # cos传递的是北京时间，需要添加8小时
+        now = datetime.utcnow() + timedelta(hours=8)
+        # 过期时间减去当前时间小于刷新时间，需要注意为负数的情况
+        if self.__expired_time < now:
+            return True
+        return (self.__expired_time - now).seconds < self.REFRESH_TIME
```

### Comparing `swanlab-0.3.6/swanlab/api/http.py` & `swanlab-0.3.7/swanlab/api/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,18 @@
     def username(self):
         """
         当前登录的用户名
         """
         return self.__login_info.username
 
     @property
+    def cos(self):
+        return self.__cos
+
+    @property
     def proj_id(self):
         return self.__proj.cuid
 
     @property
     def projname(self):
         return self.__proj.name
 
@@ -171,14 +175,15 @@
         """
         批量上传文件，keys和local_paths的长度应该相等
         :param keys: 上传到cos
         :param local_paths: 本地文件路径，需用绝对路径
         :return: 返回上传结果, 包含success_all和detail两个字段，detail为每一个文件的上传结果（通过index索引对应）
         """
         if self.__cos.should_refresh:
+            swanlog.debug("Refresh cos...")
             self.__get_cos()
         keys = [key[1:] if key.startswith("/") else key for key in keys]
         return self.__cos.upload_files(keys, local_paths)
 
     def mount_project(self, name: str, username: str = None) -> ProjectInfo:
         self.__username = self.__username if username is None else username
 
@@ -212,17 +217,19 @@
         """
 
         def _():
             """
             先创建实验，后生成cos凭证
             :return:
             """
+
             data = self.post(
                 f"/project/{self.groupname}/{self.__proj.name}/runs",
-                {"name": exp_name, "colors": list(colors), "description": description},
+                {"name": exp_name, "colors": list(colors), "description": description} if description else {
+                    "name": exp_name, "colors": list(colors)}
             )
             self.__exp = ExperimentInfo(data)
             # 获取cos信息
             self.__get_cos()
 
         FONT.loading("Creating experiment...", _)
 
@@ -231,15 +238,15 @@
         更新实验状态
         :param success: 实验是否成功
         """
 
         def _():
             self.put(
                 f"/project/{self.groupname}/{self.projname}/runs/{self.exp_id}/state",
-                {"state": "FINISHED" if success else "CRASHED"},
+                {"state": "FINISHED" if success else "CRASHED", "from": "sdk"},
             )
 
         FONT.loading("Updating experiment status...", _)
 
 
 http: Optional["HTTP"] = None
 """
```

### Comparing `swanlab-0.3.6/swanlab/api/info.py` & `swanlab-0.3.7/swanlab/api/info.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/api/auth/login.py` & `swanlab-0.3.7/swanlab/api/auth/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     return login_info
 
 
 def terminal_login(api_key: str = None) -> LoginInfo:
     """
     终端登录，此时直接覆盖本地token文件，但是新增交互，让用户输入api_key
     运行此函数，如果是认证失败的错误，重新要求用户输入api_key
+    本地文件上层文件夹不保证存在，需要上层函数保证
     """
     # 1. api_key存在，跳过输入环节，直接请求登录接口，这与代码内swanlab.login方法一致
     # 2. api_key为None，提示用户输入
     input_key = api_key is None
     if api_key is None:
         api_key = input_api_key()
     while True:
```

### Comparing `swanlab-0.3.6/swanlab/api/upload/__init__.py` & `swanlab-0.3.7/swanlab/api/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/api/upload/model.py` & `swanlab-0.3.7/swanlab/api/upload/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cli/main.py` & `swanlab-0.3.7/swanlab/cli/main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cli/utils.py` & `swanlab-0.3.7/swanlab/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cloud/_log_collector.py` & `swanlab-0.3.7/swanlab/cloud/_log_collector.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cloud/start_thread.py` & `swanlab-0.3.7/swanlab/cloud/start_thread.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cloud/task_types.py` & `swanlab-0.3.7/swanlab/cloud/task_types.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cloud/utils.py` & `swanlab-0.3.7/swanlab/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cloud/dog/log_sniffer.py` & `swanlab-0.3.7/swanlab/cloud/dog/log_sniffer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cloud/dog/metadata_handle.py` & `swanlab-0.3.7/swanlab/cloud/dog/metadata_handle.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/cloud/dog/sniffer_queue.py` & `swanlab-0.3.7/swanlab/cloud/dog/sniffer_queue.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/compat/server/controller/experiment.py` & `swanlab-0.3.7/swanlab/compat/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/converter/tfb/_utils.py` & `swanlab-0.3.7/swanlab/converter/tfb/_utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/converter/tfb/tfb_converter.py` & `swanlab-0.3.7/swanlab/converter/tfb/tfb_converter.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/converter/wb/wb_converter.py` & `swanlab-0.3.7/swanlab/converter/wb/wb_converter.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/__init__.py` & `swanlab-0.3.7/swanlab/data/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/callback_cloud.py` & `swanlab-0.3.7/swanlab/data/callback_cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 from swanlab.package import get_host_web, get_host_api
 from swanlab.error import KeyFileError
 from swanlab.env import get_swanlab_folder
 from .callback_local import LocalRunCallback, get_run, SwanLabRunState
 from swanlab.cloud import LogSnifferTask, ThreadPool
 from swanlab.db import Experiment
 from swanlab.utils import create_time
+from swanlab.package import get_package_version, get_package_latest_version
 import sys
 import os
+import io
 
 
 class CloudRunCallback(LocalRunCallback):
     login_info: LoginInfo = None
     """
     用户登录信息
     """
@@ -49,20 +51,35 @@
         """
         发起登录，获取登录信息，执行此方法会覆盖原有的login_info
         """
         key = None
         try:
             key = get_key(os.path.join(get_swanlab_folder(), ".netrc"), get_host_api())[2]
         except KeyFileError:
-            fd = sys.stdin.fileno()
-            # 不是标准终端，且非jupyter环境，无法控制其回显
-            if not os.isatty(fd) and not in_jupyter():
-                raise KeyFileError("The key file is not found, call `swanlab.login()` or use `swanlab login` ")
+            try:
+                fd = sys.stdin.fileno()
+                # 不是标准终端，且非jupyter环境，无法控制其回显
+                if not os.isatty(fd) and not in_jupyter():
+                    raise KeyFileError("The key file is not found, call `swanlab.login()` or use `swanlab login` ")
+            # 当使用capsys、capfd或monkeypatch等fixture来捕获或修改标准输入输出时，会抛出io.UnsupportedOperation
+            # 这种情况下为用户自定义情况
+            except io.UnsupportedOperation:
+                pass
         return terminal_login(key)
 
+    @staticmethod
+    def _get_package_latest_version():
+        """
+        cloud模式训练开始时，检测package是否为最新版本
+        """
+        latest_version = get_package_latest_version()
+        local_version = get_package_version()
+        if latest_version is not None and latest_version != local_version:
+            swanlog.info(f"swanlab version {latest_version} is available!  Upgrade: `pip install -U swanlab`")
+
     def _view_web_print(self):
         self._watch_tip_print()
         http = get_http()
         project_url = get_host_web() + f"/@{http.groupname}/{http.projname}"
         experiment_url = project_url + f"/runs/{http.exp_id}"
         swanlog.info("🏠 View project at " + FONT.blue(FONT.underline(project_url)))
         swanlog.info("🚀 View run at " + FONT.blue(FONT.underline(experiment_url)))
@@ -91,17 +108,20 @@
             raise tp(val)
 
     def __str__(self):
         return "SwanLabCloudRunCallback"
 
     def on_init(self, project: str, workspace: str, logdir: str = None) -> int:
         super(CloudRunCallback, self).on_init(project, workspace, logdir)
+        # 检测是否有最新的版本
+        self._get_package_latest_version()
         if self.login_info is None:
             swanlog.debug("Login info is None, get login info.")
             self.login_info = self.get_login_info()
+
         http = create_http(self.login_info)
         return http.mount_project(project, workspace).history_exp_count
 
     def on_run(self):
         swanlog.install(self.settings.console_dir)
         # 注册实验信息
         try:
@@ -136,27 +156,26 @@
         experiment_url = self._view_web_print()
 
         # 在Jupyter Notebook环境下，显示按钮
         if in_jupyter():
             show_button_html(experiment_url)
 
     def on_column_create(self, column_info: ColumnInfo):
-        self.pool.queue.put((
-            UploadType.COLUMN,
-            [ColumnModel(column_info.key, column_info.data_type.upper(), column_info.error)]
-        ))
+        self.pool.queue.put(
+            (UploadType.COLUMN, [ColumnModel(column_info.key, column_info.data_type.upper(), column_info.error)])
+        )
 
     def on_metric_create(self, metric_info: MetricInfo):
         super(CloudRunCallback, self).on_metric_create(metric_info)
         if metric_info.error:
             return
         new_data = metric_info.metric
-        new_data['key'] = metric_info.key
-        new_data['index'] = metric_info.step
-        new_data['epoch'] = metric_info.epoch
+        new_data["key"] = metric_info.key
+        new_data["index"] = metric_info.step
+        new_data["epoch"] = metric_info.epoch
         if metric_info.data_type == "default":
             return self.pool.queue.put((UploadType.SCALAR_METRIC, [new_data]))
         key = quote(metric_info.key, safe="")
         data = (new_data, key, metric_info.data_type, metric_info.static_dir)
         self.pool.queue.put((UploadType.MEDIA_METRIC, [data]))
 
     def on_stop(self, error: str = None):
```

### Comparing `swanlab-0.3.6/swanlab/data/callback_local.py` & `swanlab-0.3.7/swanlab/data/callback_local.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/config.py` & `swanlab-0.3.7/swanlab/data/config.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/sdk.py` & `swanlab-0.3.7/swanlab/data/sdk.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/settings.py` & `swanlab-0.3.7/swanlab/data/settings.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/_utils.py` & `swanlab-0.3.7/swanlab/data/modules/_utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/audio.py` & `swanlab-0.3.7/swanlab/data/modules/audio.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/base.py` & `swanlab-0.3.7/swanlab/data/modules/base.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/chart.py` & `swanlab-0.3.7/swanlab/data/modules/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/image.py` & `swanlab-0.3.7/swanlab/data/modules/image.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/object_3d.py` & `swanlab-0.3.7/swanlab/data/modules/object_3d.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/text.py` & `swanlab-0.3.7/swanlab/data/modules/text.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/video.py` & `swanlab-0.3.7/swanlab/data/modules/video.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/utils_modules/bounding_boxes.py` & `swanlab-0.3.7/swanlab/data/modules/utils_modules/bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/modules/utils_modules/image_mask.py` & `swanlab-0.3.7/swanlab/data/modules/utils_modules/image_mask.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/run/callback.py` & `swanlab-0.3.7/swanlab/data/run/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         key: str,
         namespace: str,
         data_type: str,
         chart_type: str,
         sort: int,
         error: Optional[Dict] = None,
         reference: Optional[str] = None,
-        config: Optional[Dict] = None
+        config: Optional[Dict] = None,
     ):
         self.key = key
         """
         列的key名称
         """
         self.namespace = namespace
         """
@@ -83,15 +83,15 @@
         summary: Union[Dict, None] = None,
         data_type: Union[float, DataType] = None,
         step: int = None,
         epoch: int = None,
         metric_path: str = None,
         summary_path: str = None,
         static_dir: str = None,
-        error: bool = True
+        error: bool = True,
     ):
         self.key = key
         """
         指标的key名称
         """
         self.column_info = column_info
         """
@@ -253,15 +253,15 @@
     def before_init_experiment(
         self,
         run_id: str,
         exp_name: str,
         description: str,
         num: int,
         suffix: str,
-        setter: Callable[[str, str, str, str], None]
+        setter: Callable[[str, str, str, str], None],
     ):
         """
         在初始化实验之前调用，此时SwanLabRun已经初始化完毕
         :param run_id: str, SwanLabRun的运行id
         :param exp_name: str, 实验名称
         :param description: str, 实验描述
         :param num: int, 历史实验数量
```

### Comparing `swanlab-0.3.6/swanlab/data/run/exp.py` & `swanlab-0.3.7/swanlab/data/run/exp.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,14 +209,19 @@
         return self.__error is None
 
     @staticmethod
     def __is_nan(data):
         """判断data是否为nan"""
         return isinstance(data, (int, float)) and math.isnan(data)
 
+    @staticmethod
+    def __is_inf(data):
+        """判断data是否为inf"""
+        return isinstance(data, (int, float)) and math.isinf(data)
+
     def add(self, data: DataType, step: int = None) -> MetricInfo:
         """添加一个数据，在内部完成数据类型转换
         如果转换失败，打印警告并退出
         并且添加数据，当前的数据保存是直接保存，后面会改成缓存形式
 
         Parameters
         ----------
@@ -246,28 +251,32 @@
         except ValueError:
             swanlog.warning(
                 f"Log failed. Reason: Data {data} on tag '{self.tag}' (step {step}) cannot be converted .It should be "
                 f"an int, float, or a DataType, but it is {type(data)}, please check the data type."
             )
             return MetricInfo(self.tag, self.__column_info)
         is_nan = self.__is_nan(data)
+        is_inf = self.__is_inf(data)
         # 更新数据概要
-        if not is_nan:
+        if not is_nan and not is_inf:
             if self._summary.get("max") is None or data > self._summary["max"]:
                 self._summary["max"] = data
                 self._summary["max_step"] = step
             if self._summary.get("min") is None or data < self._summary["min"]:
                 self._summary["min"] = data
                 self._summary["min_step"] = step
         self._summary["num"] = self._summary.get("num", 0) + 1
         self.__steps.add(step)
         swanlog.debug(f"Add data, tag: {self.tag}, step: {step}, data: {data}")
         if len(self.__data["data"]) >= self.__slice_size:
             self.__data = self.__new_tags()
+
         data = data if not is_nan else "NaN"
+        data = data if not is_inf else "INF"
+
         new_data = self.__new_tag(step, data, more=more)
         self.__data["data"].append(new_data)
         epoch = len(self.__steps)
         mu = math.ceil(epoch / self.__slice_size)
         file_path = os.path.join(self.save_path, str(mu * self.__slice_size) + ".log")
         return MetricInfo(
             self.tag,
@@ -339,14 +348,17 @@
                     excepted = data.expect_types()
                 else:
                     class_name = data.__class__.__name__
                     excepted = [i.__name__ for i in self.data_types]
                 error = {"data_class": class_name, "excepted": excepted}
         if self.__is_nan(data):
             error = {"data_class": "NaN", "excepted": [i.__name__ for i in self.data_types]}
+        if self.__is_inf(data):
+            error = {"data_class": "INF", "excepted": [i.__name__ for i in self.data_types]}
+
         column_info = ColumnInfo(tag, namespace, data_type, chart_type, sort, error, reference, config)
         self.__error = error
         self.data_type = data_type
         self.__column_info = column_info
         return column_info
 
     @staticmethod
```

### Comparing `swanlab-0.3.6/swanlab/data/run/main.py` & `swanlab-0.3.7/swanlab/data/run/main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/run/operator.py` & `swanlab-0.3.7/swanlab/data/run/operator.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/system/info.py` & `swanlab-0.3.7/swanlab/data/system/info.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/system/monitor.py` & `swanlab-0.3.7/swanlab/data/system/monitor.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/data/system/bin/apple_gpu_stats` & `swanlab-0.3.7/swanlab/data/system/bin/apple_gpu_stats`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/__init__.py` & `swanlab-0.3.7/swanlab/db/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/callback.py` & `swanlab-0.3.7/swanlab/db/callback.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/db_connect.py` & `swanlab-0.3.7/swanlab/db/db_connect.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/error.py` & `swanlab-0.3.7/swanlab/db/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/model.py` & `swanlab-0.3.7/swanlab/db/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/docs/Errors.md` & `swanlab-0.3.7/swanlab/db/docs/Errors.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/docs/README.md` & `swanlab-0.3.7/swanlab/db/docs/README.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/migrate/chart.py` & `swanlab-0.3.7/swanlab/db/migrate/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/migrate/experiment.py` & `swanlab-0.3.7/swanlab/db/migrate/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/migrate/namespace.py` & `swanlab-0.3.7/swanlab/db/migrate/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/migrate/project.py` & `swanlab-0.3.7/swanlab/db/migrate/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/models/charts.py` & `swanlab-0.3.7/swanlab/db/models/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/models/displays.py` & `swanlab-0.3.7/swanlab/db/models/displays.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/models/experiments.py` & `swanlab-0.3.7/swanlab/db/models/experiments.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/models/namespaces.py` & `swanlab-0.3.7/swanlab/db/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/models/projects.py` & `swanlab-0.3.7/swanlab/db/models/projects.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/models/sources.py` & `swanlab-0.3.7/swanlab/db/models/sources.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/models/tags.py` & `swanlab-0.3.7/swanlab/db/models/tags.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/db/utils/chart.py` & `swanlab-0.3.7/swanlab/db/utils/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/integration/fastai.py` & `swanlab-0.3.7/swanlab/integration/fastai.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,52 +7,53 @@
     from fastcore.basics import store_attr, detuplify, ignore_exceptions
     from fastai.callback.hook import total_params
 except ImportError:
     raise RuntimeError(
         "This module requires `fastai` to be installed. " "Please install it with command: \n pip install fastai"
     )
 
-from typing import Optional
+from typing import Optional, Any
 import swanlab
 from swanlab.log import swanlog as swl
 
 
 class SwanLabCallback(Callback):
     def __init__(
         self,
         project: Optional[str] = None,
         experiment_name: Optional[str] = None,
         description: Optional[str] = None,
         workspace: Optional[str] = None,
         config: Optional[dict] = None,
-        cloud: Optional[bool] = True,
+        mode: Optional[str] = None,
         logdir: Optional[str] = None,
+        **kwargs: Any,
     ):
         store_attr()
         self._experiment = swanlab
 
         self.project = project
         self.experiment_name = experiment_name
         self.workspace = workspace
         self.config = config
         self.description = description
-        self.cloud = cloud
+        self.mode = mode
         self.logdir = logdir
         self.train_suffix = "train"
         self.summary_suffix = "summary"
 
     def setup_swanlab(self):
         if self._experiment.get_run() is None:
             self._experiment.init(
                 project=self.project,
                 workspace=self.workspace,
                 experiment_name=self.experiment_name,
                 description=self.description,
                 config=self.config,
-                cloud=self.cloud,
+                mode=self.mode,
                 logdir=self.logdir,
             )
 
     def before_fit(self):
         # print("=" * 10 + "before_fit" + "=" * 10)
         self.setup_swanlab()
         configs_log = self.gather_args()
```

### Comparing `swanlab-0.3.6/swanlab/integration/huggingface.py` & `swanlab-0.3.7/swanlab/integration/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,37 +34,37 @@
     def __init__(
         self,
         project: Optional[str] = None,
         workspace: Optional[str] = None,
         experiment_name: Optional[str] = None,
         description: Optional[str] = None,
         logdir: Optional[str] = None,
-        cloud: Optional[bool] = True,
+        mode: Optional[str] = None,
         **kwargs: Any,
     ):
         self._initialized = False
         self._experiment = swanlab
 
         self._swanlab_init: Dict[str, Any] = {
             "project": project,
             "workspace": workspace,
             "experiment_name": experiment_name,
             "description": description,
             "logdir": logdir,
-            "cloud": cloud,
+            "mode": mode,
         }
 
         self._swanlab_init.update(**kwargs)
 
         self._project = self._swanlab_init.get("project")
         self._workspace = self._swanlab_init.get("workspace")
         self._experiment_name = self._swanlab_init.get("experiment_name")
         self._description = self._swanlab_init.get("decsription")
         self._logdir = self._swanlab_init.get("logdir")
-        self._cloud = self._swanlab_init.get("cloud")
+        self._mode = self._swanlab_init.get("mode")
 
     def setup(self, args, state, model, **kwargs):
         self._initialized = True
 
         if not state.is_world_process_zero:
             return
```

### Comparing `swanlab-0.3.6/swanlab/integration/mmengine.py` & `swanlab-0.3.7/swanlab/integration/mmengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         type="SwanlabVisBackend",
         save_dir="./swanlog_save_path",             # swanlab save path
         init_kwargs={                               # swanlab.init args
             "project": "YourProject ",              # project name on swanlab
             "experiment_name": "YourExperiment",    # experiment name on swanlab
             "description": "have fun",              # experiment description (can be null)
             "workspace": "YourOrganization",        # Your Organization on swanlab
-            # "cloud": False,                       # Upload to cloud
+            # "mode": "cloud",                       # Upload to cloud
         },
     ),
 ]
 ...
 ---------------------------------
 """
```

### Comparing `swanlab-0.3.6/swanlab/integration/pytorch_lightning.py` & `swanlab-0.3.7/swanlab/integration/pytorch_lightning.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,37 +53,37 @@
     def __init__(
         self,
         project: Optional[str] = None,
         workspace: Optional[str] = None,
         experiment_name: Optional[str] = None,
         description: Optional[str] = None,
         logdir: Optional[str] = None,
-        cloud: Optional[bool] = True,
+        mode: Optional[str] = None,
         save_dir: Union[str, Path] = ".",
         **kwargs: Any,
     ):
         super().__init__()
 
         self._swanlab_init: Dict[str, Any] = {
             "project": project,
             "workspace": workspace,
             "experiment_name": experiment_name,
             "description": description,
             "logdir": logdir,
-            "cloud": cloud,
+            "mode": mode,
         }
 
         self._swanlab_init.update(**kwargs)
 
         self._project = self._swanlab_init.get("project")
         self._workspace = self._swanlab_init.get("workspace")
         self._experiment_name = self._swanlab_init.get("experiment_name")
         self._description = self._swanlab_init.get("decsription")
         self._logdir = self._swanlab_init.get("logdir")
-        self._cloud = self._swanlab_init.get("cloud")
+        self._mode = self._swanlab_init.get("mode")
 
         if save_dir is not None:
             save_dir = os.fspath(save_dir)
         self._save_dir = save_dir
 
     @property
     @rank_zero_experiment
```

### Comparing `swanlab-0.3.6/swanlab/integration/sb3.py` & `swanlab-0.3.7/swanlab/integration/sb3.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,38 +66,38 @@
     def __init__(
         self,
         project: Optional[str] = None,
         workspace: Optional[str] = None,
         experiment_name: Optional[str] = None,
         description: Optional[str] = None,
         logdir: Optional[str] = None,
-        cloud: Optional[bool] = True,
+        mode: Optional[bool] = None,
         verbose: int = 0,
         **kwargs: Any,
     ):
         super().__init__(verbose)
         self._run = None
 
         self._swanlab_init: Dict[str, Any] = {
             "project": project,
             "workspace": workspace,
             "experiment_name": experiment_name,
             "description": description,
             "logdir": logdir,
-            "cloud": cloud,
+            "mode": mode,
         }
 
         self._swanlab_init.update(**kwargs)
 
         self._project = self._swanlab_init.get("project")
         self._workspace = self._swanlab_init.get("workspace")
         self._experiment_name = self._swanlab_init.get("experiment_name")
         self._description = self._swanlab_init.get("decsription")
         self._logdir = self._swanlab_init.get("logdir")
-        self._cloud = self._swanlab_init.get("cloud")
+        self._mode = self._swanlab_init.get("mode")
 
     def _init_callback(self) -> None:
         args = {"algo": type(self.model).__name__}
         for key in self.model.__dict__:
             if type(self.model.__dict__[key]) in [float, int, str]:
                 args[key] = self.model.__dict__[key]
             else:
```

### Comparing `swanlab-0.3.6/swanlab/integration/integration_utils/autologging.py` & `swanlab-0.3.7/swanlab/integration/integration_utils/autologging.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,24 +175,24 @@
     def __init__(
         self,
         name: str,
         symbols: Sequence[str],
         resolver: ArgumentResponseResolver,
         client=None,
         lib_version=None,
-        cloud: bool = True,
+        mode: str = None,
     ) -> None:
         """Autolog API calls to SwanLab."""
 
         self._patch_api = PatchAPI(
             name=name, symbols=symbols, resolver=resolver, client=client, lib_version=lib_version
         )
         self._name = self._patch_api.name
         self._run: Optional[SwanLabRun] = None
-        self.cloud = cloud
+        self.mode = mode
         self.client: openai.Client = client
         self.lib_version = lib_version
 
     @property
     def _is_enabled(self) -> bool:
         """Returns whether autologging is enabled."""
         return self._run is not None
```

### Comparing `swanlab-0.3.6/swanlab/integration/integration_utils/get_modules.py` & `swanlab-0.3.7/swanlab/integration/integration_utils/get_modules.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/integration/integration_utils/timer.py` & `swanlab-0.3.7/swanlab/integration/integration_utils/timer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/integration/openai/openai.py` & `swanlab-0.3.7/swanlab/integration/openai/openai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/integration/openai/resolver.py` & `swanlab-0.3.7/swanlab/integration/openai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/integration/zhipuai/resolver.py` & `swanlab-0.3.7/swanlab/integration/zhipuai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/integration/zhipuai/zhipuai.py` & `swanlab-0.3.7/swanlab/integration/zhipuai/zhipuai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/log/console.py` & `swanlab-0.3.7/swanlab/log/console.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/log/log.py` & `swanlab-0.3.7/swanlab/log/log.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/app.py` & `swanlab-0.3.7/swanlab/server/app.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/settings.py` & `swanlab-0.3.7/swanlab/server/settings.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/controller/chart.py` & `swanlab-0.3.7/swanlab/server/controller/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/controller/experiment.py` & `swanlab-0.3.7/swanlab/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/controller/namespace.py` & `swanlab-0.3.7/swanlab/server/controller/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/controller/project.py` & `swanlab-0.3.7/swanlab/server/controller/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/controller/utils/__init__.py` & `swanlab-0.3.7/swanlab/server/controller/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/controller/utils/charts.py` & `swanlab-0.3.7/swanlab/server/controller/utils/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/controller/utils/tag.py` & `swanlab-0.3.7/swanlab/server/controller/utils/tag.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/middleware/common.py` & `swanlab-0.3.7/swanlab/server/middleware/common.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/module/resp.py` & `swanlab-0.3.7/swanlab/server/module/resp.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/router/chart.py` & `swanlab-0.3.7/swanlab/server/router/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/router/experiment.py` & `swanlab-0.3.7/swanlab/server/router/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/router/media.py` & `swanlab-0.3.7/swanlab/server/router/media.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/router/namespace.py` & `swanlab-0.3.7/swanlab/server/router/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/server/router/project.py` & `swanlab-0.3.7/swanlab/server/router/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/ChartPage-C2Rj7xI3.js` & `swanlab-0.3.7/swanlab/template/assets/ChartPage-BqfnvJQ4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,22 +7,22 @@
     h as i,
     k as c,
     o as n,
     a as l,
     e as h,
     d as u,
     f as o
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     C as p,
     u as _,
     a as d,
     m
-} from "./chart-eW1meEc1.js";
-import "./SLLoading-6DfF2aH0.js";
+} from "./chart-Cb2YjpB3.js";
+import "./SLLoading-B-49YNim.js";
 const g = {
         key: 0,
         class: "chart-page"
     },
     M = {
         key: 0,
         class: "font-semibold pt-5 text-center"
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/ChartsView-DpI6U3QH.js` & `swanlab-0.3.7/swanlab/template/assets/ChartsView-DKnkZV4x.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,22 +4,22 @@
     o as t,
     g as r,
     d as s,
     h as o,
     i as l,
     a as u,
     f as n
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     u as c,
     a as p,
     m as h,
     C as i
-} from "./chart-eW1meEc1.js";
-import "./SLLoading-6DfF2aH0.js";
+} from "./chart-Cb2YjpB3.js";
+import "./SLLoading-B-49YNim.js";
 const d = {
         __name: "ChartsPage",
         props: {
             groups: {
                 type: Array,
                 required: !0
             },
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/EnvHardware-4H7mp2Bs.js` & `swanlab-0.3.7/swanlab/template/assets/EnvHardware-Dh6G7EyN.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -8,18 +8,18 @@
     F as n,
     s as m,
     f as p,
     O as u,
     c as o,
     e as i,
     g as c
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     E as d
-} from "./EnvItems-B4PwmQT4.js";
+} from "./EnvItems-z9WBoR8b.js";
 const v = {
         key: 0,
         class: "flex flex-col gap-y-4 pt-4"
     },
     y = {
         class: "w-full flex"
     },
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/EnvIndex-B5_l1b65.js` & `swanlab-0.3.7/swanlab/template/assets/EnvIndex-3qdPSvC8.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -8,18 +8,18 @@
     b as s,
     t as n,
     d as u,
     F as r,
     s as g,
     B as m,
     g as v
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     E as d
-} from "./EnvItems-B4PwmQT4.js";
+} from "./EnvItems-z9WBoR8b.js";
 const y = {
         class: "w-full border p-6 rounded-lg bg-default"
     },
     h = {
         class: "w-full text-xl font-semibold pb-4 border-b mb-2"
     },
     c = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/EnvItems-B4PwmQT4.js` & `swanlab-0.3.7/swanlab/template/assets/EnvItems-z9WBoR8b.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     q as o,
     al as u,
     m as r,
     C as p,
     c as v,
     F as y,
     s as c
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 const d = {
         key: 0,
         class: "w-full flex relative"
     },
     h = {
         class: "text-dimmer w-44 shrink-0"
     },
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/EnvItems-BfjcRO-X.css` & `swanlab-0.3.7/swanlab/template/assets/EnvItems-BfjcRO-X.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js` & `swanlab-0.3.7/swanlab/template/assets/EnvRequirements-B26RqDqU.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -14,18 +14,18 @@
     F as v,
     s as m,
     f as p,
     T as f,
     aj as b,
     q as x,
     C as h
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     F as g
-} from "./FuncBar-Ct_nBdvU.js";
+} from "./FuncBar-Chts8yho.js";
 const w = {
         key: 0,
         class: "w-full border p-6 rounded-lg bg-default"
     },
     y = {
         class: "flex items-center justify-between border-b pb-4 mb-5"
     },
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js` & `swanlab-0.3.7/swanlab/template/assets/EnvironmentPage-DLnE8Co5.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     w as r,
     b as i,
     t as c,
     C as u,
     L as d,
     q as h,
     d as p
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 const m = {
         class: "lg:w-48 lg:h-auto lg:px-4 lg:transition-none px-6 w-0 h-0 transition-all overflow-hidden"
     },
     v = e({
         __name: "SiderNav",
         setup(e) {
             const d = [{
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/ExperimentView-BTbu21ka.js` & `swanlab-0.3.7/swanlab/template/assets/ExperimentView-x-2IwSHi.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -24,21 +24,21 @@
     c as w,
     q as I,
     N as $,
     O as S,
     P as E,
     g as k,
     Q as L
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     _ as R,
     D as j,
     a as C
-} from "./SLStatusLabel-DvEKZN8v.js";
-import "./SLLoading-6DfF2aH0.js";
+} from "./SLStatusLabel-DNkFoo89.js";
+import "./SLLoading-B-49YNim.js";
 const F = {
         class: "w-full h-full py-5"
     },
     N = {
         class: "px-6 border-b"
     },
     D = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/ExperimentView-CCDMXo4h.css` & `swanlab-0.3.7/swanlab/template/assets/ExperimentView-CCDMXo4h.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/FuncBar-Ct_nBdvU.js` & `swanlab-0.3.7/swanlab/template/assets/FuncBar-Chts8yho.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     H as i,
     al as p,
     m as f,
     A as m,
     at as w,
     C as g,
     D as x
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 const h = {
         class: "w-full flex justify-between gap-5"
     },
     v = {
         class: "flex items-center w-full"
     },
     y = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/HomeView-BS7FyMAt.css` & `swanlab-0.3.7/swanlab/template/assets/HomeView-BS7FyMAt.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/HomeView-BqTu9_fG.js` & `swanlab-0.3.7/swanlab/template/assets/HomeView-uDUGPxwP.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -34,21 +34,21 @@
     C as I,
     D as M,
     E as C,
     G as H,
     H as R,
     I as z,
     J as U
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     _ as W,
     D as q,
     a as D
-} from "./SLStatusLabel-DvEKZN8v.js";
-import "./SLLoading-6DfF2aH0.js";
+} from "./SLStatusLabel-DNkFoo89.js";
+import "./SLLoading-B-49YNim.js";
 const G = {
         class: "w-full h-full pt-5 flex flex-col"
     },
     N = {
         class: "px-6 border-b flex-shrink-0"
     },
     O = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/IndexPage-C5dvtib2.css` & `swanlab-0.3.7/swanlab/template/assets/IndexPage-C5dvtib2.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/IndexPage-CrqN4Ekl.js` & `swanlab-0.3.7/swanlab/template/assets/IndexPage-Jy4F58Oh.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,15 @@
     e as p,
     w as m,
     H as y,
     D as f,
     S as x,
     h as g,
     E as b
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 const k = {
         class: "w-full px-6 pb-2 text-default relative"
     },
     h = {
         class: "flex justify-between pt-6 pb-2 flex-wrap"
     },
     w = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf` & `swanlab-0.3.7/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/LogPage-B-fC6sB7.js` & `swanlab-0.3.7/swanlab/template/assets/LogPage-D3SdB10-.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -20,21 +20,21 @@
     t as f,
     T as y,
     aj as w,
     v as b,
     x as k,
     ao as S,
     C as j
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     _ as L
-} from "./SLLoading-6DfF2aH0.js";
+} from "./SLLoading-B-49YNim.js";
 import {
     F as T
-} from "./FuncBar-Ct_nBdvU.js";
+} from "./FuncBar-Chts8yho.js";
 const q = {
         class: "w-full h-full px-7 py-6 relative overflow-hidden"
     },
     _ = {
         key: 0
     },
     H = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/LogPage-DBzoauOW.css` & `swanlab-0.3.7/swanlab/template/assets/LogPage-DBzoauOW.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/NotFound-DijsQ96i.js` & `swanlab-0.3.7/swanlab/template/assets/NotFound-Dt02Ekhs.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     a as s,
     b as t,
     t as a,
     e as o,
     w as r,
     D as l,
     H as d
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 const i = {
         class: "w-full flex flex-col items-center pt-10"
     },
     m = t("h1", {
         class: "text-5xl font-semibold"
     }, "404", -1),
     n = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/SLLoading-6DfF2aH0.js` & `swanlab-0.3.7/swanlab/template/assets/SLLoading-B-49YNim.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     o as e,
     a as s,
     q as i,
     b as l
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 const t = [l("div", {
         class: "absolute w-full h-full rounded-full border-4 border-t-positive-default border-positive-dimmest"
     }, null, -1), l("div", {
         class: "w-2 h-2 z-10 rounded-full bg-positive-default animate-ping"
     }, null, -1)],
     a = {
         __name: "SLLoading",
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/SLStatusLabel-BRacn5XK.css` & `swanlab-0.3.7/swanlab/template/assets/SLStatusLabel-BRacn5XK.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js` & `swanlab-0.3.7/swanlab/template/assets/SLStatusLabel-DNkFoo89.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,18 +22,18 @@
     C as x,
     W as _,
     F as $,
     N as w,
     K as j,
     r as S,
     X as k
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     _ as C
-} from "./SLLoading-6DfF2aH0.js";
+} from "./SLLoading-B-49YNim.js";
 const L = {
         class: "text-xl font-semibold"
     },
     V = {
         class: "relative pt-4"
     },
     E = {
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf` & `swanlab-0.3.7/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/chart-DB312WPs.css` & `swanlab-0.3.7/swanlab/template/assets/chart-B9MmDiWI.css`

 * *Files 15% similar despite different names*

```diff
@@ -1 +1 @@
-@charset "UTF-8";.lc-tooltip[data-v-218d6cfa]{position:absolute;z-index:10;border-radius:.25rem;border-width:1px;background-color:var(--background-default, #fff);padding:.5rem .75rem;min-width:180px;box-shadow:#15181f29 0 12px 24px;visibility:visible}.lc-tooltip p[data-v-218d6cfa]{font-size:.75rem;line-height:1rem;font-weight:600;color:var(--foreground-default, #000)}.lc-tooltip .lc-tooltip-item-no-zoom[data-v-218d6cfa],.lc-tooltip .lc-tooltip-item-zoom[data-v-218d6cfa]{display:flex;align-items:center;gap:.75rem}.lc-tooltip .lc-tooltip-item-no-zoom[data-v-218d6cfa]:not(:last-child),.lc-tooltip .lc-tooltip-item-zoom[data-v-218d6cfa]:not(:last-child){margin-bottom:.375rem}.lc-tooltip .lc-tooltip-item-no-zoom .lc-tooltip-color[data-v-218d6cfa],.lc-tooltip .lc-tooltip-item-zoom .lc-tooltip-color[data-v-218d6cfa]{display:flex;width:1.25rem;flex-shrink:0;align-items:center}.lc-tooltip .lc-tooltip-item-no-zoom .lc-tooltip-color-rect[data-v-218d6cfa]:before,.lc-tooltip .lc-tooltip-item-zoom .lc-tooltip-color-rect[data-v-218d6cfa]:before{content:"";display:inline-block;width:20px;height:6px;border-radius:2px;margin-right:5px;background-color:currentColor}.lc-tooltip .lc-tooltip-tip[data-v-218d6cfa]{flex-shrink:0;font-size:.75rem;line-height:1rem;font-weight:400;color:var(--foreground-dimmest, #b5b5b5)}.lc-tooltip-item-no-zoom[data-v-218d6cfa]{font-size:.75rem;line-height:1rem}.lc-tooltip-item-no-zoom .lc-tooltip-step[data-v-218d6cfa]{flex-shrink:0;font-weight:600}.lc-tooltip-item-no-zoom .lc-tooltip-step[data-v-218d6cfa]:after{content:":";font-weight:600}.lc-tooltip-item-no-zoom .lc-tooltip-value[data-v-218d6cfa]{text-align:left;font-weight:600}.lc-tooltip-item-no-zoom .lc-tooltip-tag[data-v-218d6cfa]{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.lc-tooltip-item-zoom .lc-tooltip-step[data-v-218d6cfa]{width:1.75rem}.lc-tooltip-item-zoom .lc-tooltip-value[data-v-218d6cfa]{text-align:left}.lc-tooltip-item-zoom .lc-tooltip-time[data-v-218d6cfa]{width:8rem}.lc-tooltip-item-zoom .lc-tooltip-tag[data-v-218d6cfa]{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.lc-legend[data-v-28a14269]{max-height:28px;min-height:16px;margin-bottom:.25rem;display:flex;flex-wrap:wrap;row-gap:.125rem;-moz-column-gap:.5rem;column-gap:.5rem;overflow-y:auto;padding-left:.75rem;padding-right:.75rem;font-size:12px;line-height:1;justify-content:center}.lc-legend .lc-legend-item[data-v-28a14269]{display:flex;flex-shrink:0;align-items:center}.lc-legend .lc-legend-item[data-v-28a14269]:hover{--tw-brightness: brightness(.75);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.lc-legend .lc-legend-item[data-v-28a14269]:before{content:"";display:inline-block;width:8px;height:2px;margin-top:2px;margin-right:4px;background-color:currentColor}.sliding-range[data-v-c91de514]{margin-left:.125rem;margin-right:.125rem;flex-grow:1;padding-top:.75rem;padding-bottom:.75rem}.sliding-range[data-v-c91de514]:hover{cursor:grab}.sliding-range[data-v-c91de514]:active{cursor:grabbing}.sliding-range .sliding-bar[data-v-c91de514]{height:100%;border-top-left-radius:9999px;border-bottom-left-radius:9999px}.sliding-range .sliding-container[data-v-c91de514]{height:100%;flex-grow:1;border-top-right-radius:9999px;border-bottom-right-radius:9999px;background-color:var(--outline-default)}.sliding-range .sliding-button[data-v-c91de514]{position:absolute;top:0;height:.75rem;width:.75rem;--tw-translate-y: -30%;--tw-translate-x: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;border-width:2px;border-color:var(--outline-dimmer, #e5e8eb);background-color:var(--background-default, #fff)}.sliding-range:active .sliding-button[data-v-c91de514]{border-color:var(--outline-dimmer, #e5e8eb)}input[type=number][data-v-c91de514]::-webkit-inner-spin-button,input[type=number][data-v-c91de514]::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}input[type=number][data-v-c91de514]{-moz-appearance:textfield;-webkit-appearance:textfield;appearance:textfield}input[data-v-c91de514]{height:1.5rem;width:4rem;border-radius:.25rem;border-width:1px;background-color:transparent;padding-left:.25rem;padding-right:1.25rem;font-size:.75rem;line-height:1rem;outline:2px solid transparent;outline-offset:2px}input[data-v-c91de514]:focus{border-color:var(--primary-default, #0f87ff)}.input-disabled[data-v-c91de514]{opacity:.5}.chart-slide[data-v-ce0f47f9]{display:flex;width:100%;-webkit-user-select:none;-moz-user-select:none;user-select:none;flex-wrap:nowrap;align-items:center;justify-content:center;gap:.5rem;color:var(--foreground-dimmer, #555)}.chart-slide .slide[data-v-ce0f47f9]{width:100%;max-width:230px}.chart-slide input[type=number][data-v-ce0f47f9]::-webkit-inner-spin-button,.chart-slide input[type=number][data-v-ce0f47f9]::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.chart-slide input[type=number][data-v-ce0f47f9]{-moz-appearance:textfield;-webkit-appearance:textfield;appearance:textfield}input[data-v-ce0f47f9]{height:1.5rem;width:4rem;border-radius:.25rem;border-width:1px;background-color:transparent;padding-left:.25rem;padding-right:1.25rem;font-size:.75rem;line-height:1rem;outline:2px solid transparent;outline-offset:2px}input[data-v-ce0f47f9]:focus{border-color:var(--primary-default, #0f87ff)}.audios-container[data-v-94852f19]{display:grid;width:100%;gap:1rem}.audios-container .audio-container[data-v-94852f19]{position:relative;display:flex;height:12rem;width:100%;flex-direction:column;color:var(--foreground-dimmer, #555)}.text-detail[data-v-9e9efe9d]{overflow:hidden;border-radius:.5rem;background-color:var(--background-higher, #f6f8fA);padding:2.5rem 1.5rem}.caption[data-v-363003df]{height:2.5rem;width:6rem;flex-shrink:0;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-right-width:1px;padding-left:1rem;padding-right:1rem;padding-top:.5rem}@media (min-width: 768px){.caption[data-v-363003df]{width:10rem}}.text[data-v-363003df]{width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;padding:.5rem 1rem}.line[data-v-363003df]{position:relative;display:flex;align-items:center;border-bottom-width:1px;border-color:var(--outline-dimmest, #f2f2f2)}.line[data-v-363003df]:hover{background-color:var(--background-higher, #f6f8fA)}.line:hover .icon[data-v-363003df]{display:block;border-radius:.125rem;border-width:1px;border-color:var(--outline-dimmest, #f2f2f2)}.line:hover .icon[data-v-363003df]:hover{border-radius:.25rem;background-color:var(--background-highest, #dadde1)}@keyframes skeleton-ani-363003df{0%{left:0}to{left:100%}}.skeleton[data-v-363003df]{display:block;background-image:linear-gradient(-45deg,#f5f5f5 40%,#fff 55%,#f5f5f5 63%);list-style:none;background-size:400% 100%;background-position:100% 50%;animation:skeleton-animation-363003df 2s ease infinite}@keyframes skeleton-animation-363003df{0%{background-position:100% 50%}to{background-position:0 50%}}.text-table[data-v-32dda51e]{margin-left:-.75rem;margin-right:-.75rem;width:calc(100% + 1.5rem);padding-top:.5rem}.pannel-button[data-v-409b3539]{height:1rem;width:1rem;height:100%;border-radius:.25rem;padding:.125rem;color:var(--foreground-dimmer, #555)}.pannel-button[data-v-409b3539]:hover{background-color:var(--positive-dimmest, #97e896);color:var(--positive-highest, #004d0d)}.pannel-button[data-v-409b3539]:disabled{cursor:progress;opacity:.6}.image-detail[data-v-b4d62674]{position:relative;height:100%;width:100%;max-height:13rem}.image-detail .image-container[data-v-b4d62674]{position:relative;display:inline-flex;width:100%;flex-grow:1;cursor:pointer;justify-content:center;height:calc(100% - 2.5rem)}.image-detail .image-container img[data-v-b4d62674]{margin-top:auto;margin-bottom:auto;-o-object-fit:contain;object-fit:contain;height:100%}.image-detail .image-container:hover .image-download-button[data-v-b4d62674]{display:block}.image-content[data-v-65e42ccf]{position:relative;margin-top:.25rem;min-height:224px;width:100%;border-radius:.125rem;padding:.5rem}.image-content .images-container[data-v-65e42ccf]{display:grid;height:100%;gap:.75rem}.image-content-no-zoom[data-v-65e42ccf]{height:14rem;overflow-y:auto;overflow-x:clip}.image-content-zoom[data-v-65e42ccf]{height:calc(100vh - 19rem);overflow-y:auto;overflow-x:clip}.image-single-zoom[data-v-65e42ccf]{display:flex;width:100%;align-items:center;justify-content:space-between}.image-single-zoom:hover .image-download-button[data-v-65e42ccf]{display:block}.image-single-zoom .icon[data-v-65e42ccf]{height:2.5rem;width:2.5rem;cursor:pointer;border-radius:9999px;border-width:1px;opacity:.2;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.image-single-zoom .icon[data-v-65e42ccf]:hover{opacity:1}.image-download-button{position:absolute;top:.25rem;right:.25rem;display:none;opacity:.75;width:1.25rem!important;height:1.25rem!important;padding:.125rem!important}.sa-popover-button-active[data-sa-menu][data-v-c797d293]{border-color:var(--primary-default)!important}.sa-menu-corner[data-sa-menu][data-v-c797d293]{z-index:9998;--tw-rotate: -45deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-top-width:1px;border-right-width:1px;background-color:var(--background-default, #fff);position:absolute;display:block;width:12px;height:12px;pointer-events:none;content:" ";clip-path:polygon(20% 0,100% 0,100% 80%,80% 100%,0 20%)}.sa-menu-pop[data-sa-menu][data-v-c797d293]{margin-top:.25rem;margin-bottom:.25rem;width:100%;border-radius:.25rem;border-width:1px;font-size:.875rem;line-height:1.25rem;box-shadow:0 4px 10px #0000001a}.sa-menu-items[data-v-eaa2bdc8]{width:100%}.sa-menu-items[data-v-eaa2bdc8]:not(:last-child){border-bottom-width:1px;padding-bottom:.5rem}input[data-v-ef7bea54]{border-radius:.25rem;border-width:1px;padding:.25rem .5rem}.param[data-v-6fce60bd]{display:flex;align-items:center;color:var(--foreground-dimmer, #555)}.param span[data-v-6fce60bd]{display:block;width:5rem}@media (min-width: 768px){.param span[data-v-6fce60bd]{width:auto}}.chart-container[data-v-7e8dfb95]{position:relative;height:auto;min-height:288px;width:100%;border-radius:.25rem;border-width:1px;background-color:var(--background-default, #fff);padding:1rem .75rem;display:flex;flex-direction:column;justify-content:space-between}.chart-panel[data-v-7e8dfb95]{position:absolute;top:.25rem;right:.5rem;height:1rem;display:flex;align-items:center;justify-content:flex-end;gap:.5rem}.line-chart[data-v-7e8dfb95]{grid-column:span 3 / span 3}@media (min-width: 1024px){.line-chart[data-v-7e8dfb95]{grid-column:span 1 / span 1}}.audio-chart[data-v-7e8dfb95],.image-chart[data-v-7e8dfb95],.text-chart[data-v-7e8dfb95]{grid-column:span 3 / span 3}.charts-container[data-v-c31782ca]{padding:1.5rem 2rem}.charts-container[data-v-c31782ca]:not(:last-child){border-bottom-width:1px}.charts-container .charts-slot[data-v-c31782ca]{margin-top:18px;display:grid;grid-template-columns:repeat(1,minmax(0,1fr));gap:1.5rem}@media (min-width: 1024px){.charts-container .charts-slot[data-v-c31782ca]{grid-template-columns:repeat(2,minmax(0,1fr))}}@media (min-width: 1280px){.charts-container .charts-slot[data-v-c31782ca]{grid-template-columns:repeat(3,minmax(0,1fr))}}.smooth-button[data-v-8c22f071]{height:2rem;width:2rem;border-radius:.25rem;padding:.25rem;color:var(--foreground-dimmer, #555)}.smooth-button[data-v-8c22f071]:hover{background-color:var(--positive-dimmer, #3cc954);color:var(--positive-default, #00a11b)}.method-items .method-item[data-v-8c22f071]:hover{background-color:var(--background-higher, #f6f8fA)}.charts-pannel[data-v-d017e294]{position:sticky;top:0;display:flex;justify-content:space-between;border-bottom-width:1px;background-color:var(--background-higher, #f6f8fA);padding:.75rem 1rem;z-index:30}
+@charset "UTF-8";.lc-tooltip[data-v-aa1bab0c]{position:absolute;z-index:10;border-radius:.25rem;border-width:1px;background-color:var(--background-default, #fff);padding:.5rem .75rem;min-width:180px;box-shadow:#15181f29 0 12px 24px;visibility:visible}.lc-tooltip p[data-v-aa1bab0c]{font-size:.75rem;line-height:1rem;font-weight:600;color:var(--foreground-default, #000)}.lc-tooltip .lc-tooltip-item-no-zoom[data-v-aa1bab0c],.lc-tooltip .lc-tooltip-item-zoom[data-v-aa1bab0c]{display:flex;align-items:center;gap:.75rem}.lc-tooltip .lc-tooltip-item-no-zoom[data-v-aa1bab0c]:not(:last-child),.lc-tooltip .lc-tooltip-item-zoom[data-v-aa1bab0c]:not(:last-child){margin-bottom:.375rem}.lc-tooltip .lc-tooltip-item-no-zoom .lc-tooltip-color[data-v-aa1bab0c],.lc-tooltip .lc-tooltip-item-zoom .lc-tooltip-color[data-v-aa1bab0c]{display:flex;width:1.25rem;flex-shrink:0;align-items:center}.lc-tooltip .lc-tooltip-item-no-zoom .lc-tooltip-color-rect[data-v-aa1bab0c]:before,.lc-tooltip .lc-tooltip-item-zoom .lc-tooltip-color-rect[data-v-aa1bab0c]:before{content:"";display:inline-block;width:20px;height:6px;border-radius:2px;margin-right:5px;background-color:currentColor}.lc-tooltip .lc-tooltip-tip[data-v-aa1bab0c]{flex-shrink:0;font-size:.75rem;line-height:1rem;font-weight:400;color:var(--foreground-dimmest, #b5b5b5)}.lc-tooltip-item-no-zoom[data-v-aa1bab0c]{font-size:.75rem;line-height:1rem}.lc-tooltip-item-no-zoom .lc-tooltip-step[data-v-aa1bab0c]{flex-shrink:0;font-weight:600}.lc-tooltip-item-no-zoom .lc-tooltip-step[data-v-aa1bab0c]:after{content:":";font-weight:600}.lc-tooltip-item-no-zoom .lc-tooltip-value[data-v-aa1bab0c]{white-space:nowrap;text-align:left;font-weight:600}.lc-tooltip-item-no-zoom .lc-tooltip-tag[data-v-aa1bab0c]{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.lc-tooltip-item-zoom .lc-tooltip-step[data-v-aa1bab0c]{width:1.75rem}.lc-tooltip-item-zoom .lc-tooltip-value[data-v-aa1bab0c]{text-align:left}.lc-tooltip-item-zoom .lc-tooltip-time[data-v-aa1bab0c]{width:8rem}.lc-tooltip-item-zoom .lc-tooltip-tag[data-v-aa1bab0c]{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.lc-legend[data-v-28a14269]{max-height:28px;min-height:16px;margin-bottom:.25rem;display:flex;flex-wrap:wrap;row-gap:.125rem;-moz-column-gap:.5rem;column-gap:.5rem;overflow-y:auto;padding-left:.75rem;padding-right:.75rem;font-size:12px;line-height:1;justify-content:center}.lc-legend .lc-legend-item[data-v-28a14269]{display:flex;flex-shrink:0;align-items:center}.lc-legend .lc-legend-item[data-v-28a14269]:hover{--tw-brightness: brightness(.75);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.lc-legend .lc-legend-item[data-v-28a14269]:before{content:"";display:inline-block;width:8px;height:2px;margin-top:2px;margin-right:4px;background-color:currentColor}.sliding-range[data-v-c91de514]{margin-left:.125rem;margin-right:.125rem;flex-grow:1;padding-top:.75rem;padding-bottom:.75rem}.sliding-range[data-v-c91de514]:hover{cursor:grab}.sliding-range[data-v-c91de514]:active{cursor:grabbing}.sliding-range .sliding-bar[data-v-c91de514]{height:100%;border-top-left-radius:9999px;border-bottom-left-radius:9999px}.sliding-range .sliding-container[data-v-c91de514]{height:100%;flex-grow:1;border-top-right-radius:9999px;border-bottom-right-radius:9999px;background-color:var(--outline-default)}.sliding-range .sliding-button[data-v-c91de514]{position:absolute;top:0;height:.75rem;width:.75rem;--tw-translate-y: -30%;--tw-translate-x: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;border-width:2px;border-color:var(--outline-dimmer, #e5e8eb);background-color:var(--background-default, #fff)}.sliding-range:active .sliding-button[data-v-c91de514]{border-color:var(--outline-dimmer, #e5e8eb)}input[type=number][data-v-c91de514]::-webkit-inner-spin-button,input[type=number][data-v-c91de514]::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}input[type=number][data-v-c91de514]{-moz-appearance:textfield;-webkit-appearance:textfield;appearance:textfield}input[data-v-c91de514]{height:1.5rem;width:4rem;border-radius:.25rem;border-width:1px;background-color:transparent;padding-left:.25rem;padding-right:1.25rem;font-size:.75rem;line-height:1rem;outline:2px solid transparent;outline-offset:2px}input[data-v-c91de514]:focus{border-color:var(--primary-default, #0f87ff)}.input-disabled[data-v-c91de514]{opacity:.5}.chart-slide[data-v-ce0f47f9]{display:flex;width:100%;-webkit-user-select:none;-moz-user-select:none;user-select:none;flex-wrap:nowrap;align-items:center;justify-content:center;gap:.5rem;color:var(--foreground-dimmer, #555)}.chart-slide .slide[data-v-ce0f47f9]{width:100%;max-width:230px}.chart-slide input[type=number][data-v-ce0f47f9]::-webkit-inner-spin-button,.chart-slide input[type=number][data-v-ce0f47f9]::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.chart-slide input[type=number][data-v-ce0f47f9]{-moz-appearance:textfield;-webkit-appearance:textfield;appearance:textfield}input[data-v-ce0f47f9]{height:1.5rem;width:4rem;border-radius:.25rem;border-width:1px;background-color:transparent;padding-left:.25rem;padding-right:1.25rem;font-size:.75rem;line-height:1rem;outline:2px solid transparent;outline-offset:2px}input[data-v-ce0f47f9]:focus{border-color:var(--primary-default, #0f87ff)}.audios-container[data-v-94852f19]{display:grid;width:100%;gap:1rem}.audios-container .audio-container[data-v-94852f19]{position:relative;display:flex;height:12rem;width:100%;flex-direction:column;color:var(--foreground-dimmer, #555)}.text-detail[data-v-9e9efe9d]{overflow:hidden;border-radius:.5rem;background-color:var(--background-higher, #f6f8fA);padding:2.5rem 1.5rem}.caption[data-v-363003df]{height:2.5rem;width:6rem;flex-shrink:0;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-right-width:1px;padding-left:1rem;padding-right:1rem;padding-top:.5rem}@media (min-width: 768px){.caption[data-v-363003df]{width:10rem}}.text[data-v-363003df]{width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;padding:.5rem 1rem}.line[data-v-363003df]{position:relative;display:flex;align-items:center;border-bottom-width:1px;border-color:var(--outline-dimmest, #f2f2f2)}.line[data-v-363003df]:hover{background-color:var(--background-higher, #f6f8fA)}.line:hover .icon[data-v-363003df]{display:block;border-radius:.125rem;border-width:1px;border-color:var(--outline-dimmest, #f2f2f2)}.line:hover .icon[data-v-363003df]:hover{border-radius:.25rem;background-color:var(--background-highest, #dadde1)}@keyframes skeleton-ani-363003df{0%{left:0}to{left:100%}}.skeleton[data-v-363003df]{display:block;background-image:linear-gradient(-45deg,#f5f5f5 40%,#fff 55%,#f5f5f5 63%);list-style:none;background-size:400% 100%;background-position:100% 50%;animation:skeleton-animation-363003df 2s ease infinite}@keyframes skeleton-animation-363003df{0%{background-position:100% 50%}to{background-position:0 50%}}.text-table[data-v-32dda51e]{margin-left:-.75rem;margin-right:-.75rem;width:calc(100% + 1.5rem);padding-top:.5rem}.pannel-button[data-v-409b3539]{height:1rem;width:1rem;height:100%;border-radius:.25rem;padding:.125rem;color:var(--foreground-dimmer, #555)}.pannel-button[data-v-409b3539]:hover{background-color:var(--positive-dimmest, #97e896);color:var(--positive-highest, #004d0d)}.pannel-button[data-v-409b3539]:disabled{cursor:progress;opacity:.6}.image-detail[data-v-b4d62674]{position:relative;height:100%;width:100%;max-height:13rem}.image-detail .image-container[data-v-b4d62674]{position:relative;display:inline-flex;width:100%;flex-grow:1;cursor:pointer;justify-content:center;height:calc(100% - 2.5rem)}.image-detail .image-container img[data-v-b4d62674]{margin-top:auto;margin-bottom:auto;-o-object-fit:contain;object-fit:contain;height:100%}.image-detail .image-container:hover .image-download-button[data-v-b4d62674]{display:block}.image-content[data-v-65e42ccf]{position:relative;margin-top:.25rem;min-height:224px;width:100%;border-radius:.125rem;padding:.5rem}.image-content .images-container[data-v-65e42ccf]{display:grid;height:100%;gap:.75rem}.image-content-no-zoom[data-v-65e42ccf]{height:14rem;overflow-y:auto;overflow-x:clip}.image-content-zoom[data-v-65e42ccf]{height:calc(100vh - 19rem);overflow-y:auto;overflow-x:clip}.image-single-zoom[data-v-65e42ccf]{display:flex;width:100%;align-items:center;justify-content:space-between}.image-single-zoom:hover .image-download-button[data-v-65e42ccf]{display:block}.image-single-zoom .icon[data-v-65e42ccf]{height:2.5rem;width:2.5rem;cursor:pointer;border-radius:9999px;border-width:1px;opacity:.2;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.image-single-zoom .icon[data-v-65e42ccf]:hover{opacity:1}.image-download-button{position:absolute;top:.25rem;right:.25rem;display:none;opacity:.75;width:1.25rem!important;height:1.25rem!important;padding:.125rem!important}.sa-popover-button-active[data-sa-menu][data-v-c797d293]{border-color:var(--primary-default)!important}.sa-menu-corner[data-sa-menu][data-v-c797d293]{z-index:9998;--tw-rotate: -45deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-top-width:1px;border-right-width:1px;background-color:var(--background-default, #fff);position:absolute;display:block;width:12px;height:12px;pointer-events:none;content:" ";clip-path:polygon(20% 0,100% 0,100% 80%,80% 100%,0 20%)}.sa-menu-pop[data-sa-menu][data-v-c797d293]{margin-top:.25rem;margin-bottom:.25rem;width:100%;border-radius:.25rem;border-width:1px;font-size:.875rem;line-height:1.25rem;box-shadow:0 4px 10px #0000001a}.sa-menu-items[data-v-eaa2bdc8]{width:100%}.sa-menu-items[data-v-eaa2bdc8]:not(:last-child){border-bottom-width:1px;padding-bottom:.5rem}input[data-v-ef7bea54]{border-radius:.25rem;border-width:1px;padding:.25rem .5rem}.param[data-v-6fce60bd]{display:flex;align-items:center;color:var(--foreground-dimmer, #555)}.param span[data-v-6fce60bd]{display:block;width:5rem}@media (min-width: 768px){.param span[data-v-6fce60bd]{width:auto}}.chart-container[data-v-c3301138]{position:relative;height:auto;min-height:288px;width:100%;border-radius:.25rem;border-width:1px;background-color:var(--background-default, #fff);padding:1rem .75rem;display:flex;flex-direction:column;justify-content:space-between}.chart-panel[data-v-c3301138]{position:absolute;top:.25rem;right:.5rem;height:1rem;display:flex;align-items:center;justify-content:flex-end;gap:.5rem}.line-chart[data-v-c3301138]{grid-column:span 3 / span 3}@media (min-width: 1024px){.line-chart[data-v-c3301138]{grid-column:span 1 / span 1}}.audio-chart[data-v-c3301138],.image-chart[data-v-c3301138],.text-chart[data-v-c3301138]{grid-column:span 3 / span 3}.charts-container[data-v-c31782ca]{padding:1.5rem 2rem}.charts-container[data-v-c31782ca]:not(:last-child){border-bottom-width:1px}.charts-container .charts-slot[data-v-c31782ca]{margin-top:18px;display:grid;grid-template-columns:repeat(1,minmax(0,1fr));gap:1.5rem}@media (min-width: 1024px){.charts-container .charts-slot[data-v-c31782ca]{grid-template-columns:repeat(2,minmax(0,1fr))}}@media (min-width: 1280px){.charts-container .charts-slot[data-v-c31782ca]{grid-template-columns:repeat(3,minmax(0,1fr))}}.smooth-button[data-v-8c22f071]{height:2rem;width:2rem;border-radius:.25rem;padding:.25rem;color:var(--foreground-dimmer, #555)}.smooth-button[data-v-8c22f071]:hover{background-color:var(--positive-dimmer, #3cc954);color:var(--positive-default, #00a11b)}.method-items .method-item[data-v-8c22f071]:hover{background-color:var(--background-higher, #f6f8fA)}.charts-pannel[data-v-3dc9e87b]{position:sticky;top:0;display:flex;justify-content:space-between;border-bottom-width:1px;background-color:var(--background-higher, #f6f8fA);padding:.75rem 1rem;z-index:30}
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/chart-eW1meEc1.js` & `swanlab-0.3.7/swanlab/template/assets/chart-Cb2YjpB3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -65,18 +65,18 @@
     r as lt,
     ar as ut,
     U as ct,
     X as ht,
     S as pt,
     as as ft,
     h as dt
-} from "./index-B5SDzoY4.js";
+} from "./index-CmcaZNbV.js";
 import {
     _ as gt
-} from "./SLLoading-6DfF2aH0.js";
+} from "./SLLoading-B-49YNim.js";
 const yt = Object.freeze(Object.defineProperty({
         __proto__: null,
         get Base() {
             return Qg
         },
         get Circle() {
             return Ug
@@ -43408,15 +43408,15 @@
             }))
         }]
     ]);
 
 function JH(t, e) {
     return jH.get(e.id)(t, e.value)
 }
-const qH = t => (K("data-v-218d6cfa"), t = t(), V(), t),
+const qH = t => (K("data-v-aa1bab0c"), t = t(), V(), t),
     ZH = qH((() => D("span", {
         class: "lc-tooltip-color lc-tooltip-color-rect"
     }, null, -1))),
     $H = {
         class: "lc-tooltip-step"
     },
     tT = {
@@ -43495,15 +43495,15 @@
                 })
             }, [AT, D("span", rT, P(t.data.index), 1), D("span", iT, P(O(u)(t.data.data)), 1), D("span", oT, P(t.data.series), 1)], 4)))), 128)) : R("", !0), D("p", aT, P(O(r)), 1)])), [
                 [S, s.value]
             ])
         }
     },
     lT = Q(sT, [
-        ["__scopeId", "data-v-218d6cfa"]
+        ["__scopeId", "data-v-aa1bab0c"]
     ]),
     uT = {
         class: "lc-legend"
     },
     cT = ["onMouseenter", "onMouseleave", "onClick"],
     hT = Q({
         __name: "LineChartLegend",
@@ -43628,14 +43628,15 @@
                 b = t(),
                 Q = r.chart.reference,
                 {
                     xField: E,
                     xTitle: S
                 } = WH[Q],
                 H = (t, e, n = {}, A = !1) => {
+                    if (!t) return;
                     const o = new Ub(t, {
                         data: e,
                         xField: E,
                         yField: "data",
                         colorField: "type",
                         legend: !1,
                         color: ({
@@ -43744,15 +43745,15 @@
                         }
                         void 0 !== n && st(o, A, rt[n].data.series, rt[n].color)
                     })), o
                 },
                 T = t => {
                     if (h) {
                         const e = {};
-                        for (const n in t) t[n] && (e[n] = {
+                        for (const n in t) t[n] && (t[n].list.some((t => "string" == typeof t.data)) ? e[n] = t[n] : e[n] = {
                             ...t[n],
                             list: JH(t[n].list, h)
                         });
                         for (const n in t) e[`${n}&smooth`] = t[n];
                         t = e
                     }
                     if (i.length < 1) throw new Error("source length must be greater than 1");
@@ -50675,27 +50676,32 @@
                 V = a((() => {
                     var t, e;
                     return !F.value && ("default" === (null == (t = i.chart) ? void 0 : t.type) || "line" === (null == (e = i.chart) ? void 0 : e.type))
                 }));
             return A({
                 chartRef: b,
                 smooth: t => {
-                    E.value = t, b.value.smooth && b.value.smooth(t)
+                    var e;
+                    E.value = t, (null == (e = b.value) ? void 0 : e.smooth) && b.value.smooth(t)
                 },
                 thicken: (...t) => {
-                    b.value.thicken && b.value.thicken(...t)
+                    var e;
+                    (null == (e = b.value) ? void 0 : e.thicken) && b.value.thicken(...t)
                 },
                 thin: (...t) => {
-                    b.value.thin && b.value.thin(...t)
+                    var e;
+                    (null == (e = b.value) ? void 0 : e.thin) && b.value.thin(...t)
                 },
                 showTooltip: (...t) => {
-                    b.value.showTooltip && b.value.showTooltip(...t)
+                    var e;
+                    (null == (e = b.value) ? void 0 : e.showTooltip) && b.value.showTooltip(...t)
                 },
                 hideTooltip: () => {
-                    b.value.hideTooltip && b.value.hideTooltip()
+                    var t;
+                    (null == (t = b.value) ? void 0 : t.hideTooltip) && b.value.hideTooltip()
                 }
             }), (t, e) => (I(), k("section", {
                 class: et(["chart-container", B.value.class]),
                 onMouseenter: h,
                 onMouseleave: p
             }, ["error" === d.value ? (I(), k("div", nX, [N(z, {
                 class: "mx-auto h-5 w-5",
@@ -50769,15 +50775,15 @@
                 ref: b,
                 title: n.chart.name,
                 chart: n.chart
             }, null, 8, ["index", "title", "chart"]))], 64)), g.value ? (I(), k("div", iX, [N(gt)])) : R("", !0)], 34))
         }
     },
     aX = Q(oX, [
-        ["__scopeId", "data-v-7e8dfb95"]
+        ["__scopeId", "data-v-c3301138"]
     ]),
     sX = {
         class: "charts-container",
         ref: "chartsContainerRef"
     },
     lX = {
         class: "flex items-center"
@@ -51060,15 +51066,15 @@
                 i = t([]),
                 o = a((() => r.value ? r.value : A.value)),
                 s = t => t.charts,
                 l = t(null),
                 c = t => {
                     i.value.forEach((e => {
                         e.chartRefList.forEach((e => {
-                            e.smooth(t)
+                            null == e || e.smooth(t)
                         }))
                     })), l.value = t
                 };
             u("smoothMethod", l);
             const h = ft(((t, e) => {
                     n.updateNamespaceStatus(t, e)
                 }), 300),
@@ -51122,15 +51128,15 @@
                     onUnhide: y
                 }, null, 8, ["label", "charts", "index", "opened", "isPinned", "isHidden", "onSwitch"]);
                 var n
             })), 128))], 64))
         }
     },
     UX = Q(QX, [
-        ["__scopeId", "data-v-d017e294"]
+        ["__scopeId", "data-v-3dc9e87b"]
     ]),
     MX = {
         get: (t, e, n) => new Promise(((A, r) => {
             dt.get("/media/" + t, {
                 params: {
                     tag: n,
                     experiment_id: e
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/index-B5SDzoY4.js` & `swanlab-0.3.7/swanlab/template/assets/index-CmcaZNbV.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-const __vite__fileDeps = ["assets/HomeView-BqTu9_fG.js", "assets/SLStatusLabel-DvEKZN8v.js", "assets/SLLoading-6DfF2aH0.js", "assets/SLStatusLabel-BRacn5XK.css", "assets/HomeView-BS7FyMAt.css", "assets/ChartsView-DpI6U3QH.js", "assets/chart-eW1meEc1.js", "assets/chart-DB312WPs.css", "assets/ExperimentView-BTbu21ka.js", "assets/ExperimentView-CCDMXo4h.css", "assets/IndexPage-CrqN4Ekl.js", "assets/IndexPage-C5dvtib2.css", "assets/ChartPage-C2Rj7xI3.js", "assets/ChartPage-DgOOkrVh.css", "assets/LogPage-B-fC6sB7.js", "assets/FuncBar-Ct_nBdvU.js", "assets/FuncBar-DgVTuZfd.css", "assets/LogPage-DBzoauOW.css", "assets/EnvironmentPage-Bb8ousXq.js", "assets/EnvironmentPage-C6uSuWBq.css", "assets/EnvIndex-B5_l1b65.js", "assets/EnvItems-B4PwmQT4.js", "assets/EnvItems-BfjcRO-X.css", "assets/EnvHardware-4H7mp2Bs.js", "assets/EnvRequirements-Cpn2Fk1D.js", "assets/EnvRequirements-BqyzUHLZ.css"],
+const __vite__fileDeps = ["assets/HomeView-uDUGPxwP.js", "assets/SLStatusLabel-DNkFoo89.js", "assets/SLLoading-B-49YNim.js", "assets/SLStatusLabel-BRacn5XK.css", "assets/HomeView-BS7FyMAt.css", "assets/ChartsView-DKnkZV4x.js", "assets/chart-Cb2YjpB3.js", "assets/chart-B9MmDiWI.css", "assets/ExperimentView-x-2IwSHi.js", "assets/ExperimentView-CCDMXo4h.css", "assets/IndexPage-Jy4F58Oh.js", "assets/IndexPage-C5dvtib2.css", "assets/ChartPage-BqfnvJQ4.js", "assets/ChartPage-DgOOkrVh.css", "assets/LogPage-D3SdB10-.js", "assets/FuncBar-Chts8yho.js", "assets/FuncBar-DgVTuZfd.css", "assets/LogPage-DBzoauOW.css", "assets/EnvironmentPage-DLnE8Co5.js", "assets/EnvironmentPage-C6uSuWBq.css", "assets/EnvIndex-3qdPSvC8.js", "assets/EnvItems-z9WBoR8b.js", "assets/EnvItems-BfjcRO-X.css", "assets/EnvHardware-Dh6G7EyN.js", "assets/EnvRequirements-B26RqDqU.js", "assets/EnvRequirements-BqyzUHLZ.css"],
     __vite__mapDeps = i => i.map(i => __vite__fileDeps[i]);
 /**
  * @vue/shared v3.4.27
  * (c) 2018-present Yuxi (Evan) You and Vue contributors
  * @license MIT
  **/
 /*! #__NO_SIDE_EFFECTS__ */
@@ -9521,14 +9521,15 @@
     return function(r, ...o) {
         n[r] && clearTimeout(n[r]), n[r] = setTimeout((() => {
             null == e || e.apply(this, [r, ...o])
         }), t)
     }
 }
 const ih = (e, t = 1e5, n = 1e-4, r = 4) => {
+        if ("NaN" === e || "INF" === e) return e;
         const o = r + 6,
             a = (e = Number(e)) >= 0 ? "" : "-";
         if ((e = Math.abs(e)) >= n && e < t || 0 === e) {
             if (e.toString().includes("e")) {
                 const t = n.toString(),
                     o = Number(t.substring(t.indexOf("-") + 1));
                 e = e.toFixed(o + r - 1)
@@ -14304,67 +14305,67 @@
             });
             if (t.payload = e, window.dispatchEvent(t), !t.defaultPrevented) throw e
         }))
     },
     Rb = [{
         path: "/",
         name: "overview",
-        component: () => Pb((() => import("./HomeView-BqTu9_fG.js")), __vite__mapDeps([0, 1, 2, 3, 4]))
+        component: () => Pb((() => import("./HomeView-uDUGPxwP.js")), __vite__mapDeps([0, 1, 2, 3, 4]))
     }, {
         path: "/charts",
         name: "charts",
-        component: () => Pb((() => import("./ChartsView-DpI6U3QH.js")), __vite__mapDeps([5, 6, 2, 7]))
+        component: () => Pb((() => import("./ChartsView-DKnkZV4x.js")), __vite__mapDeps([5, 6, 2, 7]))
     }, {
         path: "/experiment/:experimentId",
         name: "experiment",
-        component: () => Pb((() => import("./ExperimentView-BTbu21ka.js")), __vite__mapDeps([8, 1, 2, 3, 9])),
+        component: () => Pb((() => import("./ExperimentView-x-2IwSHi.js")), __vite__mapDeps([8, 1, 2, 3, 9])),
         redirect: {
             name: "experiment_chart"
         },
         children: [{
             path: "index",
             name: "experiment_index",
-            component: () => Pb((() => import("./IndexPage-CrqN4Ekl.js")), __vite__mapDeps([10, 11]))
+            component: () => Pb((() => import("./IndexPage-Jy4F58Oh.js")), __vite__mapDeps([10, 11]))
         }, {
             path: "chart",
             name: "experiment_chart",
-            component: () => Pb((() => import("./ChartPage-C2Rj7xI3.js")), __vite__mapDeps([12, 6, 2, 7, 13]))
+            component: () => Pb((() => import("./ChartPage-BqfnvJQ4.js")), __vite__mapDeps([12, 6, 2, 7, 13]))
         }, {
             path: "log",
             name: "experiment_log",
-            component: () => Pb((() => import("./LogPage-B-fC6sB7.js")), __vite__mapDeps([14, 2, 15, 16, 17]))
+            component: () => Pb((() => import("./LogPage-D3SdB10-.js")), __vite__mapDeps([14, 2, 15, 16, 17]))
         }, {
             path: "env",
             name: "experiment_env",
-            component: () => Pb((() => import("./EnvironmentPage-Bb8ousXq.js")), __vite__mapDeps([18, 19])),
+            component: () => Pb((() => import("./EnvironmentPage-DLnE8Co5.js")), __vite__mapDeps([18, 19])),
             redirect: {
                 name: "exp_env_index"
             },
             children: [{
                 path: "index",
                 name: "exp_env_index",
-                component: () => Pb((() => import("./EnvIndex-B5_l1b65.js")), __vite__mapDeps([20, 21, 22]))
+                component: () => Pb((() => import("./EnvIndex-3qdPSvC8.js")), __vite__mapDeps([20, 21, 22]))
             }, {
                 path: "hardware",
                 name: "exp_env_hardware",
-                component: () => Pb((() => import("./EnvHardware-4H7mp2Bs.js")), __vite__mapDeps([23, 21, 22]))
+                component: () => Pb((() => import("./EnvHardware-Dh6G7EyN.js")), __vite__mapDeps([23, 21, 22]))
             }, {
                 path: "requirements",
                 name: "exp_env_dependencies",
-                component: () => Pb((() => import("./EnvRequirements-Cpn2Fk1D.js")), __vite__mapDeps([24, 15, 16, 25]))
+                component: () => Pb((() => import("./EnvRequirements-B26RqDqU.js")), __vite__mapDeps([24, 15, 16, 25]))
             }]
         }]
     }, {
         path: "/help",
         name: "help",
-        component: () => Pb((() => import("./HelpView-C4wSXY1I.js")), [])
+        component: () => Pb((() => import("./HelpView-BS1FZ4Nz.js")), [])
     }, {
         path: "/404",
         name: "not-found",
-        component: () => Pb((() => import("./NotFound-DijsQ96i.js")), [])
+        component: () => Pb((() => import("./NotFound-Dt02Ekhs.js")), [])
     }, {
         path: "/:pathMatch(.*)*",
         redirect: "/404"
     }],
     Ib = function(e) {
         const t = gm(e.routes, e),
             n = e.parseQuery || Sm,
```

### Comparing `swanlab-0.3.6/swanlab/template/assets/index-B7Izi8NT.css` & `swanlab-0.3.7/swanlab/template/assets/index-B7Izi8NT.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/template/assets/logo-ChHf2ozk.ico` & `swanlab-0.3.7/swanlab/template/assets/logo-ChHf2ozk.ico`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/utils/file.py` & `swanlab-0.3.7/swanlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/utils/font.py` & `swanlab-0.3.7/swanlab/utils/font.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/utils/judgment.py` & `swanlab-0.3.7/swanlab/utils/judgment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/swanlab/utils/key.py` & `swanlab-0.3.7/swanlab/utils/key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/create_experiment.py` & `swanlab-0.3.7/test/create_experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/start_server.py` & `swanlab-0.3.7/test/start_server.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/use_swanlog.py` & `swanlab-0.3.7/test/use_swanlog.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/integration/README.md` & `swanlab-0.3.7/test/integration/README.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/integration/fastai/fastai_train.py` & `swanlab-0.3.7/test/integration/fastai/fastai_train.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/integration/huggingface/transformers_bert_train.py` & `swanlab-0.3.7/test/integration/huggingface/transformers_bert_train.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/integration/lightning/lightning_base.py` & `swanlab-0.3.7/test/integration/lightning/lightning_base.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/integration/lightning/lightning_train.py` & `swanlab-0.3.7/test/integration/lightning/lightning_train.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/integration/sb3/sb3_PPO.py` & `swanlab-0.3.7/test/integration/sb3/sb3_PPO.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/unit/pytest_example.py` & `swanlab-0.3.7/test/unit/pytest_example.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/unit/data/pytest_sdk.py` & `swanlab-0.3.7/test/unit/data/pytest_sdk.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,99 +3,105 @@
 r"""
 @DATE: 2024/4/26 16:03
 @File: pytest_sdk.py
 @IDE: pycharm
 @Description:
     测试sdk的一些api
 """
-from swanlab import init
 from swanlab.env import (
     reset_env,
+    get_swanlab_folder,
     MODE,
     ROOT,
+    HOME
 )
-from tutils import TEMP_PATH
+import tutils as T
+import swanlab.data.sdk as S
+import swanlab.error as E
 from swanlab.log import swanlog
 from swanlab.data.run import get_run
 from nanoid import generate
 import pytest
 import os
 
 
 @pytest.fixture(scope="function", autouse=True)
 def setup_function():
     """
     在当前测试文件下的每个测试函数执行前后执行
     """
-    reset_env()
     swanlog.disable_log()
     yield
+    # 恢复原状
     swanlog.enable_log()
     if get_run() is not None:
         get_run().finish()
+    os.environ[ROOT] = T.SWANLAB_LOG_DIR
+    if HOME in os.environ:
+        del os.environ[HOME]
 
 
 class TestInitMode:
     """
     测试init时函数的mode参数设置行为
     """
 
     def test_init_disabled(self):
-        run = init(mode="disabled", logdir=generate())
+        run = S.init(mode="disabled", logdir=generate())
         assert os.environ[MODE] == "disabled"
         run.log({"TestInitMode": 1})  # 不会报错
         a = run.settings.run_dir
         assert not os.path.exists(a)
         assert get_run() is not None
 
     def test_init_local(self):
-        run = init(mode="local")
+        run = S.init(mode="local")
         assert os.environ[MODE] == "local"
         run.log({"TestInitMode": 1})  # 不会报错
         assert get_run() is not None
 
     def test_init_cloud(self):
-        run = init(mode="cloud")
+        run = S.init(mode="cloud")
         assert os.environ[MODE] == "cloud"
         run.log({"TestInitMode": 1})  # 不会报错
         assert get_run() is not None
 
     def test_init_error(self):
         with pytest.raises(ValueError):
-            init(mode="123456")
+            S.init(mode="123456")
         assert get_run() is None
 
     # ---------------------------------- 测试环境变量输入 ----------------------------------
 
     def test_init_disabled_env(self):
         os.environ[MODE] = "disabled"
-        run = init()
+        run = S.init()
         assert os.environ[MODE] == "disabled"
         run.log({"TestInitMode": 1})
         a = run.settings.run_dir
         assert not os.path.exists(a)
         assert get_run() is not None
 
     def test_init_local_env(self):
         os.environ[MODE] = "local"
-        run = init()
+        run = S.init()
         assert os.environ[MODE] == "local"
         run.log({"TestInitMode": 1})
 
     def test_init_cloud_env(self):
         os.environ[MODE] = "cloud"
-        run = init()
+        run = S.init()
         assert os.environ[MODE] == "cloud"
         run.log({"TestInitMode": 1})
 
     # ---------------------------------- 环境变量和mode的情况 ----------------------------------
 
     def test_init_disabled_env_mode(self):
         os.environ[MODE] = "local"
-        run = init(mode="disabled")
+        run = S.init(mode="disabled")
         assert os.environ[MODE] == "disabled"
         run.log({"TestInitMode": 1})
         a = run.settings.run_dir
         assert not os.path.exists(a)
         assert get_run() is not None
 
 
@@ -104,65 +110,93 @@
     测试init时函数的project参数设置行为
     """
 
     def test_init_project_none(self):
         """
         设置project为None
         """
-        run = init(project=None, mode="disabled")
+        run = S.init(project=None, mode="disabled")
         assert run.project_name == os.path.basename(os.getcwd())
 
     def test_init_project(self):
         """
         设置project为字符串
         """
         project = "test_project"
-        run = init(project=project, mode="disabled")
+        run = S.init(project=project, mode="disabled")
         assert run.project_name == project
 
 
 class TestInitLogdir:
     """
     测试init时函数的logdir参数设置行为
     """
 
     def test_init_logdir_disabled(self):
         """
         disabled模式下设置logdir不生效，采用的是环境变量的设置
         """
         logdir = generate()
-        run = init(logdir=logdir, mode="disabled")
+        run = S.init(logdir=logdir, mode="disabled")
         assert run.settings.swanlog_dir != logdir
         assert run.settings.swanlog_dir == os.environ[ROOT]
         run.finish()
         del os.environ[ROOT]
-        run = init(logdir=logdir, mode="disabled")
+        run = S.init(logdir=logdir, mode="disabled")
         assert run.settings.swanlog_dir != logdir
         assert run.settings.swanlog_dir == os.path.join(os.getcwd(), "swanlog")
 
     def test_init_logdir_enabled(self):
         """
         其他模式下设置logdir生效
         """
-        logdir = os.path.join(TEMP_PATH, generate()).__str__()
-        run = init(logdir=logdir, mode="local")
+        logdir = os.path.join(T.TEMP_PATH, generate()).__str__()
+        run = S.init(logdir=logdir, mode="local")
         assert run.settings.swanlog_dir == logdir
         run.finish()
         del os.environ[ROOT]
-        logdir = os.path.join(TEMP_PATH, generate()).__str__()
-        run = init(logdir=logdir, mode="local")
+        logdir = os.path.join(T.TEMP_PATH, generate()).__str__()
+        run = S.init(logdir=logdir, mode="local")
         assert run.settings.swanlog_dir == logdir
 
     def test_init_logdir_env(self):
         """
         通过环境变量设置logdir
         """
-        logdir = os.path.join(TEMP_PATH, generate()).__str__()
+        logdir = os.path.join(T.TEMP_PATH, generate()).__str__()
         os.environ[ROOT] = logdir
-        run = init(mode="local")
+        run = S.init(mode="local")
         assert run.settings.swanlog_dir == logdir
         run.finish()
         del os.environ[ROOT]
-        logdir = os.path.join(TEMP_PATH, generate()).__str__()
+        logdir = os.path.join(T.TEMP_PATH, generate()).__str__()
         os.environ[ROOT] = logdir
-        run = init(mode="local")
+        run = S.init(mode="local")
         assert run.settings.swanlog_dir == logdir
+
+
+class TestLogin:
+    """
+    测试通过sdk封装的login函数登录
+    不填apikey的部分不太好测
+    """
+
+    def test_use_home_key(self, monkeypatch):
+        """
+        使用家目录下的key，不需要输入
+        如果家目录下的key获取失败，会使用getpass.getpass要求用户输入，作为测试，使用monkeypatch替换getpass.getpass
+        """
+        os.environ[HOME] = T.TEMP_PATH
+        monkeypatch.setattr("getpass.getpass", T.get_password)
+        S.login()
+        # 默认保存Key
+        assert os.path.exists(os.path.join(get_swanlab_folder(), ".netrc"))
+
+    def test_use_input_key(self, monkeypatch):
+        """
+        使用输入的key
+        """
+        key = generate()
+        with pytest.raises(E.ValidationError):
+            S.login(api_key=key)
+        key = T.KEY
+        S.login(api_key=key)
```

### Comparing `swanlab-0.3.6/test/unit/data/run/pytest_main.py` & `swanlab-0.3.7/test/unit/data/run/pytest_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 r"""
 @DATE: 2024/4/26 16:03
 @File: pytest_main.py
 @IDE: pycharm
 @Description:
     测试SwanLabRun主类
 """
+import math
+
 from swanlab.data.run.main import SwanLabRun, get_run, SwanLabRunState, swanlog
 from swanlab import Image, Audio, Text
 from nanoid import generate
 from tutils import clear, TEMP_PATH
 from PIL import Image as PILImage
 import torch
 import soundfile as sf
@@ -128,14 +130,52 @@
         assert ac.sort == 0
         assert ac.config == {}
         assert ac.key == "a"
         assert ac.chart_type == "default"
         assert ac.namespace == "default"
         assert ac.reference == "step"
 
+    def test_log_number_inf(self):
+        """
+        测试解析一个inf
+        """
+        run = SwanLabRun()
+        metric_dict = run.log({"float(inf)": float("inf"), "math.inf": math.inf})
+        assert metric_dict["float(inf)"] is not None and metric_dict["math.inf"] is not None
+        assert len(metric_dict) == 2
+        a1 = metric_dict["float(inf)"]
+        a2 = metric_dict["math.inf"]
+        ac1 = a1.column_info
+        ac2 = a2.column_info
+        # ---------------------------------- 指标信息 ----------------------------------
+        assert a1.metric is None
+        assert a2.metric is None
+        # ---------------------------------- float(inf)信息 ----------------------------------
+        assert ac1.data_type == "default"
+        assert ac1.error["data_class"] == "INF"
+        assert ac1.error["excepted"] == ["float", "int"]
+        # 默认排在最前面
+        assert ac1.sort == 0
+        assert ac1.config == {}
+        assert ac1.key == "float(inf)"
+        assert ac1.chart_type == "default"
+        assert ac1.namespace == "default"
+        assert ac1.reference == "step"
+        # ---------------------------------- math.inf信息 ----------------------------------
+        assert ac2.data_type == "default"
+        assert ac2.error["data_class"] == "INF"
+        assert ac2.error["excepted"] == ["float", "int"]
+        # 默认排在最前面
+        assert ac2.sort == 0
+        assert ac2.config == {}
+        assert ac2.key == "math.inf"
+        assert ac2.chart_type == "default"
+        assert ac2.namespace == "default"
+        assert ac2.reference == "step"
+
     def test_log_number_str(self):
         """
         测试解析其他字符串
         """
         """
         测试解析一个nan
         """
```

### Comparing `swanlab-0.3.6/test/unit/log/pytest_log.py` & `swanlab-0.3.7/test/unit/log/pytest_log.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/unit/server/controller/utils/utils.py` & `swanlab-0.3.7/test/unit/server/controller/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/unit/utils/pytest_file.py` & `swanlab-0.3.7/test/unit/utils/pytest_file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/unit/utils/pytest_key.py` & `swanlab-0.3.7/test/unit/utils/pytest_key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/test/unit/utils/pytest_package.py` & `swanlab-0.3.7/test/unit/pytest_package.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-r"""
-@DATE: 2024/4/3 17:08
-@File: pytest_package.py
-@IDE: pycharm
-@Description:
-    测试package.py，提供测试时的包管理函数
-"""
 from tutils.config import nanoid
 import json
 from swanlab.package import (
     get_package_version,
     get_host_web,
     get_user_setting_path,
     get_host_api,
     get_project_url,
     get_experiment_url
 )
 import os
+from swanlab.package import get_package_latest_version
 
 PACKAGE_PATH = os.environ["SWANLAB_PACKAGE_PATH"]
 
 package_data = json.load(open(PACKAGE_PATH))
 
 
+def test_package_latest_version():
+    """
+    测试获取swanlab最新版本号
+    """
+    # 正常情况
+    assert isinstance(get_package_latest_version(), str)
+    # 超时情况
+    assert get_package_latest_version(timeout=1e-3) is None
+
+
 def mock_get_package_version():
     return get_package_version(PACKAGE_PATH)
 
 
 def mock_get_host_web():
     return get_host_web(PACKAGE_PATH)
```

### Comparing `swanlab-0.3.6/LICENSE` & `swanlab-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/pyproject.toml` & `swanlab-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.6/PKG-INFO` & `swanlab-0.3.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,1939 +1,1400 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 330a 4e61 6d65 3a20 7377 616e  : 2.3.Name: swan
-00000020: 6c61 620a 5665 7273 696f 6e3a 2030 2e33  lab.Version: 0.3
-00000030: 2e36 0a53 756d 6d61 7279 3a20 5079 7468  .6.Summary: Pyth
-00000040: 6f6e 206c 6962 7261 7279 2066 6f72 2073  on library for s
-00000050: 7472 6561 6d6c 696e 6564 2074 7261 636b  treamlined track
-00000060: 696e 6720 616e 6420 6d61 6e61 6765 6d65  ing and manageme
-00000070: 6e74 206f 6620 4149 2074 7261 696e 696e  nt of AI trainin
-00000080: 6720 7072 6f63 6573 7365 732e 0a50 726f  g processes..Pro
-00000090: 6a65 6374 2d55 524c 3a20 486f 6d65 7061  ject-URL: Homepa
-000000a0: 6765 2c20 6874 7470 733a 2f2f 7377 616e  ge, https://swan
-000000b0: 6875 622e 636f 0a50 726f 6a65 6374 2d55  hub.co.Project-U
-000000c0: 524c 3a20 536f 7572 6365 2c20 6874 7470  RL: Source, http
-000000d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-000000e0: 7761 6e48 7562 582f 5377 616e 4c61 620a  wanHubX/SwanLab.
-000000f0: 5072 6f6a 6563 742d 5552 4c3a 2042 7567  Project-URL: Bug
-00000100: 2052 6570 6f72 7473 2c20 6874 7470 733a   Reports, https:
-00000110: 2f2f 6769 7468 7562 2e63 6f6d 2f53 7761  //github.com/Swa
-00000120: 6e48 7562 582f 5377 616e 4c61 622f 6973  nHubX/SwanLab/is
-00000130: 7375 6573 0a50 726f 6a65 6374 2d55 524c  sues.Project-URL
-00000140: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
-00000150: 2068 7474 7073 3a2f 2f67 6565 6b74 6563   https://geektec
-00000160: 6873 7475 6469 6f2e 6665 6973 6875 2e63  hstudio.feishu.c
-00000170: 6e2f 7769 6b69 2f73 7061 6365 2f37 3331  n/wiki/space/731
-00000180: 3035 3933 3332 3533 3734 3031 3334 3434  0593325374013444
-00000190: 3f63 636d 5f6f 7065 6e5f 7479 7065 3d6c  ?ccm_open_type=l
-000001a0: 6172 6b5f 7769 6b69 5f73 7061 6365 4c69  ark_wiki_spaceLi
-000001b0: 6e6b 266f 7065 6e5f 7461 625f 6672 6f6d  nk&open_tab_from
-000001c0: 3d77 696b 695f 686f 6d65 0a41 7574 686f  =wiki_home.Autho
-000001d0: 722d 656d 6169 6c3a 2043 756e 7975 6520  r-email: Cunyue 
-000001e0: 3c74 6561 6d40 7377 616e 6875 622e 636f  <team@swanhub.co
-000001f0: 3e2c 2046 6575 6461 6c6d 616e 203c 7465  >, Feudalman <te
-00000200: 616d 4073 7761 6e68 7562 2e63 6f3e 2c20  am@swanhub.co>, 
-00000210: 5a65 5969 204c 696e 203c 7465 616d 4073  ZeYi Lin <team@s
-00000220: 7761 6e68 7562 2e63 6f3e 2c20 4b61 7368  wanhub.co>, Kash
-00000230: 6977 6142 7974 6520 3c74 6561 6d40 7377  iwaByte <team@sw
-00000240: 616e 6875 622e 636f 3e0a 4c69 6365 6e73  anhub.co>.Licens
-00000250: 652d 4578 7072 6573 7369 6f6e 3a20 4170  e-Expression: Ap
-00000260: 6163 6865 2d32 2e30 0a4c 6963 656e 7365  ache-2.0.License
-00000270: 2d46 696c 653a 204c 4943 454e 5345 0a4b  -File: LICENSE.K
-00000280: 6579 776f 7264 733a 206d 6163 6869 6e65  eywords: machine
-00000290: 206c 6561 726e 696e 672c 7265 7072 6f64   learning,reprod
-000002a0: 7563 6962 696c 6974 792c 7669 7375 616c  ucibility,visual
-000002b0: 697a 6174 696f 6e0a 436c 6173 7369 6669  ization.Classifi
-000002c0: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
-000002d0: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
-000002e0: 7068 610a 436c 6173 7369 6669 6572 3a20  pha.Classifier: 
-000002f0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000300: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
-00000310: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
-00000320: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
-00000330: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000340: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000350: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
-00000360: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000370: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000380: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
-00000390: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000003a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003b0: 3320 3a3a 204f 6e6c 790a 436c 6173 7369  3 :: Only.Classi
-000003c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003e0: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
-000003f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000400: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000410: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
-00000420: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000430: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000440: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000450: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000460: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000470: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000480: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
-00000490: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000004a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000004b0: 3a20 332e 3132 0a43 6c61 7373 6966 6965  : 3.12.Classifie
-000004c0: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
-000004d0: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-000004e0: 6e67 0a43 6c61 7373 6966 6965 723a 2054  ng.Classifier: T
-000004f0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000500: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-00000510: 3a20 4172 7469 6669 6369 616c 2049 6e74  : Artificial Int
-00000520: 656c 6c69 6765 6e63 650a 436c 6173 7369  elligence.Classi
-00000530: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000540: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000550: 6572 696e 6720 3a3a 2056 6973 7561 6c69  ering :: Visuali
-00000560: 7a61 7469 6f6e 0a52 6571 7569 7265 732d  zation.Requires-
-00000570: 5079 7468 6f6e 3a20 3e3d 332e 380a 5265  Python: >=3.8.Re
-00000580: 7175 6972 6573 2d44 6973 743a 2063 6c69  quires-Dist: cli
-00000590: 636b 0a52 6571 7569 7265 732d 4469 7374  ck.Requires-Dist
-000005a0: 3a20 636f 732d 7079 7468 6f6e 2d73 646b  : cos-python-sdk
-000005b0: 2d76 350a 5265 7175 6972 6573 2d44 6973  -v5.Requires-Dis
-000005c0: 743a 2066 6173 7461 7069 3e3d 302e 3131  t: fastapi>=0.11
-000005d0: 302e 310a 5265 7175 6972 6573 2d44 6973  0.1.Requires-Dis
-000005e0: 743a 206e 756d 7079 0a52 6571 7569 7265  t: numpy.Require
-000005f0: 732d 4469 7374 3a20 7065 6577 6565 0a52  s-Dist: peewee.R
-00000600: 6571 7569 7265 732d 4469 7374 3a20 7069  equires-Dist: pi
-00000610: 6c6c 6f77 0a52 6571 7569 7265 732d 4469  llow.Requires-Di
-00000620: 7374 3a20 7073 7574 696c 0a52 6571 7569  st: psutil.Requi
-00000630: 7265 732d 4469 7374 3a20 7079 6e76 6d6c  res-Dist: pynvml
-00000640: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000650: 7079 7961 6d6c 0a52 6571 7569 7265 732d  pyyaml.Requires-
-00000660: 4469 7374 3a20 7265 7175 6573 7473 0a52  Dist: requests.R
-00000670: 6571 7569 7265 732d 4469 7374 3a20 736f  equires-Dist: so
-00000680: 756e 6466 696c 650a 5265 7175 6972 6573  undfile.Requires
-00000690: 2d44 6973 743a 2075 6a73 6f6e 0a52 6571  -Dist: ujson.Req
-000006a0: 7569 7265 732d 4469 7374 3a20 7576 6963  uires-Dist: uvic
-000006b0: 6f72 6e3e 3d30 2e31 342e 300a 5265 7175  orn>=0.14.0.Requ
-000006c0: 6972 6573 2d44 6973 743a 2077 6174 6368  ires-Dist: watch
-000006d0: 646f 670a 5072 6f76 6964 6573 2d45 7874  dog.Provides-Ext
-000006e0: 7261 3a20 6f61 7574 680a 4465 7363 7269  ra: oauth.Descri
-000006f0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000700: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000710: 6e0a 0a21 5b4f 7665 7276 6965 775d 2868  n..![Overview](h
-00000720: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000730: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000740: 2f53 7761 6e48 7562 582f 7377 616e 6c61  /SwanHubX/swanla
-00000750: 622f 6d61 696e 2f72 6561 646d 655f 6669  b/main/readme_fi
-00000760: 6c65 732f 7377 616e 6c61 622d 6f76 6572  les/swanlab-over
-00000770: 7669 6577 2d6e 6577 2e70 6e67 290a 0a3c  view-new.png)..<
-00000780: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000790: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-000007a0: 3a2f 2f73 7761 6e6c 6162 2e63 6e22 3e53  ://swanlab.cn">S
-000007b0: 7761 6e4c 6162 2043 6c6f 7564 3c2f 613e  wanLab Cloud</a>
-000007c0: 20c2 b720 3c61 2068 7265 663d 2268 7474   .. <a href="htt
-000007d0: 7073 3a2f 2f64 6f63 732e 7377 616e 6c61  ps://docs.swanla
-000007e0: 622e 636e 223e 446f 6375 6d65 6e74 3c2f  b.cn">Document</
-000007f0: 613e 20c2 b720 3c61 2068 7265 663d 2268  a> .. <a href="h
-00000800: 7474 7073 3a2f 2f67 6565 6b74 6563 6873  ttps://geektechs
-00000810: 7475 6469 6f2e 6665 6973 6875 2e63 6e2f  tudio.feishu.cn/
-00000820: 7769 6b69 2f4e 495a 3977 7035 4c52 6953  wiki/NIZ9wp5LRiS
-00000830: 7151 796b 697a 6247 6356 7a55 4b6e 6963  qQykizbGcVzUKnic
-00000840: 223e 5765 4368 6174 3c2f 613e 20c2 b720  ">WeChat</a> .. 
-00000850: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000860: 2f67 6974 6875 622e 636f 6d2f 7377 616e  /github.com/swan
-00000870: 6875 6278 2f73 7761 6e6c 6162 2f69 7373  hubx/swanlab/iss
-00000880: 7565 7322 3e52 6570 6f72 7420 4973 7375  ues">Report Issu
-00000890: 653c 2f61 3e20 c2b7 203c 6120 6872 6566  e</a> .. <a href
-000008a0: 3d22 6874 7470 733a 2f2f 6765 656b 7465  ="https://geekte
-000008b0: 6368 7374 7564 696f 2e66 6569 7368 752e  chstudio.feishu.
-000008c0: 636e 2f73 6861 7265 2f62 6173 652f 666f  cn/share/base/fo
-000008d0: 726d 2f73 6872 636e 7942 6c4b 384f 4d44  rm/shrcnyBlK8OMD
-000008e0: 3065 7765 6f46 6363 3253 7657 4b63 223e  0eweoFcc2SvWKc">
-000008f0: 4665 6564 6261 636b 3c2f 613e 20c2 b720  Feedback</a> .. 
-00000900: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000910: 2f67 6974 6875 622e 636f 6d2f 5377 616e  /github.com/Swan
-00000920: 4875 6258 2f53 7761 6e4c 6162 2f62 6c6f  HubX/SwanLab/blo
-00000930: 622f 6d61 696e 2f43 4841 4e47 454c 4f47  b/main/CHANGELOG
-00000940: 2e6d 6422 3e43 6861 6e67 656c 6f67 3c2f  .md">Changelog</
-00000950: 613e 0a0a 0a3c 2f70 3e0a 0a3c 7020 616c  a>...</p>..<p al
-00000960: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000970: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000980: 2f67 6974 6875 622e 636f 6d2f 5377 616e  /github.com/Swan
-00000990: 4875 6258 2f53 7761 6e4c 6162 2f62 6c6f  HubX/SwanLab/blo
-000009a0: 622f 6d61 696e 2f4c 4943 454e 5345 223e  b/main/LICENSE">
-000009b0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000009c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000009d0: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
-000009e0: 5377 616e 4875 6258 2f53 7761 6e4c 6162  SwanHubX/SwanLab
-000009f0: 2e73 7667 3f63 6f6c 6f72 3d62 7269 6768  .svg?color=brigh
-00000a00: 7467 7265 656e 2220 616c 743d 226c 6963  tgreen" alt="lic
-00000a10: 656e 7365 223e 3c2f 613e 0a20 203c 6120  ense"></a>.  <a 
-00000a20: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000a30: 7468 7562 2e63 6f6d 2f53 7761 6e48 7562  thub.com/SwanHub
-00000a40: 582f 5377 616e 4c61 622f 636f 6d6d 6974  X/SwanLab/commit
-00000a50: 732f 6d61 696e 223e 3c69 6d67 2073 7263  s/main"><img src
-00000a60: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000a70: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000a80: 6c61 7374 2d63 6f6d 6d69 742f 5377 616e  last-commit/Swan
-00000a90: 4875 6258 2f53 7761 6e4c 6162 2220 616c  HubX/SwanLab" al
-00000aa0: 743d 226c 6963 656e 7365 223e 3c2f 613e  t="license"></a>
-00000ab0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00000ac0: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
-00000ad0: 6f72 672f 7079 7069 2f73 7761 6e6c 6162  org/pypi/swanlab
-00000ae0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00000af0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000b00: 696f 2f70 7970 692f 762f 7377 616e 6c61  io/pypi/v/swanla
-00000b10: 623f 636f 6c6f 723d 6f72 616e 6765 2220  b?color=orange" 
-00000b20: 616c 743d 202f 3e3c 2f61 3e0a 2020 3c61  alt= /></a>.  <a
-00000b30: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-00000b40: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
-00000b50: 2f73 7761 6e6c 6162 223e 3c69 6d67 2061  /swanlab"><img a
-00000b60: 6c74 3d22 7079 7069 2044 6f77 6e6c 6f61  lt="pypi Downloa
-00000b70: 6422 2073 7263 3d22 6874 7470 733a 2f2f  d" src="https://
-00000b80: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
-00000b90: 2f62 6164 6765 2f73 7761 6e6c 6162 223e  /badge/swanlab">
-00000ba0: 3c2f 613e 0a20 203c 6120 6872 6566 3d22  </a>.  <a href="
-00000bb0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000bc0: 6f6d 2f73 7761 6e68 7562 782f 7377 616e  om/swanhubx/swan
-00000bd0: 6c61 622f 6973 7375 6573 223e 3c69 6d67  lab/issues"><img
-00000be0: 2061 6c74 3d22 6973 7375 6573 2220 7372   alt="issues" sr
-00000bf0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000c00: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000c10: 2f69 7373 7565 732f 7377 616e 6875 6278  /issues/swanhubx
-00000c20: 2f73 7761 6e6c 6162 223e 3c2f 613e 0a20  /swanlab"></a>. 
-00000c30: 203c 6272 3e0a 2020 3c61 2068 7265 663d   <br>.  <a href=
-00000c40: 2268 7474 7073 3a2f 2f73 7761 6e6c 6162  "https://swanlab
-00000c50: 2e63 6e22 2074 6172 6765 743d 225f 626c  .cn" target="_bl
-00000c60: 616e 6b22 3e0a 2020 2020 2020 2020 3c69  ank">.        <i
-00000c70: 6d67 2061 6c74 3d22 5374 6174 6963 2042  mg alt="Static B
-00000c80: 6164 6765 2220 7372 633d 2268 7474 7073  adge" src="https
-00000c90: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000ca0: 6f2f 6261 6467 652f 5072 6f64 7563 742d  o/badge/Product-
-00000cb0: 5377 616e 4c61 62e4 ba91 e7ab afe7 8988  SwanLab.........
-00000cc0: 2d36 3336 6133 6622 3e3c 2f61 3e0a 2020  -636a3f"></a>.  
-00000cd0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000ce0: 2f67 6565 6b74 6563 6873 7475 6469 6f2e  /geektechstudio.
-00000cf0: 6665 6973 6875 2e63 6e2f 7769 6b69 2f4e  feishu.cn/wiki/N
-00000d00: 495a 3977 7035 4c52 6953 7151 796b 697a  IZ9wp5LRiSqQykiz
-00000d10: 6247 6356 7a55 4b6e 6963 2220 7461 7267  bGcVzUKnic" targ
-00000d20: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
-00000d30: 2020 2020 203c 696d 6720 616c 743d 2253       <img alt="S
-00000d40: 7461 7469 6320 4261 6467 6522 2073 7263  tatic Badge" src
-00000d50: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000d60: 6965 6c64 732e 696f 2f62 6164 6765 2f57  ields.io/badge/W
-00000d70: 6543 6861 742d e5be aee4 bfa1 2d34 6362  eChat-......-4cb
-00000d80: 3535 6522 3e3c 2f61 3e0a 2020 3c61 2068  55e"></a>.  <a h
-00000d90: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
-00000da0: 2e78 6961 6f68 6f6e 6773 6875 2e63 6f6d  .xiaohongshu.com
-00000db0: 2f75 7365 722f 7072 6f66 696c 652f 3630  /user/profile/60
-00000dc0: 3537 3836 6239 3030 3030 3030 3030 3031  5786b90000000001
-00000dd0: 3030 3361 3831 2220 7461 7267 6574 3d22  003a81" target="
-00000de0: 5f62 6c61 6e6b 223e 0a20 2020 2020 2020  _blank">.       
-00000df0: 203c 696d 6720 616c 743d 2253 7461 7469   <img alt="Stati
-00000e00: 6320 4261 6467 6522 2073 7263 3d22 6874  c Badge" src="ht
-00000e10: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000e20: 732e 696f 2f62 6164 6765 2fe5 b08f e7ba  s.io/badge/.....
-00000e30: a2e4 b9a6 2d46 3034 3433 3822 3e3c 2f61  ....-F04438"></a
-00000e40: 3e0a 0a3c 2f70 3e0a 0a3c 6469 7620 616c  >..</p>..<div al
-00000e50: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000e60: 3c61 2068 7265 663d 222e 2f68 7474 7073  <a href="./https
-00000e70: 3a2f 2f67 6974 6875 622e 636f 6d2f 5377  ://github.com/Sw
-00000e80: 616e 4875 6258 2f53 7761 6e4c 6162 2f62  anHubX/SwanLab/b
-00000e90: 6c6f 622f 6d61 696e 2f52 4541 444d 452e  lob/main/README.
-00000ea0: 6d64 223e 3c69 6d67 2061 6c74 3d22 e88b  md"><img alt="..
-00000eb0: b1e6 9687 e696 87e6 a1a3 2220 7372 633d  .........." src=
-00000ec0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000ed0: 656c 6473 2e69 6f2f 6261 6467 652f 456e  elds.io/badge/En
-00000ee0: 676c 6973 682d 6439 6439 6439 223e 3c2f  glish-d9d9d9"></
-00000ef0: 613e 0a20 203c 6120 6872 6566 3d22 2e2f  a>.  <a href="./
-00000f00: 5245 4144 4d45 5f63 6e2e 6d64 223e 3c69  README_cn.md"><i
-00000f10: 6d67 2061 6c74 3d22 e4b8 ade6 9687 e696  mg alt="........
-00000f20: 87e6 a1a3 2220 7372 633d 2268 7474 7073  ...." src="https
-00000f30: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000f40: 6f2f 6261 6467 652f e7ae 80e4 bd93 e4b8  o/badge/........
-00000f50: ade6 9687 2d64 3964 3964 3922 3e3c 2f61  ....-d9d9d9"></a
-00000f60: 3e0a 3c2f 6469 763e 0a0a 3c64 6574 6169  >.</div>..<detai
-00000f70: 6c73 3e0a 3c73 756d 6d61 7279 3e54 6162  ls>.<summary>Tab
-00000f80: 6c65 206f 6620 636f 6e74 656e 7473 3c2f  le of contents</
-00000f90: 7375 6d6d 6172 793e 0a0a 2323 2323 2054  summary>..#### T
-00000fa0: 4f43 0a0a 2d20 5bf0 9f91 8bf0 9f8f bb20  OC..- [........ 
-00000fb0: 496e 7472 6f64 7563 7469 6f6e 5d28 232d  Introduction](#-
-00000fc0: 496e 7472 6f64 7563 7469 6f6e 290a 2d20  Introduction).- 
-00000fd0: 5bf0 9f8f 8120 5175 6963 6b20 5374 6172  [.... Quick Star
-00000fe0: 745d 2823 f09f 8f81 2d71 7569 636b 2d73  t](#....-quick-s
-00000ff0: 7461 7274 290a 2020 2020 2d20 5b31 2e49  tart).    - [1.I
-00001000: 6e73 7461 6c6c 6174 696f 6e5d 2823 3169  nstallation](#1i
-00001010: 6e73 7461 6c6c 6174 696f 6e29 0a20 2020  nstallation).   
-00001020: 202d 205b 322e 4c6f 6720 496e 2061 6e64   - [2.Log In and
-00001030: 2047 6574 2074 6865 2041 5049 204b 6579   Get the API Key
-00001040: 5d28 2332 6c6f 672d 696e 2d61 6e64 2d67  ](#2log-in-and-g
-00001050: 6574 2d74 6865 2d61 7069 2d6b 6579 290a  et-the-api-key).
-00001060: 2020 2020 2d20 5b33 2e49 6e74 6567 7261      - [3.Integra
-00001070: 7465 2053 7761 6e4c 6162 2077 6974 6820  te SwanLab with 
-00001080: 596f 7572 2043 6f64 655d 2823 332d 696e  Your Code](#3-in
-00001090: 7465 6772 6174 652d 7377 616e 6c61 622d  tegrate-swanlab-
-000010a0: 7769 7468 2d79 6f75 722d 636f 6465 290a  with-your-code).
-000010b0: 2d20 5bf0 9f93 8320 4d6f 7265 2045 7861  - [.... More Exa
-000010c0: 6d70 6c65 735d 2823 2d6d 6f72 652d 6578  mples](#-more-ex
-000010d0: 616d 706c 6573 290a 2d20 5bf0 9f92 bb20  amples).- [.... 
-000010e0: 5365 6c66 2d68 6f73 7465 645d 2823 2d73  Self-hosted](#-s
-000010f0: 656c 662d 686f 7374 6564 290a 2020 2020  elf-hosted).    
-00001100: 2d20 5b4f 6666 6c69 6e65 2045 7870 6572  - [Offline Exper
-00001110: 696d 656e 7420 5472 6163 6b69 6e67 5d28  iment Tracking](
-00001120: 236f 6666 6c69 6e65 2d65 7870 6572 696d  #offline-experim
-00001130: 656e 742d 7472 6163 6b69 6e67 290a 2020  ent-tracking).  
-00001140: 2020 2d20 5b4f 7065 6e20 4f66 666c 696e    - [Open Offlin
-00001150: 6520 4461 7368 626f 6172 645d 2823 6f70  e Dashboard](#op
-00001160: 656e 2d6f 6666 6c69 6e65 2d62 6f61 7264  en-offline-board
-00001170: 290a 2d20 5bf0 9f9a 9720 496e 7465 6772  ).- [.... Integr
-00001180: 6174 696f 6e5d 2823 2d69 6e74 6567 7261  ation](#-integra
-00001190: 7469 6f6e 290a 2d20 5bf0 9f86 9a20 436f  tion).- [.... Co
-000011a0: 6d70 6172 6973 6f6e 2077 6974 6820 4661  mparison with Fa
-000011b0: 6d69 6c69 6172 2054 6f6f 6c73 5d28 232d  miliar Tools](#-
-000011c0: 636f 6d70 6172 6973 6f6e 2d77 6974 682d  comparison-with-
-000011d0: 6661 6d69 6c69 6172 2d74 6f6f 6c73 290a  familiar-tools).
-000011e0: 2020 2020 2d20 5b54 656e 736f 7262 6f61      - [Tensorboa
-000011f0: 7264 2076 7320 5377 616e 4c61 625d 2823  rd vs SwanLab](#
-00001200: 7465 6e73 6f72 626f 6172 642d 7673 2d73  tensorboard-vs-s
-00001210: 7761 6e6c 6162 290a 2020 2020 2d20 5b57  wanlab).    - [W
-00001220: 6569 6768 7473 2026 2042 6961 7365 7320  eights & Biases 
-00001230: 7673 2053 7761 6e4c 6162 5d28 2377 6569  vs SwanLab](#wei
-00001240: 6768 7473 2d61 6e64 2d62 6961 7365 732d  ghts-and-biases-
-00001250: 7673 2d73 7761 6e6c 6162 290a 2d20 5bf0  vs-swanlab).- [.
-00001260: 9f9b a3ef b88f 2052 6f61 646d 6170 5d28  ...... Roadmap](
-00001270: 2325 4546 2542 3825 3846 2d72 6f61 646d  #%EF%B8%8F-roadm
-00001280: 6170 290a 2020 2020 2d20 5b49 6e20 5072  ap).    - [In Pr
-00001290: 6f67 7265 7373 204e 6f77 5d28 2369 6e2d  ogress Now](#in-
-000012a0: 7072 6f67 7265 7373 2d6e 6f77 290a 2020  progress-now).  
-000012b0: 2020 2d20 5b4e 6578 7420 506c 616e 6e65    - [Next Planne
-000012c0: 645d 2823 6e65 7874 2d70 6c61 6e6e 6564  d](#next-planned
-000012d0: 290a 2020 2020 2d20 5b4c 6f6e 6720 5465  ).    - [Long Te
-000012e0: 726d 2043 6f6e 6365 726e 5d28 236c 6f6e  rm Concern](#lon
-000012f0: 672d 7465 726d 2d63 6f6e 6365 726e 290a  g-term-concern).
-00001300: 2d20 5bf0 9f91 a520 436f 6d6d 756e 6974  - [.... Communit
-00001310: 795d 2823 2d63 6f6d 6d75 6e69 7479 290a  y](#-community).
-00001320: 2020 2020 2d20 5b43 6f6d 6d75 6e69 7479      - [Community
-00001330: 2061 6e64 2053 7570 706f 7274 5d28 2363   and Support](#c
-00001340: 6f6d 6d75 6e69 7479 2d61 6e64 2d73 7570  ommunity-and-sup
-00001350: 706f 7274 290a 2020 2020 2d20 5b53 7761  port).    - [Swa
-00001360: 6e4c 6162 2052 4541 444d 4520 4261 6467  nLab README Badg
-00001370: 655d 2823 7377 616e 6c61 622d 7265 6164  e](#swanlab-read
-00001380: 6d65 2d62 6164 6765 290a 2020 2020 2d20  me-badge).    - 
-00001390: 5b43 6974 696e 6720 5377 616e 4c61 6220  [Citing SwanLab 
-000013a0: 696e 2074 6865 2050 6170 6572 5d28 2363  in the Paper](#c
-000013b0: 6974 696e 672d 7377 616e 6c61 622d 696e  iting-swanlab-in
-000013c0: 2d74 6865 2d70 6170 6572 290a 2020 2020  -the-paper).    
-000013d0: 2d20 5b43 6f6e 7472 6962 7574 6520 746f  - [Contribute to
-000013e0: 2053 7761 6e4c 6162 5d28 2363 6f6e 7472   SwanLab](#contr
-000013f0: 6962 7574 652d 746f 2d73 7761 6e6c 6162  ibute-to-swanlab
-00001400: 290a 2020 2020 2d20 5b44 6f77 6e6c 6f61  ).    - [Downloa
-00001410: 6420 4963 6f6e 5d28 2364 6f77 6e6c 6f61  d Icon](#downloa
-00001420: 642d 6963 6f6e 290a 2d20 5bf0 9f93 8320  d-icon).- [.... 
-00001430: 4c69 6365 6e73 655d 2823 2d6c 6963 656e  License](#-licen
-00001440: 7365 290a 0a3c 6272 2f3e 0a0a 3c2f 6465  se)..<br/>..</de
-00001450: 7461 696c 733e 0a0a 2323 20f0 9f91 8bf0  tails>..## .....
-00001460: 9f8f bb20 496e 7472 6f64 7563 7469 6f6e  ... Introduction
-00001470: 0a0a 5377 616e 4c61 6220 6973 2061 6e20  ..SwanLab is an 
-00001480: 6f70 656e 2d73 6f75 7263 652c 206c 6967  open-source, lig
-00001490: 6874 7765 6967 6874 2041 4920 6578 7065  htweight AI expe
-000014a0: 7269 6d65 6e74 2074 7261 636b 696e 6720  riment tracking 
-000014b0: 746f 6f6c 2074 6861 7420 7072 6f76 6964  tool that provid
-000014c0: 6573 2061 2070 6c61 7466 6f72 6d20 666f  es a platform fo
-000014d0: 7220 7472 6163 6b69 6e67 2c20 636f 6d70  r tracking, comp
-000014e0: 6172 696e 672c 2061 6e64 0a63 6f6c 6c61  aring, and.colla
-000014f0: 626f 7261 7469 6e67 206f 6e20 6578 7065  borating on expe
-00001500: 7269 6d65 6e74 732c 2061 696d 696e 6720  riments, aiming 
-00001510: 746f 2061 6363 656c 6572 6174 6520 7468  to accelerate th
-00001520: 6520 7265 7365 6172 6368 2061 6e64 2064  e research and d
-00001530: 6576 656c 6f70 6d65 6e74 2065 6666 6963  evelopment effic
-00001540: 6965 6e63 7920 6f66 2041 4920 7465 616d  iency of AI team
-00001550: 7320 6279 2031 3030 2074 696d 6573 2e0a  s by 100 times..
-00001560: 0a53 7761 6e4c 6162 e698 afe4 b880 e4b8  .SwanLab........
-00001570: aae5 bc80 e6ba 90e3 8081 e8bd bbe9 878f  ................
-00001580: e7ba a7e7 9a84 4149 e5ae 9ee9 aa8c e8b7  ......AI........
-00001590: 9fe8 b8aa e5b7 a5e5 85b7 efbc 8ce6 8f90  ................
-000015a0: e4be 9be4 ba86 e4b8 80e4 b8aa e8b7 9fe8  ................
-000015b0: b8aa e380 81e6 af94 e8be 83e3 8081 e592  ................
-000015c0: 8ce5 8d8f e4bd 9ce5 ae9e e9aa 8ce7 9a84  ................
-000015d0: e5b9 b3e5 8fb0 efbc 8ce6 97a8 e59c a8e5  ................
-000015e0: 8aa0 e980 9f41 49e7 a094 e58f 91e5 9ba2  .....AI.........
-000015f0: e998 9f31 3030 e580 8de7 9a84 e7a0 94e5  ...100..........
-00001600: 8f91 e695 88e7 8e87 e380 820a 0a49 7420  .............It 
-00001610: 6f66 6665 7273 2061 2075 7365 722d 6672  offers a user-fr
-00001620: 6965 6e64 6c79 2041 5049 2061 6e64 2061  iendly API and a
-00001630: 2064 6563 656e 7420 696e 7465 7266 6163   decent interfac
-00001640: 652c 2063 6f6d 6269 6e69 6e67 2066 6561  e, combining fea
-00001650: 7475 7265 7320 7375 6368 2061 7320 7472  tures such as tr
-00001660: 6163 6b69 6e67 2068 7970 6572 7061 7261  acking hyperpara
-00001670: 6d65 7465 722c 2072 6563 6f72 6469 6e67  meter, recording
-00001680: 0a6d 6574 7269 632c 206f 6e6c 696e 6520  .metric, online 
-00001690: 636f 6c6c 6162 6f72 6174 696f 6e2c 2073  collaboration, s
-000016a0: 6861 7269 6e67 2065 7870 6572 696d 656e  haring experimen
-000016b0: 7420 6c69 6e6b 2c20 7265 616c 2d74 696d  t link, real-tim
-000016c0: 6520 6d65 7373 6167 6520 6e6f 7469 6669  e message notifi
-000016d0: 6361 7469 6f6e 732c 2061 6c6c 6f77 696e  cations, allowin
-000016e0: 6720 796f 7520 746f 2071 7569 636b 6c79  g you to quickly
-000016f0: 2074 7261 636b 204d 4c0a 6578 7065 7269   track ML.experi
-00001700: 6d65 6e74 732c 2076 6973 7561 6c69 7a65  ments, visualize
-00001710: 2070 726f 6365 7373 6573 2c20 616e 6420   processes, and 
-00001720: 7368 6172 6520 7769 7468 2070 6565 7273  share with peers
-00001730: 2e0a 0a42 7920 7573 696e 672c 2072 6573  ...By using, res
-00001740: 6561 7263 6865 7273 2063 616e 2061 6363  earchers can acc
-00001750: 756d 756c 6174 6520 7468 6569 7220 7472  umulate their tr
-00001760: 6169 6e69 6e67 2065 7870 6572 6965 6e63  aining experienc
-00001770: 6573 2061 6e64 2073 6561 6d6c 6573 736c  es and seamlessl
-00001780: 7920 636f 6d6d 756e 6963 6174 6520 616e  y communicate an
-00001790: 6420 636f 6c6c 6162 6f72 6174 6520 7769  d collaborate wi
-000017a0: 7468 2070 6565 7273 2e0a 4d61 6368 696e  th peers..Machin
-000017b0: 6520 6c65 6172 6e69 6e67 2065 6e67 696e  e learning engin
-000017c0: 6565 7273 2063 616e 2064 6576 656c 6f70  eers can develop
-000017d0: 206d 6f64 656c 7320 666f 7220 7072 6f64   models for prod
-000017e0: 7563 7469 6f6e 206d 6f72 6520 6566 6669  uction more effi
-000017f0: 6369 656e 746c 792e 0a0a 215b 5d28 6874  ciently...![](ht
-00001800: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00001810: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001820: 5377 616e 4875 6258 2f73 7761 6e6c 6162  SwanHubX/swanlab
-00001830: 2f6d 6169 6e2f 7265 6164 6d65 5f66 696c  /main/readme_fil
-00001840: 6573 2f69 6e74 726f 6475 6374 696f 6e2e  es/introduction.
-00001850: 706e 6729 0a0a 4865 7265 2069 7320 7468  png)..Here is th
-00001860: 6520 456e 676c 6973 6820 7665 7273 696f  e English versio
-00001870: 6e20 6f66 2074 6865 2063 6f72 6520 6665  n of the core fe
-00001880: 6174 7572 6520 6c69 7374 2066 6f72 2061  ature list for a
-00001890: 6e20 4149 2070 6c61 7466 6f72 6d3a 0a0a  n AI platform:..
-000018a0: 2a2a 312e 20f0 9f93 8a20 4578 7065 7269  **1. .... Experi
-000018b0: 6d65 6e74 616c 204d 6574 7269 6373 2061  mental Metrics a
-000018c0: 6e64 2054 7261 636b 696e 6720 4879 7065  nd Tracking Hype
-000018d0: 7270 6172 616d 6574 6572 2a2a 3a20 456d  rparameter**: Em
-000018e0: 6265 6420 796f 7572 206d 6163 6869 6e65  bed your machine
-000018f0: 206c 6561 726e 696e 6720 7069 7065 6c69   learning pipeli
-00001900: 6e65 2077 6974 6820 6d69 6e69 6d61 6c69  ne with minimali
-00001910: 7374 6963 2063 6f64 650a 616e 6420 7472  stic code.and tr
-00001920: 6163 6b20 6b65 7920 7472 6169 6e69 6e67  ack key training
-00001930: 206d 6574 7269 6373 2e0a 0a2d 2046 6c65   metrics...- Fle
-00001940: 7869 626c 6520 7265 636f 7264 696e 6720  xible recording 
-00001950: 6f66 2068 7970 6572 7061 7261 6d65 7465  of hyperparamete
-00001960: 7273 2061 6e64 2065 7870 6572 696d 656e  rs and experimen
-00001970: 7420 636f 6e66 6967 7572 6174 696f 6e73  t configurations
-00001980: 2e0a 2d20 2a2a 5375 7070 6f72 7465 6420  ..- **Supported 
-00001990: 6d65 7461 6461 7461 2074 7970 6573 2a2a  metadata types**
-000019a0: 3a20 7363 616c 6172 206d 6574 7269 6373  : scalar metrics
-000019b0: 2c20 696d 6167 6573 2c20 6175 6469 6f2c  , images, audio,
-000019c0: 2074 6578 742c 2065 7463 2e0a 2d20 2a2a   text, etc..- **
-000019d0: 5375 7070 6f72 7465 6420 6368 6172 7420  Supported chart 
-000019e0: 7479 7065 732a 2a3a 206c 696e 6520 6772  types**: line gr
-000019f0: 6170 6873 2c20 6d65 6469 6120 6368 6172  aphs, media char
-00001a00: 7473 2028 696d 6167 6573 2c20 6175 6469  ts (images, audi
-00001a10: 6f2c 2074 6578 7429 2c20 6574 632e 0a2d  o, text), etc..-
-00001a20: 202a 2a41 7574 6f6d 6174 6963 206c 6f67   **Automatic log
-00001a30: 6769 6e67 2a2a 3a20 636f 6e73 6f6c 6520  ging**: console 
-00001a40: 6c6f 6767 696e 672c 2047 5055 2068 6172  logging, GPU har
-00001a50: 6477 6172 652c 2047 6974 2069 6e66 6f72  dware, Git infor
-00001a60: 6d61 7469 6f6e 2c20 5079 7468 6f6e 2069  mation, Python i
-00001a70: 6e74 6572 7072 6574 6572 2c20 6c69 7374  nterpreter, list
-00001a80: 206f 6620 5079 7468 6f6e 206c 6962 7261   of Python libra
-00001a90: 7269 6573 2c0a 2020 636f 6465 2064 6972  ries,.  code dir
-00001aa0: 6563 746f 7279 2e0a 0a2a 2a32 2e20 e29a  ectory...**2. ..
-00001ab0: a1ef b88f 2043 6f6d 7072 6568 656e 7369  .... Comprehensi
-00001ac0: 7665 2046 7261 6d65 776f 726b 2049 6e74  ve Framework Int
-00001ad0: 6567 7261 7469 6f6e 2a2a 3a20 5079 546f  egration**: PyTo
-00001ae0: 7263 68e3 8081 5465 6e73 6f72 666c 6f77  rch...Tensorflow
-00001af0: e380 8150 7954 6f72 6368 204c 6967 6874  ...PyTorch Light
-00001b00: 6e69 6e67 e380 81f0 9fa4 9748 7567 6769  ning.......Huggi
-00001b10: 6e67 4661 6365 e380 8154 7261 6e73 666f  ngFace...Transfo
-00001b20: 726d 6572 73e3 8081 4d4d 456e 6769 6e65  rmers...MMEngine
-00001b30: e380 8155 6c74 7261 6c79 7469 6373 e380  ...Ultralytics..
-00001b40: 8166 6173 7461 69e3 8081 5465 6e73 6f72  .fastai...Tensor
-00001b50: 626f 6172 64e3 8081 4f70 656e 4149 e380  board...OpenAI..
-00001b60: 815a 6869 7075 4149 e380 8148 7964 7261  .ZhipuAI...Hydra
-00001b70: e380 812e 2e2e 0a0a 2a2a 332e 20f0 9f93  ........**3. ...
-00001b80: a620 4f72 6761 6e69 7a69 6e67 2045 7870  . Organizing Exp
-00001b90: 6572 696d 656e 7473 2a2a 3a20 4365 6e74  eriments**: Cent
-00001ba0: 7261 6c69 7a65 6420 6461 7368 626f 6172  ralized dashboar
-00001bb0: 6420 666f 7220 6566 6669 6369 656e 746c  d for efficientl
-00001bc0: 7920 6d61 6e61 6769 6e67 206d 756c 7469  y managing multi
-00001bd0: 706c 6520 7072 6f6a 6563 7473 2061 6e64  ple projects and
-00001be0: 2065 7870 6572 696d 656e 7473 2c0a 7072   experiments,.pr
-00001bf0: 6f76 6964 696e 6720 616e 206f 7665 7276  oviding an overv
-00001c00: 6965 7720 6f66 2074 7261 696e 696e 6720  iew of training 
-00001c10: 6174 2061 2067 6c61 6e63 652e 0a0a 2a2a  at a glance...**
-00001c20: 342e 20f0 9f86 9a20 436f 6d70 6172 696e  4. .... Comparin
-00001c30: 6720 5265 7375 6c74 732a 2a3a 2055 7365  g Results**: Use
-00001c40: 206f 6e6c 696e 6520 7461 626c 6573 2061   online tables a
-00001c50: 6e64 2070 6169 7265 6420 6368 6172 7473  nd paired charts
-00001c60: 2074 6f20 636f 6d70 6172 6520 7468 6520   to compare the 
-00001c70: 6879 7065 7270 6172 616d 6574 6572 7320  hyperparameters 
-00001c80: 616e 6420 6f75 7463 6f6d 6573 206f 6620  and outcomes of 
-00001c90: 6469 6666 6572 656e 740a 6578 7065 7269  different.experi
-00001ca0: 6d65 6e74 732c 2064 6576 656c 6f70 696e  ments, developin
-00001cb0: 6720 6974 6572 6174 6976 6520 696e 7370  g iterative insp
-00001cc0: 6972 6174 696f 6e2e 0a0a 2a2a 352e 20f0  iration...**5. .
-00001cd0: 9f91 a520 4f6e 6c69 6e65 2043 6f6c 6c61  ... Online Colla
-00001ce0: 626f 7261 7469 6f6e 2a2a 3a20 436f 6c6c  boration**: Coll
-00001cf0: 6162 6f72 6174 6520 7769 7468 2079 6f75  aborate with you
-00001d00: 7220 7465 616d 206f 6e20 7472 6169 6e69  r team on traini
-00001d10: 6e67 2070 726f 6a65 6374 732c 2073 7570  ng projects, sup
-00001d20: 706f 7274 696e 6720 7265 616c 2d74 696d  porting real-tim
-00001d30: 6520 7379 6e63 6872 6f6e 697a 6174 696f  e synchronizatio
-00001d40: 6e20 6f66 0a65 7870 6572 696d 656e 7473  n of.experiments
-00001d50: 2075 6e64 6572 2074 6865 2073 616d 6520   under the same 
-00001d60: 7072 6f6a 6563 742c 2061 6c6c 6f77 696e  project, allowin
-00001d70: 6720 796f 7520 746f 2073 796e 6368 726f  g you to synchro
-00001d80: 6e69 7a65 2074 7261 696e 696e 6720 7265  nize training re
-00001d90: 636f 7264 7320 6f66 2074 6865 2074 6561  cords of the tea
-00001da0: 6d20 6f6e 6c69 6e65 2061 6e64 2073 6861  m online and sha
-00001db0: 7265 2069 6e73 6967 6874 730a 616e 6420  re insights.and 
-00001dc0: 7375 6767 6573 7469 6f6e 7320 6261 7365  suggestions base
-00001dd0: 6420 6f6e 2072 6573 756c 7473 2e0a 0a2a  d on results...*
-00001de0: 2a36 2e20 e29c 89ef b88f 2053 6861 7269  *6. ...... Shari
-00001df0: 6e67 2052 6573 756c 7473 2a2a 3a20 436f  ng Results**: Co
-00001e00: 7079 2061 6e64 2073 656e 6420 7065 7273  py and send pers
-00001e10: 6973 7465 6e74 2055 524c 7320 746f 2073  istent URLs to s
-00001e20: 6861 7265 2065 6163 6820 6578 7065 7269  hare each experi
-00001e30: 6d65 6e74 2c20 6566 6669 6369 656e 746c  ment, efficientl
-00001e40: 7920 7365 6e64 2074 6865 6d20 746f 2063  y send them to c
-00001e50: 6f6c 6c65 6167 7565 732c 0a6f 7220 656d  olleagues,.or em
-00001e60: 6265 6420 7468 656d 2069 6e20 6f6e 6c69  bed them in onli
-00001e70: 6e65 206e 6f74 6573 2e0a 0a2a 2a37 2e20  ne notes...**7. 
-00001e80: f09f 92bb 2053 656c 662d 686f 7374 696e  .... Self-hostin
-00001e90: 6720 5375 7070 6f72 742a 2a3a 2053 7570  g Support**: Sup
-00001ea0: 706f 7274 7320 6f66 666c 696e 6520 6d6f  ports offline mo
-00001eb0: 6465 2077 6974 6820 6120 7365 6c66 2d68  de with a self-h
-00001ec0: 6f73 7465 6420 636f 6d6d 756e 6974 7920  osted community 
-00001ed0: 7665 7273 696f 6e20 7468 6174 2061 6c73  version that als
-00001ee0: 6f20 616c 6c6f 7773 2066 6f72 2064 6173  o allows for das
-00001ef0: 6862 6f61 7264 0a76 6965 7769 6e67 2061  hboard.viewing a
-00001f00: 6e64 2065 7870 6572 696d 656e 7420 6d61  nd experiment ma
-00001f10: 6e61 6765 6d65 6e74 2e0a 0a3e 205c 5b21  nagement...> \[!
-00001f20: 494d 504f 5254 414e 545d 0a3e 0a3e 202a  IMPORTANT].>.> *
-00001f30: 2a53 7461 7220 5573 2a2a 2c20 596f 7520  *Star Us**, You 
-00001f40: 7769 6c6c 2072 6563 6569 7665 2061 6c6c  will receive all
-00001f50: 2072 656c 6561 7365 206e 6f74 6966 6963   release notific
-00001f60: 6174 696f 6e73 2066 726f 6d20 4769 7448  ations from GitH
-00001f70: 7562 2077 6974 686f 7574 2061 6e79 2064  ub without any d
-00001f80: 656c 6179 207e 20e2 ad90 efb8 8f0a 0a0a  elay ~ .........
-00001f90: 0a21 5b73 7461 722d 7573 5d28 6874 7470  .![star-us](http
-00001fa0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00001fb0: 6572 636f 6e74 656e 742e 636f 6d2f 5377  ercontent.com/Sw
-00001fc0: 616e 4875 6258 2f73 7761 6e6c 6162 2f6d  anHubX/swanlab/m
-00001fd0: 6169 6e2f 7265 6164 6d65 5f66 696c 6573  ain/readme_files
-00001fe0: 2f73 7461 722d 7573 2e70 6e67 290a 0a3c  /star-us.png)..<
-00001ff0: 6272 3e0a 0a23 2320 f09f 8f81 2051 7569  br>..## .... Qui
-00002000: 636b 2053 7461 7274 0a0a 2323 2320 312e  ck Start..### 1.
-00002010: 496e 7374 616c 6c61 7469 6f6e 0a0a 6060  Installation..``
-00002020: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
-00002030: 6c20 7377 616e 6c61 620a 6060 600a 0a23  l swanlab.```..#
-00002040: 2323 2032 2e4c 6f67 2069 6e20 616e 6420  ## 2.Log in and 
-00002050: 6765 7420 7468 6520 4150 4920 4b65 790a  get the API Key.
-00002060: 0a31 2e20 2a2a 4672 6565 205b 5369 676e  .1. **Free [Sign
-00002070: 2055 705d 2868 7474 7073 3a2f 2f73 7761   Up](https://swa
-00002080: 6e6c 6162 2e63 6e29 2a2a 0a0a 322e 202a  nlab.cn)**..2. *
-00002090: 2a4c 6f67 2069 6e20 746f 2079 6f75 7220  *Log in to your 
-000020a0: 6163 636f 756e 742a 2a2c 2067 6f20 746f  account**, go to
-000020b0: 2055 7365 7220 5365 7474 696e 6773 203e   User Settings >
-000020c0: 205b 4150 4920 4b65 795d 2868 7474 7073   [API Key](https
-000020d0: 3a2f 2f73 7761 6e6c 6162 2e63 6e2f 7365  ://swanlab.cn/se
-000020e0: 7474 696e 6773 2920 616e 6420 636f 7079  ttings) and copy
-000020f0: 2079 6f75 7220 4150 4920 4b65 792e 0a0a   your API Key...
-00002100: 332e 202a 2a4f 7065 6e20 796f 7572 2074  3. **Open your t
-00002110: 6572 6d69 6e61 6c20 616e 6420 656e 7465  erminal and ente
-00002120: 722a 2a3a 0a0a 6060 6062 6173 680a 7377  r**:..```bash.sw
-00002130: 616e 6c61 6220 6c6f 6769 6e0a 6060 600a  anlab login.```.
-00002140: 0a57 6865 6e20 7072 6f6d 7074 6564 2c20  .When prompted, 
-00002150: 656e 7465 7220 796f 7572 2041 5049 204b  enter your API K
-00002160: 6579 2061 6e64 2070 7265 7373 2045 6e74  ey and press Ent
-00002170: 6572 2074 6f20 636f 6d70 6c65 7465 2074  er to complete t
-00002180: 6865 206c 6f67 696e 2e0a 0a23 2323 2033  he login...### 3
-00002190: 2e20 496e 7465 6772 6174 6520 5377 616e  . Integrate Swan
-000021a0: 4c61 6220 7769 7468 2059 6f75 7220 436f  Lab with Your Co
-000021b0: 6465 0a0a 6060 6070 7974 686f 6e0a 696d  de..```python.im
-000021c0: 706f 7274 2073 7761 6e6c 6162 0a0a 2320  port swanlab..# 
-000021d0: 4372 6561 7465 2061 206e 6577 2053 7761  Create a new Swa
-000021e0: 6e4c 6162 2065 7870 6572 696d 656e 740a  nLab experiment.
-000021f0: 7377 616e 6c61 622e 696e 6974 280a 2020  swanlab.init(.  
-00002200: 2020 7072 6f6a 6563 743d 226d 792d 6669    project="my-fi
-00002210: 7273 742d 6d6c 222c 0a20 2020 2063 6f6e  rst-ml",.    con
-00002220: 6669 673d 7b27 6c65 6172 6e69 6e67 2d72  fig={'learning-r
-00002230: 6174 6527 3a20 302e 3030 337d 0a29 0a0a  ate': 0.003}.)..
-00002240: 2320 4c6f 6720 6d65 7472 6963 730a 666f  # Log metrics.fo
-00002250: 7220 6920 696e 2072 616e 6765 2831 3029  r i in range(10)
-00002260: 3a0a 2020 2020 7377 616e 6c61 622e 6c6f  :.    swanlab.lo
-00002270: 6728 7b22 6c6f 7373 223a 2069 7d29 0a60  g({"loss": i}).`
-00002280: 6060 0a0a 2a2a 416c 6c20 7365 7421 2a2a  ``..**All set!**
-00002290: 2056 6973 6974 205b 5377 616e 4c61 625d   Visit [SwanLab]
-000022a0: 2868 7474 7073 3a2f 2f73 7761 6e6c 6162  (https://swanlab
-000022b0: 2e63 6e29 2074 6f20 7365 6520 796f 7572  .cn) to see your
-000022c0: 2066 6972 7374 2053 7761 6e4c 6162 2065   first SwanLab e
-000022d0: 7870 6572 696d 656e 742e 0a0a 215b 4d4e  xperiment...![MN
-000022e0: 4953 545d 2868 7474 7073 3a2f 2f72 6177  IST](https://raw
-000022f0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00002300: 6e74 2e63 6f6d 2f53 7761 6e48 7562 582f  nt.com/SwanHubX/
-00002310: 7377 616e 6c61 622f 6d61 696e 2f72 6561  swanlab/main/rea
-00002320: 646d 655f 6669 6c65 732f 7265 6164 6d65  dme_files/readme
-00002330: 2d6d 6e69 7374 2e70 6e67 290a 0a3c 6272  -mnist.png)..<br
-00002340: 3e0a 0a23 2320 f09f 9383 204d 6f72 6520  >..## .... More 
-00002350: 4578 616d 706c 6573 0a0a 3c64 6574 6169  Examples..<detai
-00002360: 6c73 3e0a 3c73 756d 6d61 7279 3e4d 4e49  ls>.<summary>MNI
-00002370: 5354 3c2f 7375 6d6d 6172 793e 0a0a 6060  ST</summary>..``
-00002380: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
-00002390: 730a 696d 706f 7274 2074 6f72 6368 0a66  s.import torch.f
-000023a0: 726f 6d20 746f 7263 6820 696d 706f 7274  rom torch import
-000023b0: 206e 6e2c 206f 7074 696d 2c20 7574 696c   nn, optim, util
-000023c0: 730a 696d 706f 7274 2074 6f72 6368 2e6e  s.import torch.n
-000023d0: 6e2e 6675 6e63 7469 6f6e 616c 2061 7320  n.functional as 
-000023e0: 460a 6672 6f6d 2074 6f72 6368 7669 7369  F.from torchvisi
-000023f0: 6f6e 2e64 6174 6173 6574 7320 696d 706f  on.datasets impo
-00002400: 7274 204d 4e49 5354 0a66 726f 6d20 746f  rt MNIST.from to
-00002410: 7263 6876 6973 696f 6e2e 7472 616e 7366  rchvision.transf
-00002420: 6f72 6d73 2069 6d70 6f72 7420 546f 5465  orms import ToTe
-00002430: 6e73 6f72 0a69 6d70 6f72 7420 7377 616e  nsor.import swan
-00002440: 6c61 620a 0a0a 2320 434e 4ee7 bd91 e7bb  lab...# CNN.....
-00002450: 9ce6 9e84 e5bb ba0a 636c 6173 7320 436f  ........class Co
-00002460: 6e76 4e65 7428 6e6e 2e4d 6f64 756c 6529  nvNet(nn.Module)
-00002470: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00002480: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00002490: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-000024a0: 5f5f 2829 0a20 2020 2020 2020 2023 2031  __().        # 1
-000024b0: 2c32 3878 3238 0a20 2020 2020 2020 2073  ,28x28.        s
-000024c0: 656c 662e 636f 6e76 3120 3d20 6e6e 2e43  elf.conv1 = nn.C
-000024d0: 6f6e 7632 6428 312c 2031 302c 2035 2920  onv2d(1, 10, 5) 
-000024e0: 2023 2031 302c 2032 3478 3234 0a20 2020   # 10, 24x24.   
-000024f0: 2020 2020 2073 656c 662e 636f 6e76 3220       self.conv2 
-00002500: 3d20 6e6e 2e43 6f6e 7632 6428 3130 2c20  = nn.Conv2d(10, 
-00002510: 3230 2c20 3329 2020 2320 3132 382c 2031  20, 3)  # 128, 1
-00002520: 3078 3130 0a20 2020 2020 2020 2073 656c  0x10.        sel
-00002530: 662e 6663 3120 3d20 6e6e 2e4c 696e 6561  f.fc1 = nn.Linea
-00002540: 7228 3230 202a 2031 3020 2a20 3130 2c20  r(20 * 10 * 10, 
-00002550: 3530 3029 0a20 2020 2020 2020 2073 656c  500).        sel
-00002560: 662e 6663 3220 3d20 6e6e 2e4c 696e 6561  f.fc2 = nn.Linea
-00002570: 7228 3530 302c 2031 3029 0a0a 2020 2020  r(500, 10)..    
-00002580: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
-00002590: 2c20 7829 3a0a 2020 2020 2020 2020 696e  , x):.        in
-000025a0: 5f73 697a 6520 3d20 782e 7369 7a65 2830  _size = x.size(0
-000025b0: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
-000025c0: 7365 6c66 2e63 6f6e 7631 2878 2920 2023  self.conv1(x)  #
-000025d0: 2032 340a 2020 2020 2020 2020 6f75 7420   24.        out 
-000025e0: 3d20 462e 7265 6c75 286f 7574 290a 2020  = F.relu(out).  
-000025f0: 2020 2020 2020 6f75 7420 3d20 462e 6d61        out = F.ma
-00002600: 785f 706f 6f6c 3264 286f 7574 2c20 322c  x_pool2d(out, 2,
-00002610: 2032 2920 2023 2031 320a 2020 2020 2020   2)  # 12.      
-00002620: 2020 6f75 7420 3d20 7365 6c66 2e63 6f6e    out = self.con
-00002630: 7632 286f 7574 2920 2023 2031 300a 2020  v2(out)  # 10.  
-00002640: 2020 2020 2020 6f75 7420 3d20 462e 7265        out = F.re
-00002650: 6c75 286f 7574 290a 2020 2020 2020 2020  lu(out).        
-00002660: 6f75 7420 3d20 6f75 742e 7669 6577 2869  out = out.view(i
-00002670: 6e5f 7369 7a65 2c20 2d31 290a 2020 2020  n_size, -1).    
-00002680: 2020 2020 6f75 7420 3d20 7365 6c66 2e66      out = self.f
-00002690: 6331 286f 7574 290a 2020 2020 2020 2020  c1(out).        
-000026a0: 6f75 7420 3d20 462e 7265 6c75 286f 7574  out = F.relu(out
-000026b0: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
-000026c0: 7365 6c66 2e66 6332 286f 7574 290a 2020  self.fc2(out).  
-000026d0: 2020 2020 2020 6f75 7420 3d20 462e 6c6f        out = F.lo
-000026e0: 675f 736f 6674 6d61 7828 6f75 742c 2064  g_softmax(out, d
-000026f0: 696d 3d31 290a 2020 2020 2020 2020 7265  im=1).        re
-00002700: 7475 726e 206f 7574 0a0a 0a23 20e6 8d95  turn out...# ...
-00002710: e88e b7e5 b9b6 e58f afe8 a786 e58c 96e5  ................
-00002720: 898d 3230 e5bc a0e5 9bbe e583 8f0a 6465  ..20..........de
-00002730: 6620 6c6f 675f 696d 6167 6573 286c 6f61  f log_images(loa
-00002740: 6465 722c 206e 756d 5f69 6d61 6765 733d  der, num_images=
-00002750: 3136 293a 0a20 2020 2069 6d61 6765 735f  16):.    images_
-00002760: 6c6f 6767 6564 203d 2030 0a20 2020 206c  logged = 0.    l
-00002770: 6f67 6765 645f 696d 6167 6573 203d 205b  ogged_images = [
-00002780: 5d0a 2020 2020 666f 7220 696d 6167 6573  ].    for images
-00002790: 2c20 6c61 6265 6c73 2069 6e20 6c6f 6164  , labels in load
-000027a0: 6572 3a0a 2020 2020 2020 2020 2320 696d  er:.        # im
-000027b0: 6167 6573 3a20 6261 7463 6820 6f66 2069  ages: batch of i
-000027c0: 6d61 6765 732c 206c 6162 656c 733a 2062  mages, labels: b
-000027d0: 6174 6368 206f 6620 6c61 6265 6c73 0a20  atch of labels. 
-000027e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000027f0: 7261 6e67 6528 696d 6167 6573 2e73 6861  range(images.sha
-00002800: 7065 5b30 5d29 3a0a 2020 2020 2020 2020  pe[0]):.        
-00002810: 2020 2020 6966 2069 6d61 6765 735f 6c6f      if images_lo
-00002820: 6767 6564 203c 206e 756d 5f69 6d61 6765  gged < num_image
-00002830: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00002840: 2020 2023 20e4 bdbf e794 a873 7761 6e6c     # ......swanl
-00002850: 6162 2e49 6d61 6765 e5b0 86e5 9bbe e583  ab.Image........
-00002860: 8fe8 bdac e68d a2e4 b8ba 7761 6e64 62e5  ..........wandb.
-00002870: 8faf e8a7 86e5 8c96 e6a0 bce5 bc8f 0a20  ............... 
-00002880: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002890: 6f67 6765 645f 696d 6167 6573 2e61 7070  ogged_images.app
-000028a0: 656e 6428 7377 616e 6c61 622e 496d 6167  end(swanlab.Imag
-000028b0: 6528 696d 6167 6573 5b69 5d2c 2063 6170  e(images[i], cap
-000028c0: 7469 6f6e 3d66 224c 6162 656c 3a20 7b6c  tion=f"Label: {l
-000028d0: 6162 656c 735b 695d 7d22 2929 0a20 2020  abels[i]}")).   
-000028e0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-000028f0: 6765 735f 6c6f 6767 6564 202b 3d20 310a  ges_logged += 1.
-00002900: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00002910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002920: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00002930: 6966 2069 6d61 6765 735f 6c6f 6767 6564  if images_logged
-00002940: 203e 3d20 6e75 6d5f 696d 6167 6573 3a0a   >= num_images:.
-00002950: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00002960: 6b0a 2020 2020 7377 616e 6c61 622e 6c6f  k.    swanlab.lo
-00002970: 6728 7b22 4d4e 4953 542d 5072 6576 6965  g({"MNIST-Previe
-00002980: 7722 3a20 6c6f 6767 6564 5f69 6d61 6765  w": logged_image
-00002990: 737d 290a 0a0a 6966 205f 5f6e 616d 655f  s})...if __name_
-000029a0: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
-000029b0: 0a0a 2020 2020 2320 e588 9de5 a78b e58c  ..    # ........
-000029c0: 9673 7761 6e6c 6162 0a20 2020 2072 756e  .swanlab.    run
-000029d0: 203d 2073 7761 6e6c 6162 2e69 6e69 7428   = swanlab.init(
-000029e0: 0a20 2020 2020 2020 2070 726f 6a65 6374  .        project
-000029f0: 3d22 4d4e 4953 542d 6578 616d 706c 6522  ="MNIST-example"
-00002a00: 2c0a 2020 2020 2020 2020 6578 7065 7269  ,.        experi
-00002a10: 6d65 6e74 5f6e 616d 653d 2243 6f6e 764e  ment_name="ConvN
-00002a20: 6574 222c 0a20 2020 2020 2020 2064 6573  et",.        des
-00002a30: 6372 6970 7469 6f6e 3d22 5472 6169 6e20  cription="Train 
-00002a40: 436f 6e76 4e65 7420 6f6e 204d 4e49 5354  ConvNet on MNIST
-00002a50: 2064 6174 6173 6574 2e22 2c0a 2020 2020   dataset.",.    
-00002a60: 2020 2020 636f 6e66 6967 3d7b 0a20 2020      config={.   
-00002a70: 2020 2020 2020 2020 2022 6d6f 6465 6c22           "model"
-00002a80: 3a20 2243 4e4e 222c 0a20 2020 2020 2020  : "CNN",.       
-00002a90: 2020 2020 2022 6f70 7469 6d22 3a20 2241       "optim": "A
-00002aa0: 6461 6d22 2c0a 2020 2020 2020 2020 2020  dam",.          
-00002ab0: 2020 226c 7222 3a20 302e 3030 312c 0a20    "lr": 0.001,. 
-00002ac0: 2020 2020 2020 2020 2020 2022 6261 7463             "batc
-00002ad0: 685f 7369 7a65 223a 2035 3132 2c0a 2020  h_size": 512,.  
-00002ae0: 2020 2020 2020 2020 2020 226e 756d 5f65            "num_e
-00002af0: 706f 6368 7322 3a20 3130 2c0a 2020 2020  pochs": 10,.    
-00002b00: 2020 2020 2020 2020 2274 7261 696e 5f64          "train_d
-00002b10: 6174 6173 6574 5f6e 756d 223a 2035 3530  ataset_num": 550
-00002b20: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-00002b30: 2276 616c 5f64 6174 6173 6574 5f6e 756d  "val_dataset_num
-00002b40: 223a 2035 3030 302c 0a20 2020 2020 2020  ": 5000,.       
-00002b50: 207d 2c0a 2020 2020 290a 0a20 2020 2023   },.    )..    #
-00002b60: 20e8 aebe e7bd aee8 aead e7bb 83e6 9cba   ...............
-00002b70: e380 81e9 aa8c e8af 81e9 9b86 e592 8ce6  ................
-00002b80: b58b e8af 95e9 9b86 0a20 2020 2064 6174  .........    dat
-00002b90: 6173 6574 203d 204d 4e49 5354 286f 732e  aset = MNIST(os.
-00002ba0: 6765 7463 7764 2829 2c20 7472 6169 6e3d  getcwd(), train=
-00002bb0: 5472 7565 2c20 646f 776e 6c6f 6164 3d54  True, download=T
-00002bc0: 7275 652c 2074 7261 6e73 666f 726d 3d54  rue, transform=T
-00002bd0: 6f54 656e 736f 7228 2929 0a20 2020 2074  oTensor()).    t
-00002be0: 7261 696e 5f64 6174 6173 6574 2c20 7661  rain_dataset, va
-00002bf0: 6c5f 6461 7461 7365 7420 3d20 7574 696c  l_dataset = util
-00002c00: 732e 6461 7461 2e72 616e 646f 6d5f 7370  s.data.random_sp
-00002c10: 6c69 7428 0a20 2020 2020 2020 2064 6174  lit(.        dat
-00002c20: 6173 6574 2c20 5b72 756e 2e63 6f6e 6669  aset, [run.confi
-00002c30: 672e 7472 6169 6e5f 6461 7461 7365 745f  g.train_dataset_
-00002c40: 6e75 6d2c 2072 756e 2e63 6f6e 6669 672e  num, run.config.
-00002c50: 7661 6c5f 6461 7461 7365 745f 6e75 6d5d  val_dataset_num]
-00002c60: 0a20 2020 2029 0a0a 2020 2020 7472 6169  .    )..    trai
-00002c70: 6e5f 6c6f 6164 6572 203d 2075 7469 6c73  n_loader = utils
-00002c80: 2e64 6174 612e 4461 7461 4c6f 6164 6572  .data.DataLoader
-00002c90: 2874 7261 696e 5f64 6174 6173 6574 2c20  (train_dataset, 
-00002ca0: 6261 7463 685f 7369 7a65 3d72 756e 2e63  batch_size=run.c
-00002cb0: 6f6e 6669 672e 6261 7463 685f 7369 7a65  onfig.batch_size
-00002cc0: 2c20 7368 7566 666c 653d 5472 7565 290a  , shuffle=True).
-00002cd0: 2020 2020 7661 6c5f 6c6f 6164 6572 203d      val_loader =
-00002ce0: 2075 7469 6c73 2e64 6174 612e 4461 7461   utils.data.Data
-00002cf0: 4c6f 6164 6572 2876 616c 5f64 6174 6173  Loader(val_datas
-00002d00: 6574 2c20 6261 7463 685f 7369 7a65 3d31  et, batch_size=1
-00002d10: 2c20 7368 7566 666c 653d 4661 6c73 6529  , shuffle=False)
-00002d20: 0a0a 2020 2020 2320 e588 9de5 a78b e58c  ..    # ........
-00002d30: 96e6 a8a1 e59e 8be3 8081 e68d 9fe5 a4b1  ................
-00002d40: e587 bde6 95b0 e592 8ce4 bc98 e58c 96e5  ................
-00002d50: 99a8 0a20 2020 206d 6f64 656c 203d 2043  ...    model = C
-00002d60: 6f6e 764e 6574 2829 0a20 2020 2063 7269  onvNet().    cri
-00002d70: 7465 7269 6f6e 203d 206e 6e2e 4372 6f73  terion = nn.Cros
-00002d80: 7345 6e74 726f 7079 4c6f 7373 2829 0a20  sEntropyLoss(). 
-00002d90: 2020 206f 7074 696d 697a 6572 203d 206f     optimizer = o
-00002da0: 7074 696d 2e41 6461 6d28 6d6f 6465 6c2e  ptim.Adam(model.
-00002db0: 7061 7261 6d65 7465 7273 2829 2c20 6c72  parameters(), lr
-00002dc0: 3d72 756e 2e63 6f6e 6669 672e 6c72 290a  =run.config.lr).
-00002dd0: 0a20 2020 2023 20ef bc88 e58f afe9 8089  .    # .........
-00002de0: efbc 89e7 9c8b e4b8 80e4 b88b e695 b0e6  ................
-00002df0: 8dae e99b 86e7 9a84 e589 8d31 36e5 bca0  ...........16...
-00002e00: e59b bee5 838f 0a20 2020 206c 6f67 5f69  .......    log_i
-00002e10: 6d61 6765 7328 7472 6169 6e5f 6c6f 6164  mages(train_load
-00002e20: 6572 2c20 3136 290a 0a20 2020 2023 20e5  er, 16)..    # .
-00002e30: bc80 e5a7 8be8 aead e7bb 830a 2020 2020  ............    
-00002e40: 666f 7220 6570 6f63 6820 696e 2072 616e  for epoch in ran
-00002e50: 6765 2831 2c20 7275 6e2e 636f 6e66 6967  ge(1, run.config
-00002e60: 2e6e 756d 5f65 706f 6368 7329 3a0a 2020  .num_epochs):.  
-00002e70: 2020 2020 2020 7377 616e 6c61 622e 6c6f        swanlab.lo
-00002e80: 6728 7b22 7472 6169 6e2f 6570 6f63 6822  g({"train/epoch"
-00002e90: 3a20 6570 6f63 687d 290a 2020 2020 2020  : epoch}).      
-00002ea0: 2020 2320 e8ae ade7 bb83 e5be aae7 8eaf    # ............
-00002eb0: 0a20 2020 2020 2020 2066 6f72 2069 7465  .        for ite
-00002ec0: 722c 2062 6174 6368 2069 6e20 656e 756d  r, batch in enum
-00002ed0: 6572 6174 6528 7472 6169 6e5f 6c6f 6164  erate(train_load
-00002ee0: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
-00002ef0: 2078 2c20 7920 3d20 6261 7463 680a 2020   x, y = batch.  
-00002f00: 2020 2020 2020 2020 2020 6f70 7469 6d69            optimi
-00002f10: 7a65 722e 7a65 726f 5f67 7261 6428 290a  zer.zero_grad().
-00002f20: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00002f30: 7574 203d 206d 6f64 656c 2878 290a 2020  ut = model(x).  
-00002f40: 2020 2020 2020 2020 2020 6c6f 7373 203d            loss =
-00002f50: 2063 7269 7465 7269 6f6e 286f 7574 7075   criterion(outpu
-00002f60: 742c 2079 290a 2020 2020 2020 2020 2020  t, y).          
-00002f70: 2020 6c6f 7373 2e62 6163 6b77 6172 6428    loss.backward(
-00002f80: 290a 2020 2020 2020 2020 2020 2020 6f70  ).            op
-00002f90: 7469 6d69 7a65 722e 7374 6570 2829 0a0a  timizer.step()..
-00002fa0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002fb0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00002fc0: 2020 2066 2245 706f 6368 205b 7b65 706f     f"Epoch [{epo
-00002fd0: 6368 7d2f 7b72 756e 2e63 6f6e 6669 672e  ch}/{run.config.
-00002fe0: 6e75 6d5f 6570 6f63 6873 7d5d 2c20 4974  num_epochs}], It
-00002ff0: 6572 6174 696f 6e20 5b7b 6974 6572 202b  eration [{iter +
-00003000: 2031 7d2f 7b6c 656e 2874 7261 696e 5f6c   1}/{len(train_l
-00003010: 6f61 6465 7229 7d5d 2c20 4c6f 7373 3a20  oader)}], Loss: 
-00003020: 7b6c 6f73 732e 6974 656d 2829 7d22 0a20  {loss.item()}". 
-00003030: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00003040: 2020 2020 2020 2020 2020 6966 2069 7465            if ite
-00003050: 7220 2520 3230 203d 3d20 303a 0a20 2020  r % 20 == 0:.   
-00003060: 2020 2020 2020 2020 2020 2020 2073 7761               swa
-00003070: 6e6c 6162 2e6c 6f67 287b 2274 7261 696e  nlab.log({"train
-00003080: 2f6c 6f73 7322 3a20 6c6f 7373 2e69 7465  /loss": loss.ite
-00003090: 6d28 297d 2c20 7374 6570 3d28 6570 6f63  m()}, step=(epoc
-000030a0: 6820 2d20 3129 202a 206c 656e 2874 7261  h - 1) * len(tra
-000030b0: 696e 5f6c 6f61 6465 7229 202b 2069 7465  in_loader) + ite
-000030c0: 7229 0a0a 2020 2020 2020 2020 2320 e6af  r)..        # ..
-000030d0: 8f34 e4b8 aa65 706f 6368 e9aa 8ce8 af81  .4...epoch......
-000030e0: e4b8 80e6 aca1 0a20 2020 2020 2020 2069  .......        i
-000030f0: 6620 6570 6f63 6820 2520 3220 3d3d 2030  f epoch % 2 == 0
-00003100: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-00003110: 6465 6c2e 6576 616c 2829 0a20 2020 2020  del.eval().     
-00003120: 2020 2020 2020 2063 6f72 7265 6374 203d         correct =
-00003130: 2030 0a20 2020 2020 2020 2020 2020 2074   0.            t
-00003140: 6f74 616c 203d 2030 0a20 2020 2020 2020  otal = 0.       
-00003150: 2020 2020 2077 6974 6820 746f 7263 682e       with torch.
-00003160: 6e6f 5f67 7261 6428 293a 0a20 2020 2020  no_grad():.     
-00003170: 2020 2020 2020 2020 2020 2066 6f72 2062             for b
-00003180: 6174 6368 2069 6e20 7661 6c5f 6c6f 6164  atch in val_load
-00003190: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-000031a0: 2020 2020 2020 2020 782c 2079 203d 2062          x, y = b
-000031b0: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
-000031c0: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-000031d0: 3d20 6d6f 6465 6c28 7829 0a20 2020 2020  = model(x).     
-000031e0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-000031f0: 2c20 7072 6564 6963 7465 6420 3d20 746f  , predicted = to
-00003200: 7263 682e 6d61 7828 6f75 7470 7574 2c20  rch.max(output, 
-00003210: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00003220: 2020 2020 2020 2074 6f74 616c 202b 3d20         total += 
-00003230: 792e 7369 7a65 2830 290a 2020 2020 2020  y.size(0).      
-00003240: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00003250: 7272 6563 7420 2b3d 2028 7072 6564 6963  rrect += (predic
-00003260: 7465 6420 3d3d 2079 292e 7375 6d28 292e  ted == y).sum().
-00003270: 6974 656d 2829 0a0a 2020 2020 2020 2020  item()..        
-00003280: 2020 2020 6163 6375 7261 6379 203d 2063      accuracy = c
-00003290: 6f72 7265 6374 202f 2074 6f74 616c 0a20  orrect / total. 
-000032a0: 2020 2020 2020 2020 2020 2073 7761 6e6c             swanl
-000032b0: 6162 2e6c 6f67 287b 2276 616c 2f61 6363  ab.log({"val/acc
-000032c0: 7572 6163 7922 3a20 6163 6375 7261 6379  uracy": accuracy
-000032d0: 7d29 0a60 6060 0a0a 3c2f 6465 7461 696c  }).```..</detail
-000032e0: 733e 0a0a 3c64 6574 6169 6c73 3e0a 3c73  s>..<details>.<s
-000032f0: 756d 6d61 7279 3e46 6173 6869 6f6e 4d4e  ummary>FashionMN
-00003300: 5349 543c 2f73 756d 6d61 7279 3e0a 0a60  SIT</summary>..`
-00003310: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00003320: 6f73 0a69 6d70 6f72 7420 746f 7263 680a  os.import torch.
-00003330: 6672 6f6d 2074 6f72 6368 2069 6d70 6f72  from torch impor
-00003340: 7420 6e6e 2c20 6f70 7469 6d2c 2075 7469  t nn, optim, uti
-00003350: 6c73 0a69 6d70 6f72 7420 746f 7263 682e  ls.import torch.
-00003360: 6e6e 2e66 756e 6374 696f 6e61 6c20 6173  nn.functional as
-00003370: 2046 0a66 726f 6d20 746f 7263 6876 6973   F.from torchvis
-00003380: 696f 6e2e 6461 7461 7365 7473 2069 6d70  ion.datasets imp
-00003390: 6f72 7420 4661 7368 696f 6e4d 4e49 5354  ort FashionMNIST
-000033a0: 0a66 726f 6d20 746f 7263 6876 6973 696f  .from torchvisio
-000033b0: 6e2e 7472 616e 7366 6f72 6d73 2069 6d70  n.transforms imp
-000033c0: 6f72 7420 546f 5465 6e73 6f72 0a69 6d70  ort ToTensor.imp
-000033d0: 6f72 7420 7377 616e 6c61 620a 0a0a 2320  ort swanlab...# 
-000033e0: 5265 734e 6574 e7bd 91e7 bb9c e69e 84e5  ResNet..........
-000033f0: bbba 0a63 6c61 7373 2042 6173 6963 626c  ...class Basicbl
-00003400: 6f63 6b28 6e6e 2e4d 6f64 756c 6529 3a0a  ock(nn.Module):.
-00003410: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00003420: 2873 656c 662c 2069 6e5f 706c 616e 6573  (self, in_planes
-00003430: 2c20 706c 616e 6573 2c20 7374 7269 6465  , planes, stride
-00003440: 3d31 293a 0a20 2020 2020 2020 2073 7570  =1):.        sup
-00003450: 6572 2842 6173 6963 626c 6f63 6b2c 2073  er(Basicblock, s
-00003460: 656c 6629 2e5f 5f69 6e69 745f 5f28 290a  elf).__init__().
-00003470: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00003480: 7631 203d 206e 6e2e 5365 7175 656e 7469  v1 = nn.Sequenti
-00003490: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-000034a0: 6e6e 2e43 6f6e 7632 6428 696e 5f63 6861  nn.Conv2d(in_cha
-000034b0: 6e6e 656c 733d 696e 5f70 6c61 6e65 732c  nnels=in_planes,
-000034c0: 206f 7574 5f63 6861 6e6e 656c 733d 706c   out_channels=pl
-000034d0: 616e 6573 2c20 6b65 726e 656c 5f73 697a  anes, kernel_siz
-000034e0: 653d 332c 2073 7472 6964 653d 7374 7269  e=3, stride=stri
-000034f0: 6465 2c20 7061 6464 696e 673d 312c 2062  de, padding=1, b
-00003500: 6961 733d 4661 6c73 6529 2c0a 2020 2020  ias=False),.    
-00003510: 2020 2020 2020 2020 6e6e 2e42 6174 6368          nn.Batch
-00003520: 4e6f 726d 3264 2870 6c61 6e65 7329 2c0a  Norm2d(planes),.
-00003530: 2020 2020 2020 2020 2020 2020 6e6e 2e52              nn.R
-00003540: 654c 5528 290a 2020 2020 2020 2020 290a  eLU().        ).
-00003550: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00003560: 7632 203d 206e 6e2e 5365 7175 656e 7469  v2 = nn.Sequenti
-00003570: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00003580: 6e6e 2e43 6f6e 7632 6428 696e 5f63 6861  nn.Conv2d(in_cha
-00003590: 6e6e 656c 733d 706c 616e 6573 2c20 6f75  nnels=planes, ou
-000035a0: 745f 6368 616e 6e65 6c73 3d70 6c61 6e65  t_channels=plane
-000035b0: 732c 206b 6572 6e65 6c5f 7369 7a65 3d33  s, kernel_size=3
-000035c0: 2c20 7374 7269 6465 3d31 2c20 7061 6464  , stride=1, padd
-000035d0: 696e 673d 312c 2062 6961 733d 4661 6c73  ing=1, bias=Fals
-000035e0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-000035f0: 6e6e 2e42 6174 6368 4e6f 726d 3264 2870  nn.BatchNorm2d(p
-00003600: 6c61 6e65 7329 2c0a 2020 2020 2020 2020  lanes),.        
-00003610: 290a 0a20 2020 2020 2020 2069 6620 7374  )..        if st
-00003620: 7269 6465 2021 3d20 3120 6f72 2069 6e5f  ride != 1 or in_
-00003630: 706c 616e 6573 2021 3d20 706c 616e 6573  planes != planes
-00003640: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00003650: 6c66 2e73 686f 7274 6375 7420 3d20 6e6e  lf.shortcut = nn
-00003660: 2e53 6571 7565 6e74 6961 6c28 0a20 2020  .Sequential(.   
-00003670: 2020 2020 2020 2020 2020 2020 206e 6e2e               nn.
-00003680: 436f 6e76 3264 2869 6e5f 6368 616e 6e65  Conv2d(in_channe
-00003690: 6c73 3d69 6e5f 706c 616e 6573 2c20 6f75  ls=in_planes, ou
-000036a0: 745f 6368 616e 6e65 6c73 3d70 6c61 6e65  t_channels=plane
-000036b0: 732c 206b 6572 6e65 6c5f 7369 7a65 3d33  s, kernel_size=3
-000036c0: 2c20 7374 7269 6465 3d73 7472 6964 652c  , stride=stride,
-000036d0: 2070 6164 6469 6e67 3d31 292c 0a20 2020   padding=1),.   
-000036e0: 2020 2020 2020 2020 2020 2020 206e 6e2e               nn.
-000036f0: 4261 7463 684e 6f72 6d32 6428 706c 616e  BatchNorm2d(plan
-00003700: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
-00003710: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00003720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003730: 2e73 686f 7274 6375 7420 3d20 6e6e 2e53  .shortcut = nn.S
-00003740: 6571 7565 6e74 6961 6c28 290a 0a20 2020  equential()..   
-00003750: 2064 6566 2066 6f72 7761 7264 2873 656c   def forward(sel
-00003760: 662c 2078 293a 0a20 2020 2020 2020 206f  f, x):.        o
-00003770: 7574 203d 2073 656c 662e 636f 6e76 3128  ut = self.conv1(
-00003780: 7829 0a20 2020 2020 2020 206f 7574 203d  x).        out =
-00003790: 2073 656c 662e 636f 6e76 3228 6f75 7429   self.conv2(out)
-000037a0: 0a20 2020 2020 2020 206f 7574 202b 3d20  .        out += 
-000037b0: 7365 6c66 2e73 686f 7274 6375 7428 7829  self.shortcut(x)
-000037c0: 0a20 2020 2020 2020 206f 7574 203d 2046  .        out = F
-000037d0: 2e72 656c 7528 6f75 7429 0a20 2020 2020  .relu(out).     
-000037e0: 2020 2072 6574 7572 6e20 6f75 740a 0a0a     return out...
-000037f0: 636c 6173 7320 5265 734e 6574 286e 6e2e  class ResNet(nn.
-00003800: 4d6f 6475 6c65 293a 0a20 2020 2064 6566  Module):.    def
-00003810: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00003820: 626c 6f63 6b2c 206e 756d 5f62 6c6f 636b  block, num_block
-00003830: 2c20 6e75 6d5f 636c 6173 7365 7329 3a0a  , num_classes):.
-00003840: 2020 2020 2020 2020 7375 7065 7228 5265          super(Re
-00003850: 734e 6574 2c20 7365 6c66 292e 5f5f 696e  sNet, self).__in
-00003860: 6974 5f5f 2829 0a20 2020 2020 2020 2073  it__().        s
-00003870: 656c 662e 696e 5f70 6c61 6e65 7320 3d20  elf.in_planes = 
-00003880: 3136 0a20 2020 2020 2020 2073 656c 662e  16.        self.
-00003890: 636f 6e76 3120 3d20 6e6e 2e53 6571 7565  conv1 = nn.Seque
-000038a0: 6e74 6961 6c28 0a20 2020 2020 2020 2020  ntial(.         
-000038b0: 2020 206e 6e2e 436f 6e76 3264 2869 6e5f     nn.Conv2d(in_
-000038c0: 6368 616e 6e65 6c73 3d31 2c20 6f75 745f  channels=1, out_
-000038d0: 6368 616e 6e65 6c73 3d31 362c 206b 6572  channels=16, ker
-000038e0: 6e65 6c5f 7369 7a65 3d33 2c20 7374 7269  nel_size=3, stri
-000038f0: 6465 3d31 2c20 7061 6464 696e 673d 3129  de=1, padding=1)
-00003900: 2c0a 2020 2020 2020 2020 2020 2020 6e6e  ,.            nn
-00003910: 2e42 6174 6368 4e6f 726d 3264 2831 3629  .BatchNorm2d(16)
-00003920: 2c0a 2020 2020 2020 2020 2020 2020 6e6e  ,.            nn
-00003930: 2e52 654c 5528 290a 2020 2020 2020 2020  .ReLU().        
-00003940: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-00003950: 6178 706f 6f6c 203d 206e 6e2e 4d61 7850  axpool = nn.MaxP
-00003960: 6f6f 6c32 6428 6b65 726e 656c 5f73 697a  ool2d(kernel_siz
-00003970: 653d 332c 2073 7472 6964 653d 312c 2070  e=3, stride=1, p
-00003980: 6164 6469 6e67 3d31 290a 0a20 2020 2020  adding=1)..     
-00003990: 2020 2073 656c 662e 626c 6f63 6b31 203d     self.block1 =
-000039a0: 2073 656c 662e 5f6d 616b 655f 6c61 7965   self._make_laye
-000039b0: 7228 626c 6f63 6b2c 2031 362c 206e 756d  r(block, 16, num
-000039c0: 5f62 6c6f 636b 5b30 5d2c 2073 7472 6964  _block[0], strid
-000039d0: 653d 3129 0a20 2020 2020 2020 2073 656c  e=1).        sel
-000039e0: 662e 626c 6f63 6b32 203d 2073 656c 662e  f.block2 = self.
-000039f0: 5f6d 616b 655f 6c61 7965 7228 626c 6f63  _make_layer(bloc
-00003a00: 6b2c 2033 322c 206e 756d 5f62 6c6f 636b  k, 32, num_block
-00003a10: 5b31 5d2c 2073 7472 6964 653d 3229 0a20  [1], stride=2). 
-00003a20: 2020 2020 2020 2073 656c 662e 626c 6f63         self.bloc
-00003a30: 6b33 203d 2073 656c 662e 5f6d 616b 655f  k3 = self._make_
-00003a40: 6c61 7965 7228 626c 6f63 6b2c 2036 342c  layer(block, 64,
-00003a50: 206e 756d 5f62 6c6f 636b 5b32 5d2c 2073   num_block[2], s
-00003a60: 7472 6964 653d 3229 0a20 2020 2020 2020  tride=2).       
-00003a70: 2023 2073 656c 662e 626c 6f63 6b34 203d   # self.block4 =
-00003a80: 2073 656c 662e 5f6d 616b 655f 6c61 7965   self._make_laye
-00003a90: 7228 626c 6f63 6b2c 2035 3132 2c20 6e75  r(block, 512, nu
-00003aa0: 6d5f 626c 6f63 6b5b 335d 2c20 7374 7269  m_block[3], stri
-00003ab0: 6465 3d32 290a 0a20 2020 2020 2020 2073  de=2)..        s
-00003ac0: 656c 662e 6f75 746c 6179 6572 203d 206e  elf.outlayer = n
-00003ad0: 6e2e 4c69 6e65 6172 2836 342c 206e 756d  n.Linear(64, num
-00003ae0: 5f63 6c61 7373 6573 290a 0a20 2020 2064  _classes)..    d
-00003af0: 6566 205f 6d61 6b65 5f6c 6179 6572 2873  ef _make_layer(s
-00003b00: 656c 662c 2062 6c6f 636b 2c20 706c 616e  elf, block, plan
-00003b10: 6573 2c20 6e75 6d5f 626c 6f63 6b2c 2073  es, num_block, s
-00003b20: 7472 6964 6529 3a0a 2020 2020 2020 2020  tride):.        
-00003b30: 6c61 7965 7273 203d 205b 5d0a 2020 2020  layers = [].    
-00003b40: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00003b50: 6765 286e 756d 5f62 6c6f 636b 293a 0a20  ge(num_block):. 
-00003b60: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
-00003b70: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-00003b80: 2020 2020 2020 6c61 7965 7273 2e61 7070        layers.app
-00003b90: 656e 6428 626c 6f63 6b28 7365 6c66 2e69  end(block(self.i
-00003ba0: 6e5f 706c 616e 6573 2c20 706c 616e 6573  n_planes, planes
-00003bb0: 2c20 7374 7269 6465 2929 0a20 2020 2020  , stride)).     
-00003bc0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003bd0: 2020 2020 2020 2020 2020 2020 206c 6179               lay
-00003be0: 6572 732e 6170 7065 6e64 2862 6c6f 636b  ers.append(block
-00003bf0: 2870 6c61 6e65 732c 2070 6c61 6e65 732c  (planes, planes,
-00003c00: 2031 2929 0a20 2020 2020 2020 2073 656c   1)).        sel
-00003c10: 662e 696e 5f70 6c61 6e65 7320 3d20 706c  f.in_planes = pl
-00003c20: 616e 6573 0a20 2020 2020 2020 2072 6574  anes.        ret
-00003c30: 7572 6e20 6e6e 2e53 6571 7565 6e74 6961  urn nn.Sequentia
-00003c40: 6c28 2a6c 6179 6572 7329 0a0a 2020 2020  l(*layers)..    
-00003c50: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
-00003c60: 2c20 7829 3a0a 2020 2020 2020 2020 7820  , x):.        x 
-00003c70: 3d20 7365 6c66 2e6d 6178 706f 6f6c 2873  = self.maxpool(s
-00003c80: 656c 662e 636f 6e76 3128 7829 290a 2020  elf.conv1(x)).  
-00003c90: 2020 2020 2020 7820 3d20 7365 6c66 2e62        x = self.b
-00003ca0: 6c6f 636b 3128 7829 2020 2320 5b32 3030  lock1(x)  # [200
-00003cb0: 2c20 3634 2c20 3238 2c20 3238 5d0a 2020  , 64, 28, 28].  
-00003cc0: 2020 2020 2020 7820 3d20 7365 6c66 2e62        x = self.b
-00003cd0: 6c6f 636b 3228 7829 2020 2320 5b32 3030  lock2(x)  # [200
-00003ce0: 2c20 3132 382c 2031 342c 2031 345d 0a20  , 128, 14, 14]. 
-00003cf0: 2020 2020 2020 2078 203d 2073 656c 662e         x = self.
-00003d00: 626c 6f63 6b33 2878 2920 2023 205b 3230  block3(x)  # [20
-00003d10: 302c 2032 3536 2c20 372c 2037 5d0a 2020  0, 256, 7, 7].  
-00003d20: 2020 2020 2020 2320 6f75 7420 3d20 7365        # out = se
-00003d30: 6c66 2e62 6c6f 636b 3428 6f75 7429 0a20  lf.block4(out). 
-00003d40: 2020 2020 2020 2078 203d 2046 2e61 7667         x = F.avg
-00003d50: 5f70 6f6f 6c32 6428 782c 2037 2920 2023  _pool2d(x, 7)  #
-00003d60: 205b 3230 302c 2032 3536 2c20 312c 2031   [200, 256, 1, 1
-00003d70: 5d0a 2020 2020 2020 2020 7820 3d20 782e  ].        x = x.
-00003d80: 7669 6577 2878 2e73 697a 6528 3029 2c20  view(x.size(0), 
-00003d90: 2d31 2920 2023 205b 3230 302c 3235 365d  -1)  # [200,256]
-00003da0: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-00003db0: 656c 662e 6f75 746c 6179 6572 2878 290a  elf.outlayer(x).
-00003dc0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-00003dd0: 7574 0a0a 0a23 20e6 8d95 e88e b7e5 b9b6  ut...# .........
-00003de0: e58f afe8 a786 e58c 96e5 898d 3230 e5bc  ............20..
-00003df0: a0e5 9bbe e583 8f0a 6465 6620 6c6f 675f  ........def log_
-00003e00: 696d 6167 6573 286c 6f61 6465 722c 206e  images(loader, n
-00003e10: 756d 5f69 6d61 6765 733d 3136 293a 0a20  um_images=16):. 
-00003e20: 2020 2069 6d61 6765 735f 6c6f 6767 6564     images_logged
-00003e30: 203d 2030 0a20 2020 206c 6f67 6765 645f   = 0.    logged_
-00003e40: 696d 6167 6573 203d 205b 5d0a 2020 2020  images = [].    
-00003e50: 666f 7220 696d 6167 6573 2c20 6c61 6265  for images, labe
-00003e60: 6c73 2069 6e20 6c6f 6164 6572 3a0a 2020  ls in loader:.  
-00003e70: 2020 2020 2020 2320 696d 6167 6573 3a20        # images: 
-00003e80: 6261 7463 6820 6f66 2069 6d61 6765 732c  batch of images,
-00003e90: 206c 6162 656c 733a 2062 6174 6368 206f   labels: batch o
-00003ea0: 6620 6c61 6265 6c73 0a20 2020 2020 2020  f labels.       
-00003eb0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00003ec0: 696d 6167 6573 2e73 6861 7065 5b30 5d29  images.shape[0])
-00003ed0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00003ee0: 2069 6d61 6765 735f 6c6f 6767 6564 203c   images_logged <
-00003ef0: 206e 756d 5f69 6d61 6765 733a 0a20 2020   num_images:.   
-00003f00: 2020 2020 2020 2020 2020 2020 2023 20e4               # .
-00003f10: bdbf e794 a873 7761 6e6c 6162 2e49 6d61  .....swanlab.Ima
-00003f20: 6765 e5b0 86e5 9bbe e583 8fe8 bdac e68d  ge..............
-00003f30: a2e4 b8ba 7761 6e64 62e5 8faf e8a7 86e5  ....wandb.......
-00003f40: 8c96 e6a0 bce5 bc8f 0a20 2020 2020 2020  .........       
-00003f50: 2020 2020 2020 2020 206c 6f67 6765 645f           logged_
-00003f60: 696d 6167 6573 2e61 7070 656e 6428 7377  images.append(sw
-00003f70: 616e 6c61 622e 496d 6167 6528 696d 6167  anlab.Image(imag
-00003f80: 6573 5b69 5d2c 2063 6170 7469 6f6e 3d66  es[i], caption=f
-00003f90: 224c 6162 656c 3a20 7b6c 6162 656c 735b  "Label: {labels[
-00003fa0: 695d 7d22 2c20 7369 7a65 3d28 3132 382c  i]}", size=(128,
-00003fb0: 2031 3238 2929 290a 2020 2020 2020 2020   128))).        
-00003fc0: 2020 2020 2020 2020 696d 6167 6573 5f6c          images_l
-00003fd0: 6f67 6765 6420 2b3d 2031 0a20 2020 2020  ogged += 1.     
-00003fe0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003ff0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00004000: 616b 0a20 2020 2020 2020 2069 6620 696d  ak.        if im
-00004010: 6167 6573 5f6c 6f67 6765 6420 3e3d 206e  ages_logged >= n
-00004020: 756d 5f69 6d61 6765 733a 0a20 2020 2020  um_images:.     
-00004030: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00004040: 2073 7761 6e6c 6162 2e6c 6f67 287b 2250   swanlab.log({"P
-00004050: 7265 7669 6577 2f4d 4e49 5354 223a 206c  review/MNIST": l
-00004060: 6f67 6765 645f 696d 6167 6573 7d29 0a0a  ogged_images})..
-00004070: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00004080: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00004090: 2320 e8ae bee7 bdae 6465 7669 6365 0a20  # ......device. 
-000040a0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000040b0: 7573 655f 6d70 7320 3d20 746f 7263 682e  use_mps = torch.
-000040c0: 6261 636b 656e 6473 2e6d 7073 2e69 735f  backends.mps.is_
-000040d0: 6176 6169 6c61 626c 6528 290a 2020 2020  available().    
-000040e0: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
-000040f0: 4572 726f 723a 0a20 2020 2020 2020 2075  Error:.        u
-00004100: 7365 5f6d 7073 203d 2046 616c 7365 0a0a  se_mps = False..
-00004110: 2020 2020 6966 2074 6f72 6368 2e63 7564      if torch.cud
-00004120: 612e 6973 5f61 7661 696c 6162 6c65 2829  a.is_available()
-00004130: 3a0a 2020 2020 2020 2020 6465 7669 6365  :.        device
-00004140: 203d 2022 6375 6461 220a 2020 2020 656c   = "cuda".    el
-00004150: 6966 2075 7365 5f6d 7073 3a0a 2020 2020  if use_mps:.    
-00004160: 2020 2020 6465 7669 6365 203d 2022 6d70      device = "mp
-00004170: 7322 0a20 2020 2065 6c73 653a 0a20 2020  s".    else:.   
-00004180: 2020 2020 2064 6576 6963 6520 3d20 2263       device = "c
-00004190: 7075 220a 0a20 2020 2023 20e5 889d e5a7  pu"..    # .....
-000041a0: 8be5 8c96 7377 616e 6c61 620a 2020 2020  ....swanlab.    
-000041b0: 7275 6e20 3d20 7377 616e 6c61 622e 696e  run = swanlab.in
-000041c0: 6974 280a 2020 2020 2020 2020 7072 6f6a  it(.        proj
-000041d0: 6563 743d 2246 6173 6869 6f6e 4d4e 4953  ect="FashionMNIS
-000041e0: 5422 2c0a 2020 2020 2020 2020 776f 726b  T",.        work
-000041f0: 7370 6163 653d 2253 7761 6e4c 6162 222c  space="SwanLab",
-00004200: 0a20 2020 2020 2020 2065 7870 6572 696d  .        experim
-00004210: 656e 745f 6e61 6d65 3d22 5265 736e 6574  ent_name="Resnet
-00004220: 3138 2d41 6461 6d22 2c0a 2020 2020 2020  18-Adam",.      
-00004230: 2020 636f 6e66 6967 3d7b 0a20 2020 2020    config={.     
-00004240: 2020 2020 2020 2022 6d6f 6465 6c22 3a20         "model": 
-00004250: 2252 6573 6e65 7433 3422 2c0a 2020 2020  "Resnet34",.    
-00004260: 2020 2020 2020 2020 226f 7074 696d 223a          "optim":
-00004270: 2022 4164 616d 222c 0a20 2020 2020 2020   "Adam",.       
-00004280: 2020 2020 2022 6c72 223a 2030 2e30 3031       "lr": 0.001
-00004290: 2c0a 2020 2020 2020 2020 2020 2020 2262  ,.            "b
-000042a0: 6174 6368 5f73 697a 6522 3a20 3332 2c0a  atch_size": 32,.
-000042b0: 2020 2020 2020 2020 2020 2020 226e 756d              "num
-000042c0: 5f65 706f 6368 7322 3a20 3130 2c0a 2020  _epochs": 10,.  
-000042d0: 2020 2020 2020 2020 2020 2274 7261 696e            "train
-000042e0: 5f64 6174 6173 6574 5f6e 756d 223a 2035  _dataset_num": 5
-000042f0: 3530 3030 2c0a 2020 2020 2020 2020 2020  5000,.          
-00004300: 2020 2276 616c 5f64 6174 6173 6574 5f6e    "val_dataset_n
-00004310: 756d 223a 2035 3030 302c 0a20 2020 2020  um": 5000,.     
-00004320: 2020 2020 2020 2022 6465 7669 6365 223a         "device":
-00004330: 2064 6576 6963 652c 0a20 2020 2020 2020   device,.       
-00004340: 2020 2020 2022 6e75 6d5f 636c 6173 7365       "num_classe
-00004350: 7322 3a20 3130 2c0a 2020 2020 2020 2020  s": 10,.        
-00004360: 7d2c 0a20 2020 2029 0a0a 2020 2020 2320  },.    )..    # 
-00004370: e8ae bee7 bdae e8ae ade7 bb83 e69c bae3  ................
-00004380: 8081 e9aa 8ce8 af81 e99b 86e5 928c e6b5  ................
-00004390: 8be8 af95 e99b 860a 2020 2020 6461 7461  ........    data
-000043a0: 7365 7420 3d20 4661 7368 696f 6e4d 4e49  set = FashionMNI
-000043b0: 5354 286f 732e 6765 7463 7764 2829 2c20  ST(os.getcwd(), 
-000043c0: 7472 6169 6e3d 5472 7565 2c20 646f 776e  train=True, down
-000043d0: 6c6f 6164 3d54 7275 652c 2074 7261 6e73  load=True, trans
-000043e0: 666f 726d 3d54 6f54 656e 736f 7228 2929  form=ToTensor())
-000043f0: 0a20 2020 2074 7261 696e 5f64 6174 6173  .    train_datas
-00004400: 6574 2c20 7661 6c5f 6461 7461 7365 7420  et, val_dataset 
-00004410: 3d20 7574 696c 732e 6461 7461 2e72 616e  = utils.data.ran
-00004420: 646f 6d5f 7370 6c69 7428 0a20 2020 2020  dom_split(.     
-00004430: 2020 2064 6174 6173 6574 2c20 5b72 756e     dataset, [run
-00004440: 2e63 6f6e 6669 672e 7472 6169 6e5f 6461  .config.train_da
-00004450: 7461 7365 745f 6e75 6d2c 2072 756e 2e63  taset_num, run.c
-00004460: 6f6e 6669 672e 7661 6c5f 6461 7461 7365  onfig.val_datase
-00004470: 745f 6e75 6d5d 0a20 2020 2029 0a0a 2020  t_num].    )..  
-00004480: 2020 7472 6169 6e5f 6c6f 6164 6572 203d    train_loader =
-00004490: 2075 7469 6c73 2e64 6174 612e 4461 7461   utils.data.Data
-000044a0: 4c6f 6164 6572 2874 7261 696e 5f64 6174  Loader(train_dat
-000044b0: 6173 6574 2c20 6261 7463 685f 7369 7a65  aset, batch_size
-000044c0: 3d72 756e 2e63 6f6e 6669 672e 6261 7463  =run.config.batc
-000044d0: 685f 7369 7a65 2c20 7368 7566 666c 653d  h_size, shuffle=
-000044e0: 5472 7565 290a 2020 2020 7661 6c5f 6c6f  True).    val_lo
-000044f0: 6164 6572 203d 2075 7469 6c73 2e64 6174  ader = utils.dat
-00004500: 612e 4461 7461 4c6f 6164 6572 2876 616c  a.DataLoader(val
-00004510: 5f64 6174 6173 6574 2c20 6261 7463 685f  _dataset, batch_
-00004520: 7369 7a65 3d31 2c20 7368 7566 666c 653d  size=1, shuffle=
-00004530: 4661 6c73 6529 0a0a 2020 2020 2320 e588  False)..    # ..
-00004540: 9de5 a78b e58c 96e6 a8a1 e59e 8be3 8081  ................
-00004550: e68d 9fe5 a4b1 e587 bde6 95b0 e592 8ce4  ................
-00004560: bc98 e58c 96e5 99a8 0a20 2020 2069 6620  .........    if 
-00004570: 7275 6e2e 636f 6e66 6967 2e6d 6f64 656c  run.config.model
-00004580: 203d 3d20 2252 6573 6e65 7431 3822 3a0a   == "Resnet18":.
-00004590: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
-000045a0: 5265 734e 6574 2842 6173 6963 626c 6f63  ResNet(Basicbloc
-000045b0: 6b2c 205b 312c 2031 2c20 312c 2031 5d2c  k, [1, 1, 1, 1],
-000045c0: 2031 3029 0a20 2020 2065 6c69 6620 7275   10).    elif ru
-000045d0: 6e2e 636f 6e66 6967 2e6d 6f64 656c 203d  n.config.model =
-000045e0: 3d20 2252 6573 6e65 7433 3422 3a0a 2020  = "Resnet34":.  
-000045f0: 2020 2020 2020 6d6f 6465 6c20 3d20 5265        model = Re
-00004600: 734e 6574 2842 6173 6963 626c 6f63 6b2c  sNet(Basicblock,
-00004610: 205b 322c 2033 2c20 352c 2032 5d2c 2031   [2, 3, 5, 2], 1
-00004620: 3029 0a20 2020 2065 6c69 6620 7275 6e2e  0).    elif run.
-00004630: 636f 6e66 6967 2e6d 6f64 656c 203d 3d20  config.model == 
-00004640: 2252 6573 6e65 7435 3022 3a0a 2020 2020  "Resnet50":.    
-00004650: 2020 2020 6d6f 6465 6c20 3d20 5265 734e      model = ResN
-00004660: 6574 2842 6173 6963 626c 6f63 6b2c 205b  et(Basicblock, [
-00004670: 332c 2034 2c20 362c 2033 5d2c 2031 3029  3, 4, 6, 3], 10)
-00004680: 0a0a 2020 2020 6d6f 6465 6c2e 746f 2874  ..    model.to(t
-00004690: 6f72 6368 2e64 6576 6963 6528 6465 7669  orch.device(devi
-000046a0: 6365 2929 0a0a 2020 2020 6372 6974 6572  ce))..    criter
-000046b0: 696f 6e20 3d20 6e6e 2e43 726f 7373 456e  ion = nn.CrossEn
-000046c0: 7472 6f70 794c 6f73 7328 290a 2020 2020  tropyLoss().    
-000046d0: 6f70 7469 6d69 7a65 7220 3d20 6f70 7469  optimizer = opti
-000046e0: 6d2e 4164 616d 286d 6f64 656c 2e70 6172  m.Adam(model.par
-000046f0: 616d 6574 6572 7328 292c 206c 723d 7275  ameters(), lr=ru
-00004700: 6e2e 636f 6e66 6967 2e6c 7229 0a0a 2020  n.config.lr)..  
-00004710: 2020 2320 efbc 88e5 8faf e980 89ef bc89    # ............
-00004720: e79c 8be4 b880 e4b8 8be6 95b0 e68d aee9  ................
-00004730: 9b86 e79a 84e5 898d 3136 e5bc a0e5 9bbe  ........16......
-00004740: e583 8f0a 2020 2020 6c6f 675f 696d 6167  ....    log_imag
-00004750: 6573 2874 7261 696e 5f6c 6f61 6465 722c  es(train_loader,
-00004760: 2031 3629 0a0a 2020 2020 2320 e5bc 80e5   16)..    # ....
-00004770: a78b e8ae ade7 bb83 0a20 2020 2066 6f72  .........    for
-00004780: 2065 706f 6368 2069 6e20 7261 6e67 6528   epoch in range(
-00004790: 312c 2072 756e 2e63 6f6e 6669 672e 6e75  1, run.config.nu
-000047a0: 6d5f 6570 6f63 6873 202b 2031 293a 0a20  m_epochs + 1):. 
-000047b0: 2020 2020 2020 2073 7761 6e6c 6162 2e6c         swanlab.l
-000047c0: 6f67 287b 2274 7261 696e 2f65 706f 6368  og({"train/epoch
-000047d0: 223a 2065 706f 6368 7d2c 2073 7465 703d  ": epoch}, step=
-000047e0: 6570 6f63 6829 0a20 2020 2020 2020 2023  epoch).        #
-000047f0: 20e8 aead e7bb 83e5 beaa e78e af0a 2020   .............  
-00004800: 2020 2020 2020 666f 7220 6974 6572 2c20        for iter, 
-00004810: 6261 7463 6820 696e 2065 6e75 6d65 7261  batch in enumera
-00004820: 7465 2874 7261 696e 5f6c 6f61 6465 7229  te(train_loader)
-00004830: 3a0a 2020 2020 2020 2020 2020 2020 782c  :.            x,
-00004840: 2079 203d 2062 6174 6368 0a20 2020 2020   y = batch.     
-00004850: 2020 2020 2020 2078 2c20 7920 3d20 782e         x, y = x.
-00004860: 746f 2864 6576 6963 6529 2c20 792e 746f  to(device), y.to
-00004870: 2864 6576 6963 6529 0a20 2020 2020 2020  (device).       
-00004880: 2020 2020 206f 7074 696d 697a 6572 2e7a       optimizer.z
-00004890: 6572 6f5f 6772 6164 2829 0a20 2020 2020  ero_grad().     
-000048a0: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
-000048b0: 6d6f 6465 6c28 7829 0a20 2020 2020 2020  model(x).       
-000048c0: 2020 2020 206c 6f73 7320 3d20 6372 6974       loss = crit
-000048d0: 6572 696f 6e28 6f75 7470 7574 2c20 7929  erion(output, y)
-000048e0: 0a20 2020 2020 2020 2020 2020 206c 6f73  .            los
-000048f0: 732e 6261 636b 7761 7264 2829 0a20 2020  s.backward().   
-00004900: 2020 2020 2020 2020 206f 7074 696d 697a           optimiz
-00004910: 6572 2e73 7465 7028 290a 0a20 2020 2020  er.step()..     
-00004920: 2020 2020 2020 2069 6620 6974 6572 2025         if iter %
-00004930: 2034 3020 3d3d 2030 3a0a 2020 2020 2020   40 == 0:.      
-00004940: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00004950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004960: 2020 2020 2066 2245 706f 6368 205b 7b65       f"Epoch [{e
-00004970: 706f 6368 7d2f 7b72 756e 2e63 6f6e 6669  poch}/{run.confi
-00004980: 672e 6e75 6d5f 6570 6f63 6873 7d5d 2c20  g.num_epochs}], 
-00004990: 4974 6572 6174 696f 6e20 5b7b 6974 6572  Iteration [{iter
-000049a0: 202b 2031 7d2f 7b6c 656e 2874 7261 696e   + 1}/{len(train
-000049b0: 5f6c 6f61 6465 7229 7d5d 2c20 4c6f 7373  _loader)}], Loss
-000049c0: 3a20 7b6c 6f73 732e 6974 656d 2829 7d22  : {loss.item()}"
-000049d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000049e0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000049f0: 2020 2073 7761 6e6c 6162 2e6c 6f67 287b     swanlab.log({
-00004a00: 2274 7261 696e 2f6c 6f73 7322 3a20 6c6f  "train/loss": lo
-00004a10: 7373 2e69 7465 6d28 297d 2c20 7374 6570  ss.item()}, step
-00004a20: 3d28 6570 6f63 6820 2d20 3129 202a 206c  =(epoch - 1) * l
-00004a30: 656e 2874 7261 696e 5f6c 6f61 6465 7229  en(train_loader)
-00004a40: 202b 2069 7465 7229 0a0a 2020 2020 2020   + iter)..      
-00004a50: 2020 2320 e6af 8f34 e4b8 aa65 706f 6368    # ...4...epoch
-00004a60: e9aa 8ce8 af81 e4b8 80e6 aca1 0a20 2020  .............   
-00004a70: 2020 2020 2069 6620 6570 6f63 6820 2520       if epoch % 
-00004a80: 3220 3d3d 2030 3a0a 2020 2020 2020 2020  2 == 0:.        
-00004a90: 2020 2020 6d6f 6465 6c2e 6576 616c 2829      model.eval()
-00004aa0: 0a20 2020 2020 2020 2020 2020 2063 6f72  .            cor
-00004ab0: 7265 6374 203d 2030 0a20 2020 2020 2020  rect = 0.       
-00004ac0: 2020 2020 2074 6f74 616c 203d 2030 0a20       total = 0. 
-00004ad0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00004ae0: 746f 7263 682e 6e6f 5f67 7261 6428 293a  torch.no_grad():
-00004af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b00: 2066 6f72 2062 6174 6368 2069 6e20 7661   for batch in va
-00004b10: 6c5f 6c6f 6164 6572 3a0a 2020 2020 2020  l_loader:.      
-00004b20: 2020 2020 2020 2020 2020 2020 2020 782c                x,
-00004b30: 2079 203d 2062 6174 6368 0a20 2020 2020   y = batch.     
-00004b40: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00004b50: 2c20 7920 3d20 782e 746f 2864 6576 6963  , y = x.to(devic
-00004b60: 6529 2c20 792e 746f 2864 6576 6963 6529  e), y.to(device)
-00004b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b80: 2020 2020 206f 7574 7075 7420 3d20 6d6f       output = mo
-00004b90: 6465 6c28 7829 0a20 2020 2020 2020 2020  del(x).         
-00004ba0: 2020 2020 2020 2020 2020 205f 2c20 7072             _, pr
-00004bb0: 6564 6963 7465 6420 3d20 746f 7263 682e  edicted = torch.
-00004bc0: 6d61 7828 6f75 7470 7574 2c20 3129 0a20  max(output, 1). 
-00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004be0: 2020 2074 6f74 616c 202b 3d20 792e 7369     total += y.si
-00004bf0: 7a65 2830 290a 2020 2020 2020 2020 2020  ze(0).          
-00004c00: 2020 2020 2020 2020 2020 636f 7272 6563            correc
-00004c10: 7420 2b3d 2028 7072 6564 6963 7465 6420  t += (predicted 
-00004c20: 3d3d 2079 292e 7375 6d28 292e 6974 656d  == y).sum().item
-00004c30: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00004c40: 6163 6375 7261 6379 203d 2063 6f72 7265  accuracy = corre
-00004c50: 6374 202f 2074 6f74 616c 0a20 2020 2020  ct / total.     
-00004c60: 2020 2020 2020 2073 7761 6e6c 6162 2e6c         swanlab.l
-00004c70: 6f67 287b 2276 616c 2f61 6363 7572 6163  og({"val/accurac
-00004c80: 7922 3a20 6163 6375 7261 6379 7d2c 2073  y": accuracy}, s
-00004c90: 7465 703d 6570 6f63 6829 0a60 6060 0a0a  tep=epoch).```..
-00004ca0: 3c2f 6465 7461 696c 733e 0a0a 3c62 723e  </details>..<br>
-00004cb0: 0a0a 2323 20f0 9f92 bb20 5365 6c66 2d68  ..## .... Self-h
-00004cc0: 6f73 7465 640a 0a54 6865 2063 6f6d 6d75  osted..The commu
-00004cd0: 6e69 7479 2065 6469 7469 6f6e 2073 7570  nity edition sup
-00004ce0: 706f 7274 7320 6f66 666c 696e 6520 7669  ports offline vi
-00004cf0: 6577 696e 6720 6f66 2053 7761 6e4c 6162  ewing of SwanLab
-00004d00: 2064 6173 6862 6f61 7264 732e 0a0a 2323   dashboards...##
-00004d10: 2320 4f66 666c 696e 6520 4578 7065 7269  # Offline Experi
-00004d20: 6d65 6e74 2054 7261 636b 696e 670a 0a53  ment Tracking..S
-00004d30: 6574 2074 6865 2070 6172 616d 6574 6572  et the parameter
-00004d40: 7320 606c 6f67 6972 6020 616e 6420 606d  s `logir` and `m
-00004d50: 6f64 6560 2069 6e20 7377 616e 6c61 622e  ode` in swanlab.
-00004d60: 696e 6974 2074 6f20 7472 6163 6b20 6578  init to track ex
-00004d70: 7065 7269 6d65 6e74 7320 6f66 666c 696e  periments offlin
-00004d80: 653a 0a0a 6060 6070 7974 686f 6e0a 2e2e  e:..```python...
-00004d90: 2e0a 0a73 7761 6e6c 6162 2e69 6e69 7428  ...swanlab.init(
-00004da0: 0a20 2020 206c 6f67 6469 723d 272e 2f6c  .    logdir='./l
-00004db0: 6f67 7327 2c0a 2020 2020 6d6f 6465 3d27  ogs',.    mode='
-00004dc0: 6c6f 6361 6c27 2c0a 290a 0a2e 2e2e 0a60  local',.)......`
-00004dd0: 6060 0a0a 2d20 5468 6520 7061 7261 6d65  ``..- The parame
-00004de0: 7465 7220 606d 6f64 6560 2069 7320 7365  ter `mode` is se
-00004df0: 7420 746f 2060 6c6f 6361 6c60 2c20 7768  t to `local`, wh
-00004e00: 6963 6820 6469 7361 626c 6573 2073 796e  ich disables syn
-00004e10: 6368 726f 6e69 7a69 6e67 2074 6865 2065  chronizing the e
-00004e20: 7870 6572 696d 656e 7420 746f 2074 6865  xperiment to the
-00004e30: 2063 6c6f 7564 2e0a 0a2d 2054 6865 2073   cloud...- The s
-00004e40: 6574 7469 6e67 206f 6620 7468 6520 7061  etting of the pa
-00004e50: 7261 6d65 7465 7220 606c 6f67 6469 7260  rameter `logdir`
-00004e60: 2069 7320 6f70 7469 6f6e 616c 2c20 616e   is optional, an
-00004e70: 6420 6974 2073 7065 6369 6669 6573 2074  d it specifies t
-00004e80: 6865 206c 6f63 6174 696f 6e20 666f 7220  he location for 
-00004e90: 7361 7669 6e67 2053 7761 6e4c 6162 206c  saving SwanLab l
-00004ea0: 6f67 2066 696c 6573 2028 6279 0a20 2064  og files (by.  d
-00004eb0: 6566 6175 6c74 2073 6176 6564 2069 6e20  efault saved in 
-00004ec0: 7468 6520 6073 7761 6e6c 6f67 6020 666f  the `swanlog` fo
-00004ed0: 6c64 6572 292e 0a0a 2d20 4c6f 6720 6669  lder)...- Log fi
-00004ee0: 6c65 7320 7769 6c6c 2062 6520 6372 6561  les will be crea
-00004ef0: 7465 6420 616e 6420 7570 6461 7465 6420  ted and updated 
-00004f00: 6475 7269 6e67 2074 7261 636b 696e 6720  during tracking 
-00004f10: 6f66 2065 7870 6572 696d 656e 7473 2c20  of experiments, 
-00004f20: 616e 6420 6c61 756e 6368 696e 6720 6f66  and launching of
-00004f30: 666c 696e 6520 6461 7368 626f 6172 6473  fline dashboards
-00004f40: 2077 696c 6c20 616c 736f 2062 650a 2020   will also be.  
-00004f50: 6261 7365 6420 6f6e 2074 6865 7365 206c  based on these l
-00004f60: 6f67 2066 696c 6573 2e0a 0a4f 7468 6572  og files...Other
-00004f70: 2070 6172 7473 2061 7265 2063 6f6d 706c   parts are compl
-00004f80: 6574 656c 7920 636f 6e73 6973 7465 6e74  etely consistent
-00004f90: 2077 6974 6820 636c 6f75 6420 7573 6167   with cloud usag
-00004fa0: 652e 0a0a 2323 2320 4f70 656e 204f 6666  e...### Open Off
-00004fb0: 6c69 6e65 2042 6f61 7264 0a0a 4f70 656e  line Board..Open
-00004fc0: 2074 6865 2074 6572 6d69 6e61 6c20 616e   the terminal an
-00004fd0: 6420 7573 6520 7468 6520 666f 6c6c 6f77  d use the follow
-00004fe0: 696e 6720 636f 6d6d 616e 6420 746f 206f  ing command to o
-00004ff0: 7065 6e20 6120 5377 616e 4c61 6220 6461  pen a SwanLab da
-00005000: 7368 626f 6172 643a 0a0a 6060 6062 6173  shboard:..```bas
-00005010: 680a 7377 616e 6c61 6220 7761 7463 6820  h.swanlab watch 
-00005020: 2d6c 202e 2f6c 6f67 730a 6060 600a 0a41  -l ./logs.```..A
-00005030: 6674 6572 2074 6865 206f 7065 7261 7469  fter the operati
-00005040: 6f6e 2069 7320 636f 6d70 6c65 7465 642c  on is completed,
-00005050: 2053 7761 6e4c 6162 2077 696c 6c20 7072   SwanLab will pr
-00005060: 6f76 6964 6520 796f 7520 7769 7468 2061  ovide you with a
-00005070: 206c 6f63 616c 2055 524c 206c 696e 6b20   local URL link 
-00005080: 2864 6566 6175 6c74 0a69 7320 5b68 7474  (default.is [htt
-00005090: 703a 2f2f 3132 372e 302e 302e 313a 3530  p://127.0.0.1:50
-000050a0: 3932 5d28 6874 7470 3a2f 2f31 3237 2e30  92](http://127.0
-000050b0: 2e30 2e31 3a35 3039 3229 292e 0a0a 5669  .0.1:5092))...Vi
-000050c0: 7369 7420 7468 6973 206c 696e 6b20 746f  sit this link to
-000050d0: 2076 6965 7720 7468 6520 6578 7065 7269   view the experi
-000050e0: 6d65 6e74 206f 6666 6c69 6e65 2069 6e20  ment offline in 
-000050f0: 7468 6520 6272 6f77 7365 7220 6461 7368  the browser dash
-00005100: 626f 6172 642e 0a0a 3c62 723e 0a0a 2323  board...<br>..##
-00005110: 20f0 9f9a 9720 496e 7465 6772 6174 696f   .... Integratio
-00005120: 6e0a 0a43 6f6d 6269 6e65 2079 6f75 7220  n..Combine your 
-00005130: 6661 766f 7269 7465 2066 7261 6d65 776f  favorite framewo
-00005140: 726b 2077 6974 680a 5377 616e 4c61 622c  rk with.SwanLab,
-00005150: 205b 4d6f 7265 2049 6e74 6567 7261 7469   [More Integrati
-00005160: 6f6e 5d28 6874 7470 733a 2f2f 646f 6373  on](https://docs
-00005170: 2e73 7761 6e6c 6162 2e63 6e2f 7a68 2f67  .swanlab.cn/zh/g
-00005180: 7569 6465 5f63 6c6f 7564 2f69 6e74 6567  uide_cloud/integ
-00005190: 7261 7469 6f6e 2f69 6e74 6567 7261 7469  ration/integrati
-000051a0: 6f6e 2d70 7974 6f72 6368 2d6c 6967 6874  on-pytorch-light
-000051b0: 6e69 6e67 2e68 746d 6c29 2e0a 0a3c 6465  ning.html)...<de
-000051c0: 7461 696c 733e 0a20 203c 7375 6d6d 6172  tails>.  <summar
-000051d0: 793e 0a20 2020 203c 7374 726f 6e67 3ee2  y>.    <strong>.
-000051e0: 9aa1 efb8 8f20 5079 546f 7263 6820 4c69  ..... PyTorch Li
-000051f0: 6768 746e 696e 673c 2f73 7472 6f6e 673e  ghtning</strong>
-00005200: 0a20 203c 2f73 756d 6d61 7279 3e0a 2020  .  </summary>.  
-00005210: 3c62 723e 0a0a 4372 6561 7465 2061 6e20  <br>..Create an 
-00005220: 696e 7374 616e 6365 2075 7369 6e67 2060  instance using `
-00005230: 5377 616e 4c61 624c 6f67 6765 7260 2061  SwanLabLogger` a
-00005240: 6e64 2070 6173 7320 6974 2069 6e74 6f20  nd pass it into 
-00005250: 7468 6520 606c 6f67 6765 7260 2070 6172  the `logger` par
-00005260: 616d 6574 6572 206f 6620 6054 7261 696e  ameter of `Train
-00005270: 6572 6020 746f 2065 6e61 626c 6520 5377  er` to enable Sw
-00005280: 616e 4c61 6220 746f 0a72 6563 6f72 6420  anLab to.record 
-00005290: 7472 6169 6e69 6e67 206d 6574 7269 6373  training metrics
-000052a0: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
-000052b0: 6d20 7377 616e 6c61 622e 696e 7465 6772  m swanlab.integr
-000052c0: 6174 696f 6e2e 7079 746f 7263 685f 6c69  ation.pytorch_li
-000052d0: 6768 746e 696e 6720 696d 706f 7274 2053  ghtning import S
-000052e0: 7761 6e4c 6162 4c6f 6767 6572 0a69 6d70  wanLabLogger.imp
-000052f0: 6f72 7420 696d 706f 7274 6c69 622e 7574  ort importlib.ut
-00005300: 696c 0a69 6d70 6f72 7420 6f73 0a69 6d70  il.import os.imp
-00005310: 6f72 7420 7079 746f 7263 685f 6c69 6768  ort pytorch_ligh
-00005320: 746e 696e 6720 6173 2070 6c0a 6672 6f6d  tning as pl.from
-00005330: 2074 6f72 6368 2069 6d70 6f72 7420 6e6e   torch import nn
-00005340: 2c20 6f70 7469 6d2c 2075 7469 6c73 0a66  , optim, utils.f
-00005350: 726f 6d20 746f 7263 6876 6973 696f 6e2e  rom torchvision.
-00005360: 6461 7461 7365 7473 2069 6d70 6f72 7420  datasets import 
-00005370: 4d4e 4953 540a 6672 6f6d 2074 6f72 6368  MNIST.from torch
-00005380: 7669 7369 6f6e 2e74 7261 6e73 666f 726d  vision.transform
-00005390: 7320 696d 706f 7274 2054 6f54 656e 736f  s import ToTenso
-000053a0: 720a 0a65 6e63 6f64 6572 203d 206e 6e2e  r..encoder = nn.
-000053b0: 5365 7175 656e 7469 616c 286e 6e2e 4c69  Sequential(nn.Li
-000053c0: 6e65 6172 2832 3820 2a20 3238 2c20 3132  near(28 * 28, 12
-000053d0: 3829 2c20 6e6e 2e52 654c 5528 292c 206e  8), nn.ReLU(), n
-000053e0: 6e2e 4c69 6e65 6172 2831 3238 2c20 3329  n.Linear(128, 3)
-000053f0: 290a 6465 636f 6465 7220 3d20 6e6e 2e53  ).decoder = nn.S
-00005400: 6571 7565 6e74 6961 6c28 6e6e 2e4c 696e  equential(nn.Lin
-00005410: 6561 7228 332c 2031 3238 292c 206e 6e2e  ear(3, 128), nn.
-00005420: 5265 4c55 2829 2c20 6e6e 2e4c 696e 6561  ReLU(), nn.Linea
-00005430: 7228 3132 382c 2032 3820 2a20 3238 2929  r(128, 28 * 28))
-00005440: 0a0a 0a63 6c61 7373 204c 6974 4175 746f  ...class LitAuto
-00005450: 456e 636f 6465 7228 706c 2e4c 6967 6874  Encoder(pl.Light
-00005460: 6e69 6e67 4d6f 6475 6c65 293a 0a20 2020  ningModule):.   
-00005470: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00005480: 6c66 2c20 656e 636f 6465 722c 2064 6563  lf, encoder, dec
-00005490: 6f64 6572 293a 0a20 2020 2020 2020 2073  oder):.        s
-000054a0: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-000054b0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
-000054c0: 6e63 6f64 6572 203d 2065 6e63 6f64 6572  ncoder = encoder
-000054d0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
-000054e0: 636f 6465 7220 3d20 6465 636f 6465 720a  coder = decoder.
-000054f0: 0a20 2020 2064 6566 2074 7261 696e 696e  .    def trainin
-00005500: 675f 7374 6570 2873 656c 662c 2062 6174  g_step(self, bat
-00005510: 6368 2c20 6261 7463 685f 6964 7829 3a0a  ch, batch_idx):.
-00005520: 2020 2020 2020 2020 2320 7472 6169 6e69          # traini
-00005530: 6e67 5f73 7465 7020 6465 6669 6e65 7320  ng_step defines 
-00005540: 7468 6520 7472 6169 6e20 6c6f 6f70 2e0a  the train loop..
-00005550: 2020 2020 2020 2020 2320 6974 2069 7320          # it is 
-00005560: 696e 6465 7065 6e64 656e 7420 6f66 2066  independent of f
-00005570: 6f72 7761 7264 0a20 2020 2020 2020 2078  orward.        x
-00005580: 2c20 7920 3d20 6261 7463 680a 2020 2020  , y = batch.    
-00005590: 2020 2020 7820 3d20 782e 7669 6577 2878      x = x.view(x
-000055a0: 2e73 697a 6528 3029 2c20 2d31 290a 2020  .size(0), -1).  
-000055b0: 2020 2020 2020 7a20 3d20 7365 6c66 2e65        z = self.e
-000055c0: 6e63 6f64 6572 2878 290a 2020 2020 2020  ncoder(x).      
-000055d0: 2020 785f 6861 7420 3d20 7365 6c66 2e64    x_hat = self.d
-000055e0: 6563 6f64 6572 287a 290a 2020 2020 2020  ecoder(z).      
-000055f0: 2020 6c6f 7373 203d 206e 6e2e 6675 6e63    loss = nn.func
-00005600: 7469 6f6e 616c 2e6d 7365 5f6c 6f73 7328  tional.mse_loss(
-00005610: 785f 6861 742c 2078 290a 2020 2020 2020  x_hat, x).      
-00005620: 2020 2320 4c6f 6767 696e 6720 746f 2054    # Logging to T
-00005630: 656e 736f 7242 6f61 7264 2028 6966 2069  ensorBoard (if i
-00005640: 6e73 7461 6c6c 6564 2920 6279 2064 6566  nstalled) by def
-00005650: 6175 6c74 0a20 2020 2020 2020 2073 656c  ault.        sel
-00005660: 662e 6c6f 6728 2274 7261 696e 5f6c 6f73  f.log("train_los
-00005670: 7322 2c20 6c6f 7373 290a 2020 2020 2020  s", loss).      
-00005680: 2020 7265 7475 726e 206c 6f73 730a 0a20    return loss.. 
-00005690: 2020 2064 6566 2074 6573 745f 7374 6570     def test_step
-000056a0: 2873 656c 662c 2062 6174 6368 2c20 6261  (self, batch, ba
-000056b0: 7463 685f 6964 7829 3a0a 2020 2020 2020  tch_idx):.      
-000056c0: 2020 2320 7465 7374 5f73 7465 7020 6465    # test_step de
-000056d0: 6669 6e65 7320 7468 6520 7465 7374 206c  fines the test l
-000056e0: 6f6f 702e 0a20 2020 2020 2020 2023 2069  oop..        # i
-000056f0: 7420 6973 2069 6e64 6570 656e 6465 6e74  t is independent
-00005700: 206f 6620 666f 7277 6172 640a 2020 2020   of forward.    
-00005710: 2020 2020 782c 2079 203d 2062 6174 6368      x, y = batch
-00005720: 0a20 2020 2020 2020 2078 203d 2078 2e76  .        x = x.v
-00005730: 6965 7728 782e 7369 7a65 2830 292c 202d  iew(x.size(0), -
-00005740: 3129 0a20 2020 2020 2020 207a 203d 2073  1).        z = s
-00005750: 656c 662e 656e 636f 6465 7228 7829 0a20  elf.encoder(x). 
-00005760: 2020 2020 2020 2078 5f68 6174 203d 2073         x_hat = s
-00005770: 656c 662e 6465 636f 6465 7228 7a29 0a20  elf.decoder(z). 
-00005780: 2020 2020 2020 206c 6f73 7320 3d20 6e6e         loss = nn
-00005790: 2e66 756e 6374 696f 6e61 6c2e 6d73 655f  .functional.mse_
-000057a0: 6c6f 7373 2878 5f68 6174 2c20 7829 0a20  loss(x_hat, x). 
-000057b0: 2020 2020 2020 2023 204c 6f67 6769 6e67         # Logging
-000057c0: 2074 6f20 5465 6e73 6f72 426f 6172 6420   to TensorBoard 
-000057d0: 2869 6620 696e 7374 616c 6c65 6429 2062  (if installed) b
-000057e0: 7920 6465 6661 756c 740a 2020 2020 2020  y default.      
-000057f0: 2020 7365 6c66 2e6c 6f67 2822 7465 7374    self.log("test
-00005800: 5f6c 6f73 7322 2c20 6c6f 7373 290a 2020  _loss", loss).  
-00005810: 2020 2020 2020 7265 7475 726e 206c 6f73        return los
-00005820: 730a 0a20 2020 2064 6566 2063 6f6e 6669  s..    def confi
-00005830: 6775 7265 5f6f 7074 696d 697a 6572 7328  gure_optimizers(
-00005840: 7365 6c66 293a 0a20 2020 2020 2020 206f  self):.        o
-00005850: 7074 696d 697a 6572 203d 206f 7074 696d  ptimizer = optim
-00005860: 2e41 6461 6d28 7365 6c66 2e70 6172 616d  .Adam(self.param
-00005870: 6574 6572 7328 292c 206c 723d 3165 2d33  eters(), lr=1e-3
-00005880: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00005890: 206f 7074 696d 697a 6572 0a0a 0a23 2069   optimizer...# i
-000058a0: 6e69 7420 7468 6520 6175 746f 656e 636f  nit the autoenco
-000058b0: 6465 720a 6175 746f 656e 636f 6465 7220  der.autoencoder 
-000058c0: 3d20 4c69 7441 7574 6f45 6e63 6f64 6572  = LitAutoEncoder
-000058d0: 2865 6e63 6f64 6572 2c20 6465 636f 6465  (encoder, decode
-000058e0: 7229 0a0a 2320 7365 7475 7020 6461 7461  r)..# setup data
-000058f0: 0a64 6174 6173 6574 203d 204d 4e49 5354  .dataset = MNIST
-00005900: 286f 732e 6765 7463 7764 2829 2c20 7472  (os.getcwd(), tr
-00005910: 6169 6e3d 5472 7565 2c20 646f 776e 6c6f  ain=True, downlo
-00005920: 6164 3d54 7275 652c 2074 7261 6e73 666f  ad=True, transfo
-00005930: 726d 3d54 6f54 656e 736f 7228 2929 0a74  rm=ToTensor()).t
-00005940: 7261 696e 5f64 6174 6173 6574 2c20 7661  rain_dataset, va
-00005950: 6c5f 6461 7461 7365 7420 3d20 7574 696c  l_dataset = util
-00005960: 732e 6461 7461 2e72 616e 646f 6d5f 7370  s.data.random_sp
-00005970: 6c69 7428 6461 7461 7365 742c 205b 3535  lit(dataset, [55
-00005980: 3030 302c 2035 3030 305d 290a 7465 7374  000, 5000]).test
-00005990: 5f64 6174 6173 6574 203d 204d 4e49 5354  _dataset = MNIST
-000059a0: 286f 732e 6765 7463 7764 2829 2c20 7472  (os.getcwd(), tr
-000059b0: 6169 6e3d 4661 6c73 652c 2064 6f77 6e6c  ain=False, downl
-000059c0: 6f61 643d 5472 7565 2c20 7472 616e 7366  oad=True, transf
-000059d0: 6f72 6d3d 546f 5465 6e73 6f72 2829 290a  orm=ToTensor()).
-000059e0: 0a74 7261 696e 5f6c 6f61 6465 7220 3d20  .train_loader = 
-000059f0: 7574 696c 732e 6461 7461 2e44 6174 614c  utils.data.DataL
-00005a00: 6f61 6465 7228 7472 6169 6e5f 6461 7461  oader(train_data
-00005a10: 7365 7429 0a76 616c 5f6c 6f61 6465 7220  set).val_loader 
-00005a20: 3d20 7574 696c 732e 6461 7461 2e44 6174  = utils.data.Dat
-00005a30: 614c 6f61 6465 7228 7661 6c5f 6461 7461  aLoader(val_data
-00005a40: 7365 7429 0a74 6573 745f 6c6f 6164 6572  set).test_loader
-00005a50: 203d 2075 7469 6c73 2e64 6174 612e 4461   = utils.data.Da
-00005a60: 7461 4c6f 6164 6572 2874 6573 745f 6461  taLoader(test_da
-00005a70: 7461 7365 7429 0a0a 7377 616e 6c61 625f  taset)..swanlab_
-00005a80: 6c6f 6767 6572 203d 2053 7761 6e4c 6162  logger = SwanLab
-00005a90: 4c6f 6767 6572 280a 2020 2020 7072 6f6a  Logger(.    proj
-00005aa0: 6563 743d 2273 7761 6e6c 6162 5f65 7861  ect="swanlab_exa
-00005ab0: 6d70 6c65 222c 0a20 2020 2065 7870 6572  mple",.    exper
-00005ac0: 696d 656e 745f 6e61 6d65 3d22 6578 616d  iment_name="exam
-00005ad0: 706c 655f 6578 7065 7269 6d65 6e74 222c  ple_experiment",
-00005ae0: 0a20 2020 2063 6c6f 7564 3d46 616c 7365  .    cloud=False
-00005af0: 2c0a 290a 0a74 7261 696e 6572 203d 2070  ,.)..trainer = p
-00005b00: 6c2e 5472 6169 6e65 7228 6c69 6d69 745f  l.Trainer(limit_
-00005b10: 7472 6169 6e5f 6261 7463 6865 733d 3130  train_batches=10
-00005b20: 302c 206d 6178 5f65 706f 6368 733d 352c  0, max_epochs=5,
-00005b30: 206c 6f67 6765 723d 7377 616e 6c61 625f   logger=swanlab_
-00005b40: 6c6f 6767 6572 290a 0a74 7261 696e 6572  logger)..trainer
-00005b50: 2e66 6974 286d 6f64 656c 3d61 7574 6f65  .fit(model=autoe
-00005b60: 6e63 6f64 6572 2c20 7472 6169 6e5f 6461  ncoder, train_da
-00005b70: 7461 6c6f 6164 6572 733d 7472 6169 6e5f  taloaders=train_
-00005b80: 6c6f 6164 6572 2c20 7661 6c5f 6461 7461  loader, val_data
-00005b90: 6c6f 6164 6572 733d 7661 6c5f 6c6f 6164  loaders=val_load
-00005ba0: 6572 290a 7472 6169 6e65 722e 7465 7374  er).trainer.test
-00005bb0: 2864 6174 616c 6f61 6465 7273 3d74 6573  (dataloaders=tes
-00005bc0: 745f 6c6f 6164 6572 290a 0a60 6060 0a0a  t_loader)..```..
-00005bd0: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
-00005be0: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e0a  ails>.<summary>.
-00005bf0: 2020 3c73 7472 6f6e 673e 20f0 9fa4 9748    <strong> ....H
-00005c00: 7567 6769 6e67 4661 6365 2054 7261 6e73  uggingFace Trans
-00005c10: 666f 726d 6572 733c 2f73 7472 6f6e 673e  formers</strong>
-00005c20: 0a3c 2f73 756d 6d61 7279 3e0a 0a3c 6272  .</summary>..<br
-00005c30: 3e0a 0a43 7265 6174 6520 616e 2069 6e73  >..Create an ins
-00005c40: 7461 6e63 6520 7573 696e 6720 6053 7761  tance using `Swa
-00005c50: 6e4c 6162 4361 6c6c 6261 636b 6020 616e  nLabCallback` an
-00005c60: 6420 7061 7373 2069 7420 696e 746f 2074  d pass it into t
-00005c70: 6865 2060 6361 6c6c 6261 636b 7360 2070  he `callbacks` p
-00005c80: 6172 616d 6574 6572 206f 6620 6054 7261  arameter of `Tra
-00005c90: 696e 6572 6020 746f 2065 6e61 626c 6520  iner` to enable 
-00005ca0: 5377 616e 4c61 6220 746f 0a72 6563 6f72  SwanLab to.recor
-00005cb0: 6420 7472 6169 6e69 6e67 206d 6574 7269  d training metri
-00005cc0: 6373 2e0a 0a60 6060 7079 7468 6f6e 0a69  cs...```python.i
-00005cd0: 6d70 6f72 7420 6576 616c 7561 7465 0a69  mport evaluate.i
-00005ce0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-00005cf0: 700a 696d 706f 7274 2073 7761 6e6c 6162  p.import swanlab
-00005d00: 0a66 726f 6d20 7377 616e 6c61 622e 696e  .from swanlab.in
-00005d10: 7465 6772 6174 696f 6e2e 6875 6767 696e  tegration.huggin
-00005d20: 6766 6163 6520 696d 706f 7274 2053 7761  gface import Swa
-00005d30: 6e4c 6162 4361 6c6c 6261 636b 0a66 726f  nLabCallback.fro
-00005d40: 6d20 6461 7461 7365 7473 2069 6d70 6f72  m datasets impor
-00005d50: 7420 6c6f 6164 5f64 6174 6173 6574 0a66  t load_dataset.f
-00005d60: 726f 6d20 7472 616e 7366 6f72 6d65 7273  rom transformers
-00005d70: 2069 6d70 6f72 7420 4175 746f 4d6f 6465   import AutoMode
-00005d80: 6c46 6f72 5365 7175 656e 6365 436c 6173  lForSequenceClas
-00005d90: 7369 6669 6361 7469 6f6e 2c20 4175 746f  sification, Auto
-00005da0: 546f 6b65 6e69 7a65 722c 2054 7261 696e  Tokenizer, Train
-00005db0: 6572 2c20 5472 6169 6e69 6e67 4172 6775  er, TrainingArgu
-00005dc0: 6d65 6e74 730a 0a0a 6465 6620 746f 6b65  ments...def toke
-00005dd0: 6e69 7a65 5f66 756e 6374 696f 6e28 6578  nize_function(ex
-00005de0: 616d 706c 6573 293a 0a20 2020 2072 6574  amples):.    ret
-00005df0: 7572 6e20 746f 6b65 6e69 7a65 7228 6578  urn tokenizer(ex
-00005e00: 616d 706c 6573 5b22 7465 7874 225d 2c20  amples["text"], 
-00005e10: 7061 6464 696e 673d 226d 6178 5f6c 656e  padding="max_len
-00005e20: 6774 6822 2c20 7472 756e 6361 7469 6f6e  gth", truncation
-00005e30: 3d54 7275 6529 0a0a 0a64 6566 2063 6f6d  =True)...def com
-00005e40: 7075 7465 5f6d 6574 7269 6373 2865 7661  pute_metrics(eva
-00005e50: 6c5f 7072 6564 293a 0a20 2020 206c 6f67  l_pred):.    log
-00005e60: 6974 732c 206c 6162 656c 7320 3d20 6576  its, labels = ev
-00005e70: 616c 5f70 7265 640a 2020 2020 7072 6564  al_pred.    pred
-00005e80: 6963 7469 6f6e 7320 3d20 6e70 2e61 7267  ictions = np.arg
-00005e90: 6d61 7828 6c6f 6769 7473 2c20 6178 6973  max(logits, axis
-00005ea0: 3d2d 3129 0a20 2020 2072 6574 7572 6e20  =-1).    return 
-00005eb0: 6d65 7472 6963 2e63 6f6d 7075 7465 2870  metric.compute(p
-00005ec0: 7265 6469 6374 696f 6e73 3d70 7265 6469  redictions=predi
-00005ed0: 6374 696f 6e73 2c20 7265 6665 7265 6e63  ctions, referenc
-00005ee0: 6573 3d6c 6162 656c 7329 0a0a 0a64 6174  es=labels)...dat
-00005ef0: 6173 6574 203d 206c 6f61 645f 6461 7461  aset = load_data
-00005f00: 7365 7428 2279 656c 705f 7265 7669 6577  set("yelp_review
-00005f10: 5f66 756c 6c22 290a 0a74 6f6b 656e 697a  _full")..tokeniz
-00005f20: 6572 203d 2041 7574 6f54 6f6b 656e 697a  er = AutoTokeniz
-00005f30: 6572 2e66 726f 6d5f 7072 6574 7261 696e  er.from_pretrain
-00005f40: 6564 2822 6265 7274 2d62 6173 652d 6361  ed("bert-base-ca
-00005f50: 7365 6422 290a 0a74 6f6b 656e 697a 6564  sed")..tokenized
-00005f60: 5f64 6174 6173 6574 7320 3d20 6461 7461  _datasets = data
-00005f70: 7365 742e 6d61 7028 746f 6b65 6e69 7a65  set.map(tokenize
-00005f80: 5f66 756e 6374 696f 6e2c 2062 6174 6368  _function, batch
-00005f90: 6564 3d54 7275 6529 0a0a 736d 616c 6c5f  ed=True)..small_
-00005fa0: 7472 6169 6e5f 6461 7461 7365 7420 3d20  train_dataset = 
-00005fb0: 746f 6b65 6e69 7a65 645f 6461 7461 7365  tokenized_datase
-00005fc0: 7473 5b22 7472 6169 6e22 5d2e 7368 7566  ts["train"].shuf
-00005fd0: 666c 6528 7365 6564 3d34 3229 2e73 656c  fle(seed=42).sel
-00005fe0: 6563 7428 7261 6e67 6528 3130 3030 2929  ect(range(1000))
-00005ff0: 0a73 6d61 6c6c 5f65 7661 6c5f 6461 7461  .small_eval_data
-00006000: 7365 7420 3d20 746f 6b65 6e69 7a65 645f  set = tokenized_
-00006010: 6461 7461 7365 7473 5b22 7465 7374 225d  datasets["test"]
-00006020: 2e73 6875 6666 6c65 2873 6565 643d 3432  .shuffle(seed=42
-00006030: 292e 7365 6c65 6374 2872 616e 6765 2831  ).select(range(1
-00006040: 3030 3029 290a 0a6d 6574 7269 6320 3d20  000))..metric = 
-00006050: 6576 616c 7561 7465 2e6c 6f61 6428 2261  evaluate.load("a
-00006060: 6363 7572 6163 7922 290a 0a6d 6f64 656c  ccuracy")..model
-00006070: 203d 2041 7574 6f4d 6f64 656c 466f 7253   = AutoModelForS
-00006080: 6571 7565 6e63 6543 6c61 7373 6966 6963  equenceClassific
-00006090: 6174 696f 6e2e 6672 6f6d 5f70 7265 7472  ation.from_pretr
-000060a0: 6169 6e65 6428 2262 6572 742d 6261 7365  ained("bert-base
-000060b0: 2d63 6173 6564 222c 206e 756d 5f6c 6162  -cased", num_lab
-000060c0: 656c 733d 3529 0a0a 7472 6169 6e69 6e67  els=5)..training
-000060d0: 5f61 7267 7320 3d20 5472 6169 6e69 6e67  _args = Training
-000060e0: 4172 6775 6d65 6e74 7328 0a20 2020 206f  Arguments(.    o
-000060f0: 7574 7075 745f 6469 723d 2274 6573 745f  utput_dir="test_
-00006100: 7472 6169 6e65 7222 2c0a 2020 2020 7265  trainer",.    re
-00006110: 706f 7274 5f74 6f3d 226e 6f6e 6522 2c0a  port_to="none",.
-00006120: 2020 2020 6e75 6d5f 7472 6169 6e5f 6570      num_train_ep
-00006130: 6f63 6873 3d33 2c0a 2020 2020 6c6f 6767  ochs=3,.    logg
-00006140: 696e 675f 7374 6570 733d 3530 2c0a 290a  ing_steps=50,.).
-00006150: 0a73 7761 6e6c 6162 5f63 616c 6c62 6163  .swanlab_callbac
-00006160: 6b20 3d20 5377 616e 4c61 6243 616c 6c62  k = SwanLabCallb
-00006170: 6163 6b28 6578 7065 7269 6d65 6e74 5f6e  ack(experiment_n
-00006180: 616d 653d 2254 7261 6e73 666f 726d 6572  ame="Transformer
-00006190: 7354 6573 7422 2c20 636c 6f75 643d 4661  sTest", cloud=Fa
-000061a0: 6c73 6529 0a0a 7472 6169 6e65 7220 3d20  lse)..trainer = 
-000061b0: 5472 6169 6e65 7228 0a20 2020 206d 6f64  Trainer(.    mod
-000061c0: 656c 3d6d 6f64 656c 2c0a 2020 2020 6172  el=model,.    ar
-000061d0: 6773 3d74 7261 696e 696e 675f 6172 6773  gs=training_args
-000061e0: 2c0a 2020 2020 7472 6169 6e5f 6461 7461  ,.    train_data
-000061f0: 7365 743d 736d 616c 6c5f 7472 6169 6e5f  set=small_train_
-00006200: 6461 7461 7365 742c 0a20 2020 2065 7661  dataset,.    eva
-00006210: 6c5f 6461 7461 7365 743d 736d 616c 6c5f  l_dataset=small_
-00006220: 6576 616c 5f64 6174 6173 6574 2c0a 2020  eval_dataset,.  
-00006230: 2020 636f 6d70 7574 655f 6d65 7472 6963    compute_metric
-00006240: 733d 636f 6d70 7574 655f 6d65 7472 6963  s=compute_metric
-00006250: 732c 0a20 2020 2063 616c 6c62 6163 6b73  s,.    callbacks
-00006260: 3d5b 7377 616e 6c61 625f 6361 6c6c 6261  =[swanlab_callba
-00006270: 636b 5d2c 0a29 0a0a 7472 6169 6e65 722e  ck],.)..trainer.
-00006280: 7472 6169 6e28 290a 6060 600a 0a3c 2f64  train().```..</d
-00006290: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
-000062a0: 733e 0a3c 7375 6d6d 6172 793e 0a20 203c  s>.<summary>.  <
-000062b0: 7374 726f 6e67 3e20 4d4d 456e 6769 6e65  strong> MMEngine
-000062c0: 284d 4d44 6574 6563 7469 6f6e 2065 7463  (MMDetection etc
-000062d0: 2e29 3c2f 7374 726f 6e67 3e0a 3c2f 7375  .)</strong>.</su
-000062e0: 6d6d 6172 793e 0a3c 6272 3e0a 0a49 6e74  mmary>.<br>..Int
-000062f0: 6567 7261 7465 2060 5377 616e 6c61 6256  egrate `SwanlabV
-00006300: 6973 4261 636b 656e 6460 2069 6e74 6f20  isBackend` into 
-00006310: 4d4d 456e 6769 6e65 2074 6f20 656e 6162  MMEngine to enab
-00006320: 6c65 2061 7574 6f6d 6174 6963 206c 6f67  le automatic log
-00006330: 6769 6e67 206f 6620 7472 6169 6e69 6e67  ging of training
-00006340: 206d 6574 7269 6373 2062 7920 5377 616e   metrics by Swan
-00006350: 4c61 622e 0a0a 4164 6420 7468 6520 666f  Lab...Add the fo
-00006360: 6c6c 6f77 696e 6720 636f 6465 2073 6e69  llowing code sni
-00006370: 7070 6574 2074 6f20 796f 7572 204d 4d20  ppet to your MM 
-00006380: 636f 6e66 6967 2066 696c 6520 746f 2073  config file to s
-00006390: 7461 7274 2074 7261 696e 696e 673a 0a0a  tart training:..
-000063a0: 6060 6070 7974 686f 6e0a 6375 7374 6f6d  ```python.custom
-000063b0: 5f69 6d70 6f72 7473 203d 2064 6963 7428  _imports = dict(
-000063c0: 696d 706f 7274 733d 5b22 7377 616e 6c61  imports=["swanla
-000063d0: 622e 696e 7465 6772 6174 696f 6e2e 6d6d  b.integration.mm
-000063e0: 656e 6769 6e65 225d 2c20 616c 6c6f 775f  engine"], allow_
-000063f0: 6661 696c 6564 5f69 6d70 6f72 7473 3d46  failed_imports=F
-00006400: 616c 7365 290a 0a76 6973 5f62 6163 6b65  alse)..vis_backe
-00006410: 6e64 7320 3d20 5b0a 2020 2020 6469 6374  nds = [.    dict
-00006420: 280a 2020 2020 2020 2020 7479 7065 3d22  (.        type="
-00006430: 5377 616e 6c61 6256 6973 4261 636b 656e  SwanlabVisBacken
-00006440: 6422 2c0a 2020 2020 2020 2020 7361 7665  d",.        save
-00006450: 5f64 6972 3d22 7275 6e73 2f73 7761 6e6c  _dir="runs/swanl
-00006460: 6162 222c 0a20 2020 2020 2020 2069 6e69  ab",.        ini
-00006470: 745f 6b77 6172 6773 3d7b 0a20 2020 2020  t_kwargs={.     
-00006480: 2020 2020 2020 2022 7072 6f6a 6563 7422         "project"
-00006490: 3a20 2273 7761 6e6c 6162 2d6d 6d65 6e67  : "swanlab-mmeng
-000064a0: 696e 6522 2c0a 2020 2020 2020 2020 7d2c  ine",.        },
-000064b0: 0a20 2020 2029 2c0a 5d0a 0a76 6973 7561  .    ),.]..visua
-000064c0: 6c69 7a65 7220 3d20 6469 6374 280a 2020  lizer = dict(.  
-000064d0: 2020 7479 7065 3d22 5669 7375 616c 697a    type="Visualiz
-000064e0: 6572 222c 0a20 2020 2076 6973 5f62 6163  er",.    vis_bac
-000064f0: 6b65 6e64 733d 7669 735f 6261 636b 656e  kends=vis_backen
-00006500: 6473 2c0a 290a 6060 600a 3c2f 6465 7461  ds,.).```.</deta
-00006510: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
-00006520: 3c73 756d 6d61 7279 3e0a 2020 3c73 7472  <summary>.  <str
-00006530: 6f6e 673e 2055 6c74 7261 6c79 7469 6373  ong> Ultralytics
-00006540: 3c2f 7374 726f 6e67 3e0a 3c2f 7375 6d6d  </strong>.</summ
-00006550: 6172 793e 0a3c 6272 3e0a 0a49 6e74 6567  ary>.<br>..Integ
-00006560: 7261 7469 6e67 2053 7761 6e4c 6162 2069  rating SwanLab i
-00006570: 6e74 6f20 556c 7472 616c 7974 6963 7320  nto Ultralytics 
-00006580: 6973 2076 6572 7920 7369 6d70 6c65 3b20  is very simple; 
-00006590: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-000065a0: 6061 6464 5f73 7761 6e6c 6162 5f63 616c  `add_swanlab_cal
-000065b0: 6c62 6163 6b60 2066 756e 6374 696f 6e3a  lback` function:
-000065c0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-000065d0: 2075 6c74 7261 6c79 7469 6373 2069 6d70   ultralytics imp
-000065e0: 6f72 7420 594f 4c4f 0a66 726f 6d20 7377  ort YOLO.from sw
-000065f0: 616e 6c61 622e 696e 7465 6772 6174 696f  anlab.integratio
-00006600: 6e2e 756c 7472 616c 7974 6963 7320 696d  n.ultralytics im
-00006610: 706f 7274 2061 6464 5f73 7761 6e6c 6162  port add_swanlab
-00006620: 5f63 616c 6c62 6163 6b0a 0a6d 6f64 656c  _callback..model
-00006630: 203d 2059 4f4c 4f28 2279 6f6c 6f76 386e   = YOLO("yolov8n
-00006640: 2e79 616d 6c22 290a 6d6f 6465 6c2e 6c6f  .yaml").model.lo
-00006650: 6164 2829 0a0a 6164 645f 7377 616e 6c61  ad()..add_swanla
-00006660: 625f 6361 6c6c 6261 636b 286d 6f64 656c  b_callback(model
-00006670: 290a 0a6d 6f64 656c 2e74 7261 696e 280a  )..model.train(.
-00006680: 2020 2020 6461 7461 3d22 2e2f 636f 636f      data="./coco
-00006690: 2e79 616d 6c22 2c0a 2020 2020 6570 6f63  .yaml",.    epoc
-000066a0: 6873 3d35 302c 200a 2020 2020 696d 6773  hs=50, .    imgs
-000066b0: 7a3d 3332 302c 0a29 0a60 6060 0a0a 3c2f  z=320,.).```..</
-000066c0: 6465 7461 696c 733e 0a0a 0a0a 3c62 723e  details>....<br>
-000066d0: 0a0a 2323 20f0 9f86 9a20 436f 6d70 6172  ..## .... Compar
-000066e0: 6973 6f6e 2077 6974 6820 6661 6d69 6c69  ison with famili
-000066f0: 6172 2074 6f6f 6c73 0a0a 2323 2320 5465  ar tools..### Te
-00006700: 6e73 6f72 626f 6172 6420 7673 2053 7761  nsorboard vs Swa
-00006710: 6e4c 6162 0a0a 2d20 2a2a e298 81ef b88f  nLab..- **......
-00006720: 204f 6e6c 696e 6520 5573 6167 6520 5375   Online Usage Su
-00006730: 7070 6f72 742a 2a3a 0a20 2057 6974 6820  pport**:.  With 
-00006740: 5377 616e 4c61 622c 2074 7261 696e 696e  SwanLab, trainin
-00006750: 6720 6578 7065 7269 6d65 6e74 7320 6361  g experiments ca
-00006760: 6e20 6265 2063 6f6e 7665 6e69 656e 746c  n be convenientl
-00006770: 7920 7379 6e63 6872 6f6e 697a 6564 2061  y synchronized a
-00006780: 6e64 2073 6176 6564 2069 6e20 7468 6520  nd saved in the 
-00006790: 636c 6f75 642c 2061 6c6c 6f77 696e 6720  cloud, allowing 
-000067a0: 666f 7220 7265 6d6f 7465 0a20 206d 6f6e  for remote.  mon
-000067b0: 6974 6f72 696e 6720 6f66 2074 7261 696e  itoring of train
-000067c0: 696e 6720 7072 6f67 7265 7373 2c20 6d61  ing progress, ma
-000067d0: 6e61 6769 6e67 2068 6973 746f 7269 6361  naging historica
-000067e0: 6c20 7072 6f6a 6563 7473 2c20 7368 6172  l projects, shar
-000067f0: 696e 6720 6578 7065 7269 6d65 6e74 206c  ing experiment l
-00006800: 696e 6b73 2c20 7365 6e64 696e 6720 7265  inks, sending re
-00006810: 616c 2d74 696d 650a 2020 6e6f 7469 6669  al-time.  notifi
-00006820: 6361 7469 6f6e 206d 6573 7361 6765 732c  cation messages,
-00006830: 2061 6e64 2076 6965 7769 6e67 2065 7870   and viewing exp
-00006840: 6572 696d 656e 7473 2061 6372 6f73 7320  eriments across 
-00006850: 6d75 6c74 6970 6c65 2064 6576 6963 6573  multiple devices
-00006860: 2e20 496e 2063 6f6e 7472 6173 742c 2054  . In contrast, T
-00006870: 656e 736f 7242 6f61 7264 2069 7320 616e  ensorBoard is an
-00006880: 206f 6666 6c69 6e65 0a20 2065 7870 6572   offline.  exper
-00006890: 696d 656e 7420 7472 6163 6b69 6e67 2074  iment tracking t
-000068a0: 6f6f 6c2e 0a0a 2d20 2a2a f09f 91a5 2043  ool...- **.... C
-000068b0: 6f6c 6c61 626f 7261 7469 7665 204d 756c  ollaborative Mul
-000068c0: 7469 2d75 7365 7220 456e 7669 726f 6e6d  ti-user Environm
-000068d0: 656e 742a 2a3a 0a20 2053 7761 6e4c 6162  ent**:.  SwanLab
-000068e0: 2066 6163 696c 6974 6174 6573 2065 6173   facilitates eas
-000068f0: 7920 6d61 6e61 6765 6d65 6e74 206f 6620  y management of 
-00006900: 6d75 6c74 692d 7065 7273 6f6e 2074 7261  multi-person tra
-00006910: 696e 696e 6720 7072 6f6a 6563 7473 2061  ining projects a
-00006920: 6e64 2073 6861 7269 6e67 206f 6620 6578  nd sharing of ex
-00006930: 7065 7269 6d65 6e74 206c 696e 6b73 2066  periment links f
-00006940: 6f72 0a20 2063 6f6c 6c61 626f 7261 7469  or.  collaborati
-00006950: 7665 206d 6163 6869 6e65 206c 6561 726e  ve machine learn
-00006960: 696e 6720 6163 726f 7373 2074 6561 6d73  ing across teams
-00006970: 2e20 4974 2061 6c73 6f20 656e 6162 6c65  . It also enable
-00006980: 7320 6372 6f73 732d 7370 6163 6520 636f  s cross-space co
-00006990: 6d6d 756e 6963 6174 696f 6e20 616e 6420  mmunication and 
-000069a0: 6469 7363 7573 7369 6f6e 2e20 4f6e 2074  discussion. On t
-000069b0: 6865 206f 7468 6572 0a20 2068 616e 642c  he other.  hand,
-000069c0: 2054 656e 736f 7242 6f61 7264 2069 7320   TensorBoard is 
-000069d0: 7072 696d 6172 696c 7920 6465 7369 676e  primarily design
-000069e0: 6564 2066 6f72 2069 6e64 6976 6964 7561  ed for individua
-000069f0: 6c20 7573 652c 206d 616b 696e 6720 6974  l use, making it
-00006a00: 2064 6966 6669 6375 6c74 2074 6f20 636f   difficult to co
-00006a10: 6c6c 6162 6f72 6174 6520 616e 6420 7368  llaborate and sh
-00006a20: 6172 6520 6578 7065 7269 6d65 6e74 730a  are experiments.
-00006a30: 2020 7769 7468 206d 756c 7469 706c 6520    with multiple 
-00006a40: 7573 6572 732e 0a0a 2d20 2a2a f09f 92bb  users...- **....
-00006a50: 2050 6572 7369 7374 656e 742c 2043 656e   Persistent, Cen
-00006a60: 7472 616c 697a 6564 2044 6173 6862 6f61  tralized Dashboa
-00006a70: 7264 2a2a 3a0a 2020 5265 6761 7264 6c65  rd**:.  Regardle
-00006a80: 7373 206f 6620 7768 6572 6520 796f 7520  ss of where you 
-00006a90: 6172 6520 7472 6169 6e69 6e67 2079 6f75  are training you
-00006aa0: 7220 6d6f 6465 6c73 2c20 6265 2069 7420  r models, be it 
-00006ab0: 6f6e 2061 206c 6f63 616c 2063 6f6d 7075  on a local compu
-00006ac0: 7465 722c 2061 206c 6162 2063 6c75 7374  ter, a lab clust
-00006ad0: 6572 2c20 6f72 206f 6e20 7075 626c 6963  er, or on public
-00006ae0: 2063 6c6f 7564 2047 5055 0a20 2069 6e73   cloud GPU.  ins
-00006af0: 7461 6e63 6573 2c20 796f 7572 2072 6573  tances, your res
-00006b00: 756c 7473 2061 7265 206c 6f67 6765 6420  ults are logged 
-00006b10: 746f 2074 6865 2073 616d 6520 6365 6e74  to the same cent
-00006b20: 7261 6c69 7a65 6420 6461 7368 626f 6172  ralized dashboar
-00006b30: 642e 2055 7369 6e67 2054 656e 736f 7242  d. Using TensorB
-00006b40: 6f61 7264 2c20 6f6e 2074 6865 206f 7468  oard, on the oth
-00006b50: 6572 2068 616e 642c 2072 6571 7569 7265  er hand, require
-00006b60: 730a 2020 7370 656e 6469 6e67 2074 696d  s.  spending tim
-00006b70: 6520 636f 7079 696e 6720 616e 6420 6d61  e copying and ma
-00006b80: 6e61 6769 6e67 2054 4645 7665 6e74 2066  naging TFEvent f
-00006b90: 696c 6573 2066 726f 6d20 6469 6666 6572  iles from differ
-00006ba0: 656e 7420 6d61 6368 696e 6573 2e0a 0a2d  ent machines...-
-00006bb0: 202a 2af0 9f92 aa20 4d6f 7265 2050 6f77   **.... More Pow
-00006bc0: 6572 6675 6c20 5461 626c 6573 2a2a 3a0a  erful Tables**:.
-00006bd0: 2020 5377 616e 4c61 6220 7461 626c 6573    SwanLab tables
-00006be0: 2061 6c6c 6f77 2079 6f75 2074 6f20 7669   allow you to vi
-00006bf0: 6577 2c20 7365 6172 6368 2c20 616e 6420  ew, search, and 
-00006c00: 6669 6c74 6572 2072 6573 756c 7473 2066  filter results f
-00006c10: 726f 6d20 7661 7269 6f75 7320 6578 7065  rom various expe
-00006c20: 7269 6d65 6e74 732c 206d 616b 696e 6720  riments, making 
-00006c30: 6974 2065 6173 7920 746f 2072 6576 6965  it easy to revie
-00006c40: 770a 2020 7468 6f75 7361 6e64 7320 6f66  w.  thousands of
-00006c50: 206d 6f64 656c 2076 6572 7369 6f6e 7320   model versions 
-00006c60: 746f 2066 696e 6420 7468 6520 6265 7374  to find the best
-00006c70: 2d70 6572 666f 726d 696e 6720 6d6f 6465  -performing mode
-00006c80: 6c73 2066 6f72 2064 6966 6665 7265 6e74  ls for different
-00006c90: 2074 6173 6b73 2e20 5465 6e73 6f72 426f   tasks. TensorBo
-00006ca0: 6172 6420 6973 206e 6f74 2077 656c 6c2d  ard is not well-
-00006cb0: 7375 6974 6564 2066 6f72 0a20 206c 6172  suited for.  lar
-00006cc0: 6765 2d73 6361 6c65 2070 726f 6a65 6374  ge-scale project
-00006cd0: 732e 0a0a 2323 2320 5765 6967 6874 7320  s...### Weights 
-00006ce0: 616e 6420 4269 6173 6573 2076 7320 5377  and Biases vs Sw
-00006cf0: 616e 4c61 620a 0a2d 2057 6569 6768 7473  anLab..- Weights
-00006d00: 2061 6e64 2042 6961 7365 7320 6973 2061   and Biases is a
-00006d10: 6e20 6f6e 6c69 6e65 2d6f 6e6c 792c 2070  n online-only, p
-00006d20: 726f 7072 6965 7461 7279 204d 4c4f 7073  roprietary MLOps
-00006d30: 2070 6c61 7466 6f72 6d2e 0a0a 2d20 4e6f   platform...- No
-00006d40: 7420 6f6e 6c79 2064 6f65 7320 5377 616e  t only does Swan
-00006d50: 4c61 6220 7375 7070 6f72 7420 6f6e 6c69  Lab support onli
-00006d60: 6e65 2075 7361 6765 2c20 6275 7420 6974  ne usage, but it
-00006d70: 2061 6c73 6f20 6f66 6665 7273 2061 6e20   also offers an 
-00006d80: 6f70 656e 2d73 6f75 7263 652c 2066 7265  open-source, fre
-00006d90: 652c 2061 6e64 2073 656c 662d 686f 7374  e, and self-host
-00006da0: 6564 2076 6572 7369 6f6e 2e0a 0a3c 6272  ed version...<br
-00006db0: 3e0a 0a23 2320 f09f 9ba3 efb8 8f20 526f  >..## ....... Ro
-00006dc0: 6164 6d61 700a 0a54 6f6f 6c73 2065 766f  admap..Tools evo
-00006dd0: 6c76 6520 696e 2069 7465 7261 7469 6f6e  lve in iteration
-00006de0: 2061 6e64 2066 6565 6462 6163 6b7e 2c20   and feedback~, 
-00006df0: 7765 6c63 6f6d 650a 746f 205b 7375 626d  welcome.to [subm
-00006e00: 6974 2066 6561 7475 7265 2073 7567 6765  it feature sugge
-00006e10: 7374 696f 6e73 5d28 6874 7470 733a 2f2f  stions](https://
-00006e20: 6765 656b 7465 6368 7374 7564 696f 2e66  geektechstudio.f
-00006e30: 6569 7368 752e 636e 2f73 6861 7265 2f62  eishu.cn/share/b
-00006e40: 6173 652f 666f 726d 2f73 6872 636e 7942  ase/form/shrcnyB
-00006e50: 6c4b 384f 4d44 3065 7765 6f46 6363 3253  lK8OMD0eweoFcc2S
-00006e60: 7657 4b63 290a 0a23 2323 2049 6e20 5072  vWKc)..### In Pr
-00006e70: 6f67 7265 7373 204e 6f77 0a0a 2d20 6054  ogress Now..- `T
-00006e80: 6162 6c65 603a 204d 6f72 6520 666c 6578  able`: More flex
-00006e90: 6962 6c65 206d 756c 7469 6469 6d65 6e73  ible multidimens
-00006ea0: 696f 6e61 6c20 7461 626c 6520 6368 6172  ional table char
-00006eb0: 7473 2c20 7375 6974 6162 6c65 2066 6f72  ts, suitable for
-00006ec0: 204c 4c4d 2c20 4149 4743 2c20 6d6f 6465   LLM, AIGC, mode
-00006ed0: 6c20 6576 616c 7561 7469 6f6e 2061 6e64  l evaluation and
-00006ee0: 206f 7468 6572 2073 6365 6e61 7269 6f73   other scenarios
-00006ef0: 2e0a 0a2d 202a 2a45 6d61 696c 206e 6f74  ...- **Email not
-00006f00: 6966 6963 6174 696f 6ef0 9f93 a72a 2a3a  ification....**:
-00006f10: 2057 6865 6e20 7472 6169 6e69 6e67 2069   When training i
-00006f20: 7320 696e 7465 7272 7570 7465 6420 756e  s interrupted un
-00006f30: 6578 7065 6374 6564 6c79 2c20 7768 656e  expectedly, when
-00006f40: 2074 7261 696e 696e 6720 6973 2063 6f6d   training is com
-00006f50: 706c 6574 6564 2c20 616e 6420 7768 656e  pleted, and when
-00006f60: 2063 7573 746f 6d0a 2020 7369 7475 6174   custom.  situat
-00006f70: 696f 6e73 206f 6363 7572 2c20 7365 6e64  ions occur, send
-00006f80: 206e 6f74 6966 6963 6174 696f 6e20 656d   notification em
-00006f90: 6169 6c73 2e0a 0a23 2323 204e 6578 7420  ails...### Next 
-00006fa0: 506c 616e 6e65 640a 0a2d 2060 4d6f 6c65  Planned..- `Mole
-00006fb0: 6375 6c65 603a 2056 6973 7561 6c69 7a61  cule`: Visualiza
-00006fc0: 7469 6f6e 2063 6861 7274 7320 6f66 2062  tion charts of b
-00006fd0: 696f 6368 656d 6973 7472 7920 6d6f 6c65  iochemistry mole
-00006fe0: 6375 6c65 730a 0a2d 2060 506c 6f74 603a  cules..- `Plot`:
-00006ff0: 2046 7265 6520 6368 6172 7420 6472 6177   Free chart draw
-00007000: 696e 6720 6d65 7468 6f64 0a0a 2d20 6041  ing method..- `A
-00007010: 7069 603a 2041 6363 6573 7320 5377 616e  pi`: Access Swan
-00007020: 4c61 6220 6461 7461 2074 6872 6f75 6768  Lab data through
-00007030: 2041 5049 2e0a 0a2d 202a 2a53 7973 7465   API...- **Syste
-00007040: 6d20 6861 7264 7761 7265 2072 6563 6f72  m hardware recor
-00007050: 6473 2a2a 3a20 5265 636f 7264 2061 2073  ds**: Record a s
-00007060: 6572 6965 7320 6f66 2068 6172 6477 6172  eries of hardwar
-00007070: 6520 636f 6e64 6974 696f 6e73 2073 7563  e conditions suc
-00007080: 6820 6173 2047 5055 2c20 4350 552c 2064  h as GPU, CPU, d
-00007090: 6973 6b2c 206e 6574 776f 726b 2c20 6574  isk, network, et
-000070a0: 632e 0a0a 2d20 2a2a 436f 6465 2072 6563  c...- **Code rec
-000070b0: 6f72 6473 2a2a 3a20 5265 636f 7264 2074  ords**: Record t
-000070c0: 7261 696e 696e 6720 636f 6465 0a0a 2d20  raining code..- 
-000070d0: 2a2a 4d6f 7265 2069 6e74 6567 7261 7469  **More integrati
-000070e0: 6f6e 732a 2a3a 204c 6967 6874 4742 4d2c  ons**: LightGBM,
-000070f0: 2058 4742 6f6f 7374 2c20 6f70 656e 6169   XGBoost, openai
-00007100: 2c20 6368 6174 676c 6d2c 206d 6d20 7365  , chatglm, mm se
-00007110: 7269 6573 2c2e 2e2e 0a2d 202e 2e2e 0a0a  ries,....- .....
-00007120: 2323 2320 4c6f 6e67 2d74 6572 6d20 436f  ### Long-term Co
-00007130: 6e63 6572 6e0a 0a2d 2054 6865 206d 6f73  ncern..- The mos
-00007140: 7420 6265 6e65 6669 6369 616c 2063 6f6c  t beneficial col
-00007150: 6c61 626f 7261 7469 7665 2077 6179 2066  laborative way f
-00007160: 6f72 2041 4920 7465 616d 2069 6e6e 6f76  or AI team innov
-00007170: 6174 696f 6e0a 0a2d 2054 6865 206d 6f73  ation..- The mos
-00007180: 7420 7573 6572 2d66 7269 656e 646c 7920  t user-friendly 
-00007190: 5549 2069 6e74 6572 6163 7469 6f6e 0a0a  UI interaction..
-000071a0: 2d20 5669 6577 696e 6720 6578 7065 7269  - Viewing experi
-000071b0: 6d65 6e74 7320 6f6e 206d 6f62 696c 650a  ments on mobile.
-000071c0: 0a3c 6272 3e0a 0a23 2320 f09f 91a5 2043  .<br>..## .... C
-000071d0: 6f6d 6d75 6e69 7479 0a0a 2323 2320 436f  ommunity..### Co
-000071e0: 6d6d 756e 6974 7920 616e 6420 7375 7070  mmunity and supp
-000071f0: 6f72 740a 0a2d 205b 4769 7448 7562 2049  ort..- [GitHub I
-00007200: 7373 7565 735d 2868 7474 7073 3a2f 2f67  ssues](https://g
-00007210: 6974 6875 622e 636f 6d2f 5377 616e 4875  ithub.com/SwanHu
-00007220: 6258 2f53 7761 6e4c 6162 2f69 7373 7565  bX/SwanLab/issue
-00007230: 7329 efbc 9a45 7272 6f72 7320 616e 6420  s)...Errors and 
-00007240: 6973 7375 6573 2065 6e63 6f75 6e74 6572  issues encounter
-00007250: 6564 2077 6865 6e20 7573 696e 6720 5377  ed when using Sw
-00007260: 616e 4c61 620a 2d20 5b45 6d61 696c 2073  anLab.- [Email s
-00007270: 7570 706f 7274 5d28 7a65 7969 2e6c 696e  upport](zeyi.lin
-00007280: 4073 7761 6e68 7562 2e63 6f29 efbc 9a46  @swanhub.co)...F
-00007290: 6565 6462 6163 6b20 6f6e 2069 7373 7565  eedback on issue
-000072a0: 7320 7769 7468 2075 7369 6e67 2053 7761  s with using Swa
-000072b0: 6e4c 6162 0a2d 203c 6120 6872 6566 3d22  nLab.- <a href="
-000072c0: 6874 7470 733a 2f2f 6765 656b 7465 6368  https://geektech
-000072d0: 7374 7564 696f 2e66 6569 7368 752e 636e  studio.feishu.cn
-000072e0: 2f77 696b 692f 4e49 5a39 7770 354c 5269  /wiki/NIZ9wp5LRi
-000072f0: 5371 5179 6b69 7a62 4763 567a 554b 6e69  SqQykizbGcVzUKni
-00007300: 6322 3e57 6543 6861 743c 2f61 3eef bc9a  c">WeChat</a>...
-00007310: 4469 7363 7573 7320 6973 7375 6573 2075  Discuss issues u
-00007320: 7369 6e67 2053 7761 6e4c 6162 2c0a 2020  sing SwanLab,.  
-00007330: 7368 6172 6520 7468 6520 6c61 7465 7374  share the latest
-00007340: 2041 4920 7465 6368 6e6f 6c6f 6779 2e0a   AI technology..
-00007350: 0a23 2323 2053 7761 6e4c 6162 2052 4541  .### SwanLab REA
-00007360: 444d 4520 4261 6467 650a 0a49 6620 796f  DME Badge..If yo
-00007370: 7520 6c69 6b65 2074 6f20 7573 6520 5377  u like to use Sw
-00007380: 616e 4c61 6220 696e 2079 6f75 7220 776f  anLab in your wo
-00007390: 726b 2c20 706c 6561 7365 2061 6464 2074  rk, please add t
-000073a0: 6865 2053 7761 6e4c 6162 2062 6164 6765  he SwanLab badge
-000073b0: 2074 6f20 796f 7572 2052 4541 444d 453a   to your README:
-000073c0: 0a0a 5b21 5b73 7761 6e6c 6162 5d28 6874  ..[![swanlab](ht
-000073d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000073e0: 732e 696f 2f62 6164 6765 2f70 6f77 6572  s.io/badge/power
-000073f0: 6564 2532 3062 792d 5377 616e 4c61 622d  ed%20by-SwanLab-
-00007400: 3433 3834 3430 295d 2868 7474 7073 3a2f  438440)](https:/
-00007410: 2f67 6974 6875 622e 636f 6d2f 7377 616e  /github.com/swan
-00007420: 6875 6278 2f73 7761 6e6c 6162 290a 0a60  hubx/swanlab)..`
-00007430: 6060 0a5b 215b 7377 616e 6c61 625d 2868  ``.[![swanlab](h
-00007440: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00007450: 6473 2e69 6f2f 6261 6467 652f 706f 7765  ds.io/badge/powe
-00007460: 7265 6425 3230 6279 2d53 7761 6e4c 6162  red%20by-SwanLab
-00007470: 2d34 3338 3434 3029 5d28 6874 7470 733a  -438440)](https:
-00007480: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7761  //github.com/swa
-00007490: 6e68 7562 782f 7377 616e 6c61 6229 0a60  nhubx/swanlab).`
-000074a0: 6060 0a0a 2323 2320 4369 7469 6e67 2053  ``..### Citing S
-000074b0: 7761 6e4c 6162 2069 6e20 7468 6520 7061  wanLab in the pa
-000074c0: 7065 720a 0a49 6620 796f 7520 6669 6e64  per..If you find
-000074d0: 2053 7761 6e4c 6162 2068 656c 7066 756c   SwanLab helpful
-000074e0: 2066 6f72 2079 6f75 7220 7265 7365 6172   for your resear
-000074f0: 6368 206a 6f75 726e 6579 2c20 706c 6561  ch journey, plea
-00007500: 7365 2063 6f6e 7369 6465 7220 6369 7469  se consider citi
-00007510: 6e67 2069 6e20 7468 6520 666f 6c6c 6f77  ng in the follow
-00007520: 696e 6720 666f 726d 6174 3a0a 0a60 6060  ing format:..```
-00007530: 6269 6274 6578 0a40 736f 6674 7761 7265  bibtex.@software
-00007540: 7b5a 6579 696c 696e 5f53 7761 6e4c 6162  {Zeyilin_SwanLab
-00007550: 5f32 3032 332c 0a20 2061 7574 686f 7220  _2023,.  author 
-00007560: 3d20 7b5a 6579 6920 4c69 6e2c 2053 6861  = {Zeyi Lin, Sha
-00007570: 6f68 6f6e 6720 4368 656e 2c20 4b61 6e67  ohong Chen, Kang
-00007580: 204c 692c 2051 6975 7368 616e 204a 6961   Li, Qiushan Jia
-00007590: 6e67 2c20 5a69 7275 6920 4361 692c 2020  ng, Zirui Cai,  
-000075a0: 4b61 6966 616e 6720 4a69 2061 6e64 207b  Kaifang Ji and {
-000075b0: 5468 6520 5377 616e 4c61 6220 7465 616d  The SwanLab team
-000075c0: 7d7d 2c0a 2020 646f 6920 3d20 7b31 302e  }},.  doi = {10.
-000075d0: 3532 3831 2f7a 656e 6f64 6f2e 3131 3130  5281/zenodo.1110
-000075e0: 3035 3530 7d2c 0a20 206c 6963 656e 7365  0550},.  license
-000075f0: 203d 207b 4170 6163 6865 2d32 2e30 7d2c   = {Apache-2.0},
-00007600: 0a20 2074 6974 6c65 203d 207b 7b53 7761  .  title = {{Swa
-00007610: 6e4c 6162 7d7d 2c0a 2020 7572 6c20 3d20  nLab}},.  url = 
-00007620: 7b68 7474 7073 3a2f 2f67 6974 6875 622e  {https://github.
-00007630: 636f 6d2f 7377 616e 6875 6278 2f73 7761  com/swanhubx/swa
-00007640: 6e6c 6162 7d2c 0a20 2079 6561 7220 3d20  nlab},.  year = 
-00007650: 7b32 3032 337d 0a7d 0a60 6060 0a0a 2323  {2023}.}.```..##
-00007660: 2320 436f 6e74 7269 6275 7465 2074 6f20  # Contribute to 
-00007670: 5377 616e 4c61 620a 0a43 6f6e 7369 6465  SwanLab..Conside
-00007680: 7269 6e67 2063 6f6e 7472 6962 7574 696e  ring contributin
-00007690: 6720 746f 2053 7761 6e4c 6162 3f20 4669  g to SwanLab? Fi
-000076a0: 7273 742c 2070 6c65 6173 6520 7461 6b65  rst, please take
-000076b0: 2073 6f6d 6520 7469 6d65 2074 6f20 7265   some time to re
-000076c0: 6164 0a74 6865 205b 436f 6e74 7269 6275  ad.the [Contribu
-000076d0: 7469 6f6e 2047 7569 6465 6c69 6e65 735d  tion Guidelines]
-000076e0: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
-000076f0: 292e 0a0a 4174 2074 6865 2073 616d 6520  )...At the same 
-00007700: 7469 6d65 2c20 7765 2077 6172 6d6c 7920  time, we warmly 
-00007710: 7765 6c63 6f6d 6520 7375 7070 6f72 7420  welcome support 
-00007720: 666f 7220 5377 616e 4c61 6220 7468 726f  for SwanLab thro
-00007730: 7567 6820 736f 6369 616c 206d 6564 6961  ugh social media
-00007740: 2c20 6576 656e 7473 2c20 616e 6420 636f  , events, and co
-00007750: 6e66 6572 656e 6365 2073 6861 7269 6e67  nference sharing
-00007760: 2e20 5468 616e 6b20 796f 7521 0a0a 3c62  . Thank you!..<b
-00007770: 723e 0a0a 2a2a 436f 6e74 7269 6275 746f  r>..**Contributo
-00007780: 7273 2a2a 0a0a 3c61 2068 7265 663d 2268  rs**..<a href="h
-00007790: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000077a0: 6d2f 7377 616e 6875 6278 2f73 7761 6e6c  m/swanhubx/swanl
-000077b0: 6162 2f67 7261 7068 732f 636f 6e74 7269  ab/graphs/contri
-000077c0: 6275 746f 7273 223e 0a20 203c 696d 6720  butors">.  <img 
-000077d0: 7372 633d 2268 7474 7073 3a2f 2f63 6f6e  src="https://con
-000077e0: 7472 6962 2e72 6f63 6b73 2f69 6d61 6765  trib.rocks/image
-000077f0: 3f72 6570 6f3d 7377 616e 6875 6278 2f73  ?repo=swanhubx/s
-00007800: 7761 6e6c 6162 2220 2f3e 0a3c 2f61 3e0a  wanlab" />.</a>.
-00007810: 0a23 2323 2044 6f77 6e6c 6f61 6420 4963  .### Download Ic
-00007820: 6f6e 0a0a 5b53 7761 6e4c 6162 2d49 636f  on..[SwanLab-Ico
-00007830: 6e2d 5356 475d 2868 7474 7073 3a2f 2f72  n-SVG](https://r
-00007840: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00007850: 7465 6e74 2e63 6f6d 2f53 7761 6e48 7562  tent.com/SwanHub
-00007860: 582f 7377 616e 6c61 622f 6d61 696e 2f72  X/swanlab/main/r
-00007870: 6561 646d 655f 6669 6c65 732f 7377 616e  eadme_files/swan
-00007880: 6c61 622d 6c6f 676f 2e73 7667 290a 0a3c  lab-logo.svg)..<
-00007890: 6272 3e0a 0a23 2320 f09f 9383 204c 6963  br>..## .... Lic
-000078a0: 656e 7365 0a0a 5468 6973 2072 6570 6f73  ense..This repos
-000078b0: 6974 6f72 7920 666f 6c6c 6f77 7320 7468  itory follows th
-000078c0: 6520 5b41 7061 6368 6520 322e 3020 4c69  e [Apache 2.0 Li
-000078d0: 6365 6e73 655d 2868 7474 7073 3a2f 2f67  cense](https://g
-000078e0: 6974 6875 622e 636f 6d2f 5377 616e 4875  ithub.com/SwanHu
-000078f0: 6258 2f53 7761 6e4c 6162 2f62 6c6f 622f  bX/SwanLab/blob/
-00007900: 6d61 696e 2f4c 4943 454e 5345 2920 6f70  main/LICENSE) op
-00007910: 656e 2073 6f75 7263 650a 6c69 6365 6e73  en source.licens
-00007920: 652e 0a                                  e..
+00000000: 215b 4f76 6572 7669 6577 5d28 7265 6164  ![Overview](read
+00000010: 6d65 5f66 696c 6573 2f73 7761 6e6c 6162  me_files/swanlab
+00000020: 2d6f 7665 7276 6965 772d 6e65 772e 706e  -overview-new.pn
+00000030: 6729 0a0a 3c70 2061 6c69 676e 3d22 6365  g)..<p align="ce
+00000040: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
+00000050: 6874 7470 733a 2f2f 7377 616e 6c61 622e  https://swanlab.
+00000060: 636e 223e 5377 616e 4c61 6220 436c 6f75  cn">SwanLab Clou
+00000070: 643c 2f61 3e20 c2b7 203c 6120 6872 6566  d</a> .. <a href
+00000080: 3d22 6874 7470 733a 2f2f 646f 6373 2e73  ="https://docs.s
+00000090: 7761 6e6c 6162 2e63 6e22 3e44 6f63 756d  wanlab.cn">Docum
+000000a0: 656e 743c 2f61 3e20 c2b7 203c 6120 6872  ent</a> .. <a hr
+000000b0: 6566 3d22 6874 7470 733a 2f2f 6765 656b  ef="https://geek
+000000c0: 7465 6368 7374 7564 696f 2e66 6569 7368  techstudio.feish
+000000d0: 752e 636e 2f77 696b 692f 4e49 5a39 7770  u.cn/wiki/NIZ9wp
+000000e0: 354c 5269 5371 5179 6b69 7a62 4763 567a  5LRiSqQykizbGcVz
+000000f0: 554b 6e69 6322 3e57 6543 6861 743c 2f61  UKnic">WeChat</a
+00000100: 3e20 c2b7 203c 6120 6872 6566 3d22 6874  > .. <a href="ht
+00000110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000120: 2f73 7761 6e68 7562 782f 7377 616e 6c61  /swanhubx/swanla
+00000130: 622f 6973 7375 6573 223e 5265 706f 7274  b/issues">Report
+00000140: 2049 7373 7565 3c2f 613e 20c2 b720 3c61   Issue</a> .. <a
+00000150: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000160: 6565 6b74 6563 6873 7475 6469 6f2e 6665  eektechstudio.fe
+00000170: 6973 6875 2e63 6e2f 7368 6172 652f 6261  ishu.cn/share/ba
+00000180: 7365 2f66 6f72 6d2f 7368 7263 6e79 426c  se/form/shrcnyBl
+00000190: 4b38 4f4d 4430 6577 656f 4663 6332 5376  K8OMD0eweoFcc2Sv
+000001a0: 574b 6322 3e46 6565 6462 6163 6b3c 2f61  WKc">Feedback</a
+000001b0: 3e20 c2b7 203c 6120 6872 6566 3d22 6874  > .. <a href="ht
+000001c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001d0: 2f53 7761 6e48 7562 582f 5377 616e 4c61  /SwanHubX/SwanLa
+000001e0: 622f 626c 6f62 2f6d 6169 6e2f 4348 414e  b/blob/main/CHAN
+000001f0: 4745 4c4f 472e 6d64 223e 4368 616e 6765  GELOG.md">Change
+00000200: 6c6f 673c 2f61 3e0a 0a0a 3c2f 703e 0a0a  log</a>...</p>..
+00000210: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000220: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000240: 2f53 7761 6e48 7562 582f 5377 616e 4c61  /SwanHubX/SwanLa
+00000250: 622f 626c 6f62 2f6d 6169 6e2f 4c49 4345  b/blob/main/LICE
+00000260: 4e53 4522 3e3c 696d 6720 7372 633d 2268  NSE"><img src="h
+00000270: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000280: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
+00000290: 656e 7365 2f53 7761 6e48 7562 582f 5377  ense/SwanHubX/Sw
+000002a0: 616e 4c61 622e 7376 673f 636f 6c6f 723d  anLab.svg?color=
+000002b0: 6272 6967 6874 6772 6565 6e22 2061 6c74  brightgreen" alt
+000002c0: 3d22 6c69 6365 6e73 6522 3e3c 2f61 3e0a  ="license"></a>.
+000002d0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000002e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5377  ://github.com/Sw
+000002f0: 616e 4875 6258 2f53 7761 6e4c 6162 2f63  anHubX/SwanLab/c
+00000300: 6f6d 6d69 7473 2f6d 6169 6e22 3e3c 696d  ommits/main"><im
+00000310: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000320: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000330: 7468 7562 2f6c 6173 742d 636f 6d6d 6974  thub/last-commit
+00000340: 2f53 7761 6e48 7562 582f 5377 616e 4c61  /SwanHubX/SwanLa
+00000350: 6222 2061 6c74 3d22 6c69 6365 6e73 6522  b" alt="license"
+00000360: 3e3c 2f61 3e0a 2020 3c61 2068 7265 663d  ></a>.  <a href=
+00000370: 2268 7474 7073 3a2f 2f70 7970 692e 7079  "https://pypi.py
+00000380: 7468 6f6e 2e6f 7267 2f70 7970 692f 7377  thon.org/pypi/sw
+00000390: 616e 6c61 6222 3e3c 696d 6720 7372 633d  anlab"><img src=
+000003a0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000003b0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f73  elds.io/pypi/v/s
+000003c0: 7761 6e6c 6162 3f63 6f6c 6f72 3d6f 7261  wanlab?color=ora
+000003d0: 6e67 6522 2061 6c74 3d20 2f3e 3c2f 613e  nge" alt= /></a>
+000003e0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+000003f0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+00000400: 6f6a 6563 742f 7377 616e 6c61 6222 3e3c  oject/swanlab"><
+00000410: 696d 6720 616c 743d 2270 7970 6920 446f  img alt="pypi Do
+00000420: 776e 6c6f 6164 2220 7372 633d 2268 7474  wnload" src="htt
+00000430: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+00000440: 2e74 6563 682f 6261 6467 652f 7377 616e  .tech/badge/swan
+00000450: 6c61 6222 3e3c 2f61 3e0a 2020 3c61 2068  lab"></a>.  <a h
+00000460: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000470: 6875 622e 636f 6d2f 7377 616e 6875 6278  hub.com/swanhubx
+00000480: 2f73 7761 6e6c 6162 2f69 7373 7565 7322  /swanlab/issues"
+00000490: 3e3c 696d 6720 616c 743d 2269 7373 7565  ><img alt="issue
+000004a0: 7322 2073 7263 3d22 6874 7470 733a 2f2f  s" src="https://
+000004b0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+000004c0: 6974 6875 622f 6973 7375 6573 2f73 7761  ithub/issues/swa
+000004d0: 6e68 7562 782f 7377 616e 6c61 6222 3e3c  nhubx/swanlab"><
+000004e0: 2f61 3e0a 2020 3c62 723e 0a20 203c 6120  /a>.  <br>.  <a 
+000004f0: 6872 6566 3d22 6874 7470 733a 2f2f 7377  href="https://sw
+00000500: 616e 6c61 622e 636e 2220 7461 7267 6574  anlab.cn" target
+00000510: 3d22 5f62 6c61 6e6b 223e 0a20 2020 2020  ="_blank">.     
+00000520: 2020 203c 696d 6720 616c 743d 2253 7461     <img alt="Sta
+00000530: 7469 6320 4261 6467 6522 2073 7263 3d22  tic Badge" src="
+00000540: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000550: 6c64 732e 696f 2f62 6164 6765 2f50 726f  lds.io/badge/Pro
+00000560: 6475 6374 2d53 7761 6e4c 6162 e4ba 91e7  duct-SwanLab....
+00000570: abaf e789 882d 3633 3661 3366 223e 3c2f  .....-636a3f"></
+00000580: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
+00000590: 7470 733a 2f2f 6765 656b 7465 6368 7374  tps://geektechst
+000005a0: 7564 696f 2e66 6569 7368 752e 636e 2f77  udio.feishu.cn/w
+000005b0: 696b 692f 4e49 5a39 7770 354c 5269 5371  iki/NIZ9wp5LRiSq
+000005c0: 5179 6b69 7a62 4763 567a 554b 6e69 6322  QykizbGcVzUKnic"
+000005d0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000005e0: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
+000005f0: 6c74 3d22 5374 6174 6963 2042 6164 6765  lt="Static Badge
+00000600: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000610: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000620: 6467 652f 5765 4368 6174 2de5 beae e4bf  dge/WeChat-.....
+00000630: a12d 3463 6235 3565 223e 3c2f 613e 0a20  .-4cb55e"></a>. 
+00000640: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000650: 2f2f 7777 772e 7869 616f 686f 6e67 7368  //www.xiaohongsh
+00000660: 752e 636f 6d2f 7573 6572 2f70 726f 6669  u.com/user/profi
+00000670: 6c65 2f36 3035 3738 3662 3930 3030 3030  le/605786b900000
+00000680: 3030 3030 3130 3033 6138 3122 2074 6172  00001003a81" tar
+00000690: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
+000006a0: 2020 2020 2020 3c69 6d67 2061 6c74 3d22        <img alt="
+000006b0: 5374 6174 6963 2042 6164 6765 2220 7372  Static Badge" sr
+000006c0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000006d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000006e0: e5b0 8fe7 baa2 e4b9 a62d 4630 3434 3338  .........-F04438
+000006f0: 223e 3c2f 613e 0a0a 3c2f 703e 0a0a 3c64  "></a>..</p>..<d
+00000700: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00000710: 223e 0a20 203c 6120 6872 6566 3d22 2e2f  ">.  <a href="./
+00000720: 5245 4144 4d45 2e6d 6422 3e3c 696d 6720  README.md"><img 
+00000730: 616c 743d 22e8 8bb1 e696 87e6 9687 e6a1  alt="...........
+00000740: a322 2073 7263 3d22 6874 7470 733a 2f2f  ." src="https://
+00000750: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000760: 6164 6765 2f45 6e67 6c69 7368 2d64 3964  adge/English-d9d
+00000770: 3964 3922 3e3c 2f61 3e0a 2020 3c61 2068  9d9"></a>.  <a h
+00000780: 7265 663d 222e 2f52 4541 444d 455f 636e  ref="./README_cn
+00000790: 2e6d 6422 3e3c 696d 6720 616c 743d 22e4  .md"><img alt=".
+000007a0: b8ad e696 87e6 9687 e6a1 a322 2073 7263  ..........." src
+000007b0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000007c0: 6965 6c64 732e 696f 2f62 6164 6765 2fe7  ields.io/badge/.
+000007d0: ae80 e4bd 93e4 b8ad e696 872d 6439 6439  ...........-d9d9
+000007e0: 6439 223e 3c2f 613e 0a3c 2f64 6976 3e0a  d9"></a>.</div>.
+000007f0: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
+00000800: 6172 793e 5461 626c 6520 6f66 2063 6f6e  ary>Table of con
+00000810: 7465 6e74 733c 2f73 756d 6d61 7279 3e0a  tents</summary>.
+00000820: 0a23 2323 2320 544f 430a 0a2d 205b f09f  .#### TOC..- [..
+00000830: 918b f09f 8fbb 2049 6e74 726f 6475 6374  ...... Introduct
+00000840: 696f 6e5d 2823 2d49 6e74 726f 6475 6374  ion](#-Introduct
+00000850: 696f 6e29 0a2d 205b f09f 8f81 2051 7569  ion).- [.... Qui
+00000860: 636b 2053 7461 7274 5d28 23f0 9f8f 812d  ck Start](#....-
+00000870: 7175 6963 6b2d 7374 6172 7429 0a20 2020  quick-start).   
+00000880: 202d 205b 312e 496e 7374 616c 6c61 7469   - [1.Installati
+00000890: 6f6e 5d28 2331 696e 7374 616c 6c61 7469  on](#1installati
+000008a0: 6f6e 290a 2020 2020 2d20 5b32 2e4c 6f67  on).    - [2.Log
+000008b0: 2049 6e20 616e 6420 4765 7420 7468 6520   In and Get the 
+000008c0: 4150 4920 4b65 795d 2823 326c 6f67 2d69  API Key](#2log-i
+000008d0: 6e2d 616e 642d 6765 742d 7468 652d 6170  n-and-get-the-ap
+000008e0: 692d 6b65 7929 0a20 2020 202d 205b 332e  i-key).    - [3.
+000008f0: 496e 7465 6772 6174 6520 5377 616e 4c61  Integrate SwanLa
+00000900: 6220 7769 7468 2059 6f75 7220 436f 6465  b with Your Code
+00000910: 5d28 2333 2d69 6e74 6567 7261 7465 2d73  ](#3-integrate-s
+00000920: 7761 6e6c 6162 2d77 6974 682d 796f 7572  wanlab-with-your
+00000930: 2d63 6f64 6529 0a2d 205b f09f 9383 204d  -code).- [.... M
+00000940: 6f72 6520 4578 616d 706c 6573 5d28 232d  ore Examples](#-
+00000950: 6d6f 7265 2d65 7861 6d70 6c65 7329 0a2d  more-examples).-
+00000960: 205b f09f 92bb 2053 656c 662d 686f 7374   [.... Self-host
+00000970: 6564 5d28 232d 7365 6c66 2d68 6f73 7465  ed](#-self-hoste
+00000980: 6429 0a20 2020 202d 205b 4f66 666c 696e  d).    - [Offlin
+00000990: 6520 4578 7065 7269 6d65 6e74 2054 7261  e Experiment Tra
+000009a0: 636b 696e 675d 2823 6f66 666c 696e 652d  cking](#offline-
+000009b0: 6578 7065 7269 6d65 6e74 2d74 7261 636b  experiment-track
+000009c0: 696e 6729 0a20 2020 202d 205b 4f70 656e  ing).    - [Open
+000009d0: 204f 6666 6c69 6e65 2044 6173 6862 6f61   Offline Dashboa
+000009e0: 7264 5d28 236f 7065 6e2d 6f66 666c 696e  rd](#open-offlin
+000009f0: 652d 626f 6172 6429 0a2d 205b f09f 9a97  e-board).- [....
+00000a00: 2049 6e74 6567 7261 7469 6f6e 5d28 232d   Integration](#-
+00000a10: 696e 7465 6772 6174 696f 6e29 0a2d 205b  integration).- [
+00000a20: f09f 869a 2043 6f6d 7061 7269 736f 6e20  .... Comparison 
+00000a30: 7769 7468 2046 616d 696c 6961 7220 546f  with Familiar To
+00000a40: 6f6c 735d 2823 2d63 6f6d 7061 7269 736f  ols](#-compariso
+00000a50: 6e2d 7769 7468 2d66 616d 696c 6961 722d  n-with-familiar-
+00000a60: 746f 6f6c 7329 0a20 2020 202d 205b 5465  tools).    - [Te
+00000a70: 6e73 6f72 626f 6172 6420 7673 2053 7761  nsorboard vs Swa
+00000a80: 6e4c 6162 5d28 2374 656e 736f 7262 6f61  nLab](#tensorboa
+00000a90: 7264 2d76 732d 7377 616e 6c61 6229 0a20  rd-vs-swanlab). 
+00000aa0: 2020 202d 205b 5765 6967 6874 7320 2620     - [Weights & 
+00000ab0: 4269 6173 6573 2076 7320 5377 616e 4c61  Biases vs SwanLa
+00000ac0: 625d 2823 7765 6967 6874 732d 616e 642d  b](#weights-and-
+00000ad0: 6269 6173 6573 2d76 732d 7377 616e 6c61  biases-vs-swanla
+00000ae0: 6229 0a2d 205b f09f 9ba3 efb8 8f20 526f  b).- [....... Ro
+00000af0: 6164 6d61 705d 2823 2545 4625 4238 2538  admap](#%EF%B8%8
+00000b00: 462d 726f 6164 6d61 7029 0a20 2020 202d  F-roadmap).    -
+00000b10: 205b 496e 2050 726f 6772 6573 7320 4e6f   [In Progress No
+00000b20: 775d 2823 696e 2d70 726f 6772 6573 732d  w](#in-progress-
+00000b30: 6e6f 7729 0a20 2020 202d 205b 4e65 7874  now).    - [Next
+00000b40: 2050 6c61 6e6e 6564 5d28 236e 6578 742d   Planned](#next-
+00000b50: 706c 616e 6e65 6429 0a20 2020 202d 205b  planned).    - [
+00000b60: 4c6f 6e67 2054 6572 6d20 436f 6e63 6572  Long Term Concer
+00000b70: 6e5d 2823 6c6f 6e67 2d74 6572 6d2d 636f  n](#long-term-co
+00000b80: 6e63 6572 6e29 0a2d 205b f09f 91a5 2043  ncern).- [.... C
+00000b90: 6f6d 6d75 6e69 7479 5d28 232d 636f 6d6d  ommunity](#-comm
+00000ba0: 756e 6974 7929 0a20 2020 202d 205b 436f  unity).    - [Co
+00000bb0: 6d6d 756e 6974 7920 616e 6420 5375 7070  mmunity and Supp
+00000bc0: 6f72 745d 2823 636f 6d6d 756e 6974 792d  ort](#community-
+00000bd0: 616e 642d 7375 7070 6f72 7429 0a20 2020  and-support).   
+00000be0: 202d 205b 5377 616e 4c61 6220 5245 4144   - [SwanLab READ
+00000bf0: 4d45 2042 6164 6765 5d28 2373 7761 6e6c  ME Badge](#swanl
+00000c00: 6162 2d72 6561 646d 652d 6261 6467 6529  ab-readme-badge)
+00000c10: 0a20 2020 202d 205b 4369 7469 6e67 2053  .    - [Citing S
+00000c20: 7761 6e4c 6162 2069 6e20 7468 6520 5061  wanLab in the Pa
+00000c30: 7065 725d 2823 6369 7469 6e67 2d73 7761  per](#citing-swa
+00000c40: 6e6c 6162 2d69 6e2d 7468 652d 7061 7065  nlab-in-the-pape
+00000c50: 7229 0a20 2020 202d 205b 436f 6e74 7269  r).    - [Contri
+00000c60: 6275 7465 2074 6f20 5377 616e 4c61 625d  bute to SwanLab]
+00000c70: 2823 636f 6e74 7269 6275 7465 2d74 6f2d  (#contribute-to-
+00000c80: 7377 616e 6c61 6229 0a20 2020 202d 205b  swanlab).    - [
+00000c90: 446f 776e 6c6f 6164 2049 636f 6e5d 2823  Download Icon](#
+00000ca0: 646f 776e 6c6f 6164 2d69 636f 6e29 0a2d  download-icon).-
+00000cb0: 205b f09f 9383 204c 6963 656e 7365 5d28   [.... License](
+00000cc0: 232d 6c69 6365 6e73 6529 0a0a 3c62 722f  #-license)..<br/
+00000cd0: 3e0a 0a3c 2f64 6574 6169 6c73 3e0a 0a23  >..</details>..#
+00000ce0: 2320 f09f 918b f09f 8fbb 2049 6e74 726f  # ........ Intro
+00000cf0: 6475 6374 696f 6e0a 0a53 7761 6e4c 6162  duction..SwanLab
+00000d00: 2069 7320 616e 206f 7065 6e2d 736f 7572   is an open-sour
+00000d10: 6365 2c20 6c69 6768 7477 6569 6768 7420  ce, lightweight 
+00000d20: 4149 2065 7870 6572 696d 656e 7420 7472  AI experiment tr
+00000d30: 6163 6b69 6e67 2074 6f6f 6c20 7468 6174  acking tool that
+00000d40: 2070 726f 7669 6465 7320 6120 706c 6174   provides a plat
+00000d50: 666f 726d 2066 6f72 2074 7261 636b 696e  form for trackin
+00000d60: 672c 2063 6f6d 7061 7269 6e67 2c20 616e  g, comparing, an
+00000d70: 640a 636f 6c6c 6162 6f72 6174 696e 6720  d.collaborating 
+00000d80: 6f6e 2065 7870 6572 696d 656e 7473 2c20  on experiments, 
+00000d90: 6169 6d69 6e67 2074 6f20 6163 6365 6c65  aiming to accele
+00000da0: 7261 7465 2074 6865 2072 6573 6561 7263  rate the researc
+00000db0: 6820 616e 6420 6465 7665 6c6f 706d 656e  h and developmen
+00000dc0: 7420 6566 6669 6369 656e 6379 206f 6620  t efficiency of 
+00000dd0: 4149 2074 6561 6d73 2062 7920 3130 3020  AI teams by 100 
+00000de0: 7469 6d65 732e 0a0a 5377 616e 4c61 62e6  times...SwanLab.
+00000df0: 98af e4b8 80e4 b8aa e5bc 80e6 ba90 e380  ................
+00000e00: 81e8 bdbb e987 8fe7 baa7 e79a 8441 49e5  .............AI.
+00000e10: ae9e e9aa 8ce8 b79f e8b8 aae5 b7a5 e585  ................
+00000e20: b7ef bc8c e68f 90e4 be9b e4ba 86e4 b880  ................
+00000e30: e4b8 aae8 b79f e8b8 aae3 8081 e6af 94e8  ................
+00000e40: be83 e380 81e5 928c e58d 8fe4 bd9c e5ae  ................
+00000e50: 9ee9 aa8c e79a 84e5 b9b3 e58f b0ef bc8c  ................
+00000e60: e697 a8e5 9ca8 e58a a0e9 809f 4149 e7a0  ............AI..
+00000e70: 94e5 8f91 e59b a2e9 989f 3130 30e5 808d  ..........100...
+00000e80: e79a 84e7 a094 e58f 91e6 9588 e78e 87e3  ................
+00000e90: 8082 0a0a 4974 206f 6666 6572 7320 6120  ....It offers a 
+00000ea0: 7573 6572 2d66 7269 656e 646c 7920 4150  user-friendly AP
+00000eb0: 4920 616e 6420 6120 6465 6365 6e74 2069  I and a decent i
+00000ec0: 6e74 6572 6661 6365 2c20 636f 6d62 696e  nterface, combin
+00000ed0: 696e 6720 6665 6174 7572 6573 2073 7563  ing features suc
+00000ee0: 6820 6173 2074 7261 636b 696e 6720 6879  h as tracking hy
+00000ef0: 7065 7270 6172 616d 6574 6572 2c20 7265  perparameter, re
+00000f00: 636f 7264 696e 670a 6d65 7472 6963 2c20  cording.metric, 
+00000f10: 6f6e 6c69 6e65 2063 6f6c 6c61 626f 7261  online collabora
+00000f20: 7469 6f6e 2c20 7368 6172 696e 6720 6578  tion, sharing ex
+00000f30: 7065 7269 6d65 6e74 206c 696e 6b2c 2072  periment link, r
+00000f40: 6561 6c2d 7469 6d65 206d 6573 7361 6765  eal-time message
+00000f50: 206e 6f74 6966 6963 6174 696f 6e73 2c20   notifications, 
+00000f60: 616c 6c6f 7769 6e67 2079 6f75 2074 6f20  allowing you to 
+00000f70: 7175 6963 6b6c 7920 7472 6163 6b20 4d4c  quickly track ML
+00000f80: 0a65 7870 6572 696d 656e 7473 2c20 7669  .experiments, vi
+00000f90: 7375 616c 697a 6520 7072 6f63 6573 7365  sualize processe
+00000fa0: 732c 2061 6e64 2073 6861 7265 2077 6974  s, and share wit
+00000fb0: 6820 7065 6572 732e 0a0a 4279 2075 7369  h peers...By usi
+00000fc0: 6e67 2c20 7265 7365 6172 6368 6572 7320  ng, researchers 
+00000fd0: 6361 6e20 6163 6375 6d75 6c61 7465 2074  can accumulate t
+00000fe0: 6865 6972 2074 7261 696e 696e 6720 6578  heir training ex
+00000ff0: 7065 7269 656e 6365 7320 616e 6420 7365  periences and se
+00001000: 616d 6c65 7373 6c79 2063 6f6d 6d75 6e69  amlessly communi
+00001010: 6361 7465 2061 6e64 2063 6f6c 6c61 626f  cate and collabo
+00001020: 7261 7465 2077 6974 6820 7065 6572 732e  rate with peers.
+00001030: 0a4d 6163 6869 6e65 206c 6561 726e 696e  .Machine learnin
+00001040: 6720 656e 6769 6e65 6572 7320 6361 6e20  g engineers can 
+00001050: 6465 7665 6c6f 7020 6d6f 6465 6c73 2066  develop models f
+00001060: 6f72 2070 726f 6475 6374 696f 6e20 6d6f  or production mo
+00001070: 7265 2065 6666 6963 6965 6e74 6c79 2e0a  re efficiently..
+00001080: 0a21 5b5d 2872 6561 646d 655f 6669 6c65  .![](readme_file
+00001090: 732f 696e 7472 6f64 7563 7469 6f6e 2e70  s/introduction.p
+000010a0: 6e67 290a 0a48 6572 6520 6973 2074 6865  ng)..Here is the
+000010b0: 2045 6e67 6c69 7368 2076 6572 7369 6f6e   English version
+000010c0: 206f 6620 7468 6520 636f 7265 2066 6561   of the core fea
+000010d0: 7475 7265 206c 6973 7420 666f 7220 616e  ture list for an
+000010e0: 2041 4920 706c 6174 666f 726d 3a0a 0a2a   AI platform:..*
+000010f0: 2a31 2e20 f09f 938a 2045 7870 6572 696d  *1. .... Experim
+00001100: 656e 7461 6c20 4d65 7472 6963 7320 616e  ental Metrics an
+00001110: 6420 5472 6163 6b69 6e67 2048 7970 6572  d Tracking Hyper
+00001120: 7061 7261 6d65 7465 722a 2a3a 2045 6d62  parameter**: Emb
+00001130: 6564 2079 6f75 7220 6d61 6368 696e 6520  ed your machine 
+00001140: 6c65 6172 6e69 6e67 2070 6970 656c 696e  learning pipelin
+00001150: 6520 7769 7468 206d 696e 696d 616c 6973  e with minimalis
+00001160: 7469 6320 636f 6465 0a61 6e64 2074 7261  tic code.and tra
+00001170: 636b 206b 6579 2074 7261 696e 696e 6720  ck key training 
+00001180: 6d65 7472 6963 732e 0a0a 2d20 466c 6578  metrics...- Flex
+00001190: 6962 6c65 2072 6563 6f72 6469 6e67 206f  ible recording o
+000011a0: 6620 6879 7065 7270 6172 616d 6574 6572  f hyperparameter
+000011b0: 7320 616e 6420 6578 7065 7269 6d65 6e74  s and experiment
+000011c0: 2063 6f6e 6669 6775 7261 7469 6f6e 732e   configurations.
+000011d0: 0a2d 202a 2a53 7570 706f 7274 6564 206d  .- **Supported m
+000011e0: 6574 6164 6174 6120 7479 7065 732a 2a3a  etadata types**:
+000011f0: 2073 6361 6c61 7220 6d65 7472 6963 732c   scalar metrics,
+00001200: 2069 6d61 6765 732c 2061 7564 696f 2c20   images, audio, 
+00001210: 7465 7874 2c20 6574 632e 0a2d 202a 2a53  text, etc..- **S
+00001220: 7570 706f 7274 6564 2063 6861 7274 2074  upported chart t
+00001230: 7970 6573 2a2a 3a20 6c69 6e65 2067 7261  ypes**: line gra
+00001240: 7068 732c 206d 6564 6961 2063 6861 7274  phs, media chart
+00001250: 7320 2869 6d61 6765 732c 2061 7564 696f  s (images, audio
+00001260: 2c20 7465 7874 292c 2065 7463 2e0a 2d20  , text), etc..- 
+00001270: 2a2a 4175 746f 6d61 7469 6320 6c6f 6767  **Automatic logg
+00001280: 696e 672a 2a3a 2063 6f6e 736f 6c65 206c  ing**: console l
+00001290: 6f67 6769 6e67 2c20 4750 5520 6861 7264  ogging, GPU hard
+000012a0: 7761 7265 2c20 4769 7420 696e 666f 726d  ware, Git inform
+000012b0: 6174 696f 6e2c 2050 7974 686f 6e20 696e  ation, Python in
+000012c0: 7465 7270 7265 7465 722c 206c 6973 7420  terpreter, list 
+000012d0: 6f66 2050 7974 686f 6e20 6c69 6272 6172  of Python librar
+000012e0: 6965 732c 0a20 2063 6f64 6520 6469 7265  ies,.  code dire
+000012f0: 6374 6f72 792e 0a0a 2a2a 322e 20e2 9aa1  ctory...**2. ...
+00001300: efb8 8f20 436f 6d70 7265 6865 6e73 6976  ... Comprehensiv
+00001310: 6520 4672 616d 6577 6f72 6b20 496e 7465  e Framework Inte
+00001320: 6772 6174 696f 6e2a 2a3a 2050 7954 6f72  gration**: PyTor
+00001330: 6368 e380 8154 656e 736f 7266 6c6f 77e3  ch...Tensorflow.
+00001340: 8081 5079 546f 7263 6820 4c69 6768 746e  ..PyTorch Lightn
+00001350: 696e 67e3 8081 f09f a497 4875 6767 696e  ing.......Huggin
+00001360: 6746 6163 65e3 8081 5472 616e 7366 6f72  gFace...Transfor
+00001370: 6d65 7273 e380 814d 4d45 6e67 696e 65e3  mers...MMEngine.
+00001380: 8081 556c 7472 616c 7974 6963 73e3 8081  ..Ultralytics...
+00001390: 6661 7374 6169 e380 8154 656e 736f 7262  fastai...Tensorb
+000013a0: 6f61 7264 e380 814f 7065 6e41 49e3 8081  oard...OpenAI...
+000013b0: 5a68 6970 7541 49e3 8081 4879 6472 61e3  ZhipuAI...Hydra.
+000013c0: 8081 2e2e 2e0a 0a2a 2a33 2e20 f09f 93a6  .......**3. ....
+000013d0: 204f 7267 616e 697a 696e 6720 4578 7065   Organizing Expe
+000013e0: 7269 6d65 6e74 732a 2a3a 2043 656e 7472  riments**: Centr
+000013f0: 616c 697a 6564 2064 6173 6862 6f61 7264  alized dashboard
+00001400: 2066 6f72 2065 6666 6963 6965 6e74 6c79   for efficiently
+00001410: 206d 616e 6167 696e 6720 6d75 6c74 6970   managing multip
+00001420: 6c65 2070 726f 6a65 6374 7320 616e 6420  le projects and 
+00001430: 6578 7065 7269 6d65 6e74 732c 0a70 726f  experiments,.pro
+00001440: 7669 6469 6e67 2061 6e20 6f76 6572 7669  viding an overvi
+00001450: 6577 206f 6620 7472 6169 6e69 6e67 2061  ew of training a
+00001460: 7420 6120 676c 616e 6365 2e0a 0a2a 2a34  t a glance...**4
+00001470: 2e20 f09f 869a 2043 6f6d 7061 7269 6e67  . .... Comparing
+00001480: 2052 6573 756c 7473 2a2a 3a20 5573 6520   Results**: Use 
+00001490: 6f6e 6c69 6e65 2074 6162 6c65 7320 616e  online tables an
+000014a0: 6420 7061 6972 6564 2063 6861 7274 7320  d paired charts 
+000014b0: 746f 2063 6f6d 7061 7265 2074 6865 2068  to compare the h
+000014c0: 7970 6572 7061 7261 6d65 7465 7273 2061  yperparameters a
+000014d0: 6e64 206f 7574 636f 6d65 7320 6f66 2064  nd outcomes of d
+000014e0: 6966 6665 7265 6e74 0a65 7870 6572 696d  ifferent.experim
+000014f0: 656e 7473 2c20 6465 7665 6c6f 7069 6e67  ents, developing
+00001500: 2069 7465 7261 7469 7665 2069 6e73 7069   iterative inspi
+00001510: 7261 7469 6f6e 2e0a 0a2a 2a35 2e20 f09f  ration...**5. ..
+00001520: 91a5 204f 6e6c 696e 6520 436f 6c6c 6162  .. Online Collab
+00001530: 6f72 6174 696f 6e2a 2a3a 2043 6f6c 6c61  oration**: Colla
+00001540: 626f 7261 7465 2077 6974 6820 796f 7572  borate with your
+00001550: 2074 6561 6d20 6f6e 2074 7261 696e 696e   team on trainin
+00001560: 6720 7072 6f6a 6563 7473 2c20 7375 7070  g projects, supp
+00001570: 6f72 7469 6e67 2072 6561 6c2d 7469 6d65  orting real-time
+00001580: 2073 796e 6368 726f 6e69 7a61 7469 6f6e   synchronization
+00001590: 206f 660a 6578 7065 7269 6d65 6e74 7320   of.experiments 
+000015a0: 756e 6465 7220 7468 6520 7361 6d65 2070  under the same p
+000015b0: 726f 6a65 6374 2c20 616c 6c6f 7769 6e67  roject, allowing
+000015c0: 2079 6f75 2074 6f20 7379 6e63 6872 6f6e   you to synchron
+000015d0: 697a 6520 7472 6169 6e69 6e67 2072 6563  ize training rec
+000015e0: 6f72 6473 206f 6620 7468 6520 7465 616d  ords of the team
+000015f0: 206f 6e6c 696e 6520 616e 6420 7368 6172   online and shar
+00001600: 6520 696e 7369 6768 7473 0a61 6e64 2073  e insights.and s
+00001610: 7567 6765 7374 696f 6e73 2062 6173 6564  uggestions based
+00001620: 206f 6e20 7265 7375 6c74 732e 0a0a 2a2a   on results...**
+00001630: 362e 20e2 9c89 efb8 8f20 5368 6172 696e  6. ...... Sharin
+00001640: 6720 5265 7375 6c74 732a 2a3a 2043 6f70  g Results**: Cop
+00001650: 7920 616e 6420 7365 6e64 2070 6572 7369  y and send persi
+00001660: 7374 656e 7420 5552 4c73 2074 6f20 7368  stent URLs to sh
+00001670: 6172 6520 6561 6368 2065 7870 6572 696d  are each experim
+00001680: 656e 742c 2065 6666 6963 6965 6e74 6c79  ent, efficiently
+00001690: 2073 656e 6420 7468 656d 2074 6f20 636f   send them to co
+000016a0: 6c6c 6561 6775 6573 2c0a 6f72 2065 6d62  lleagues,.or emb
+000016b0: 6564 2074 6865 6d20 696e 206f 6e6c 696e  ed them in onlin
+000016c0: 6520 6e6f 7465 732e 0a0a 2a2a 372e 20f0  e notes...**7. .
+000016d0: 9f92 bb20 5365 6c66 2d68 6f73 7469 6e67  ... Self-hosting
+000016e0: 2053 7570 706f 7274 2a2a 3a20 5375 7070   Support**: Supp
+000016f0: 6f72 7473 206f 6666 6c69 6e65 206d 6f64  orts offline mod
+00001700: 6520 7769 7468 2061 2073 656c 662d 686f  e with a self-ho
+00001710: 7374 6564 2063 6f6d 6d75 6e69 7479 2076  sted community v
+00001720: 6572 7369 6f6e 2074 6861 7420 616c 736f  ersion that also
+00001730: 2061 6c6c 6f77 7320 666f 7220 6461 7368   allows for dash
+00001740: 626f 6172 640a 7669 6577 696e 6720 616e  board.viewing an
+00001750: 6420 6578 7065 7269 6d65 6e74 206d 616e  d experiment man
+00001760: 6167 656d 656e 742e 0a0a 3e20 5c5b 2149  agement...> \[!I
+00001770: 4d50 4f52 5441 4e54 5d0a 3e0a 3e20 2a2a  MPORTANT].>.> **
+00001780: 5374 6172 2055 732a 2a2c 2059 6f75 2077  Star Us**, You w
+00001790: 696c 6c20 7265 6365 6976 6520 616c 6c20  ill receive all 
+000017a0: 7265 6c65 6173 6520 6e6f 7469 6669 6361  release notifica
+000017b0: 7469 6f6e 7320 6672 6f6d 2047 6974 4875  tions from GitHu
+000017c0: 6220 7769 7468 6f75 7420 616e 7920 6465  b without any de
+000017d0: 6c61 7920 7e20 e2ad 90ef b88f 0a0a 0a0a  lay ~ ..........
+000017e0: 215b 7374 6172 2d75 735d 2872 6561 646d  ![star-us](readm
+000017f0: 655f 6669 6c65 732f 7374 6172 2d75 732e  e_files/star-us.
+00001800: 706e 6729 0a0a 3c62 723e 0a0a 2323 20f0  png)..<br>..## .
+00001810: 9f8f 8120 5175 6963 6b20 5374 6172 740a  ... Quick Start.
+00001820: 0a23 2323 2031 2e49 6e73 7461 6c6c 6174  .### 1.Installat
+00001830: 696f 6e0a 0a60 6060 6261 7368 0a70 6970  ion..```bash.pip
+00001840: 2069 6e73 7461 6c6c 2073 7761 6e6c 6162   install swanlab
+00001850: 0a60 6060 0a0a 2323 2320 322e 4c6f 6720  .```..### 2.Log 
+00001860: 696e 2061 6e64 2067 6574 2074 6865 2041  in and get the A
+00001870: 5049 204b 6579 0a0a 312e 202a 2a46 7265  PI Key..1. **Fre
+00001880: 6520 5b53 6967 6e20 5570 5d28 6874 7470  e [Sign Up](http
+00001890: 733a 2f2f 7377 616e 6c61 622e 636e 292a  s://swanlab.cn)*
+000018a0: 2a0a 0a32 2e20 2a2a 4c6f 6720 696e 2074  *..2. **Log in t
+000018b0: 6f20 796f 7572 2061 6363 6f75 6e74 2a2a  o your account**
+000018c0: 2c20 676f 2074 6f20 5573 6572 2053 6574  , go to User Set
+000018d0: 7469 6e67 7320 3e20 5b41 5049 204b 6579  tings > [API Key
+000018e0: 5d28 6874 7470 733a 2f2f 7377 616e 6c61  ](https://swanla
+000018f0: 622e 636e 2f73 6574 7469 6e67 7329 2061  b.cn/settings) a
+00001900: 6e64 2063 6f70 7920 796f 7572 2041 5049  nd copy your API
+00001910: 204b 6579 2e0a 0a33 2e20 2a2a 4f70 656e   Key...3. **Open
+00001920: 2079 6f75 7220 7465 726d 696e 616c 2061   your terminal a
+00001930: 6e64 2065 6e74 6572 2a2a 3a0a 0a60 6060  nd enter**:..```
+00001940: 6261 7368 0a73 7761 6e6c 6162 206c 6f67  bash.swanlab log
+00001950: 696e 0a60 6060 0a0a 5768 656e 2070 726f  in.```..When pro
+00001960: 6d70 7465 642c 2065 6e74 6572 2079 6f75  mpted, enter you
+00001970: 7220 4150 4920 4b65 7920 616e 6420 7072  r API Key and pr
+00001980: 6573 7320 456e 7465 7220 746f 2063 6f6d  ess Enter to com
+00001990: 706c 6574 6520 7468 6520 6c6f 6769 6e2e  plete the login.
+000019a0: 0a0a 2323 2320 332e 2049 6e74 6567 7261  ..### 3. Integra
+000019b0: 7465 2053 7761 6e4c 6162 2077 6974 6820  te SwanLab with 
+000019c0: 596f 7572 2043 6f64 650a 0a60 6060 7079  Your Code..```py
+000019d0: 7468 6f6e 0a69 6d70 6f72 7420 7377 616e  thon.import swan
+000019e0: 6c61 620a 0a23 2043 7265 6174 6520 6120  lab..# Create a 
+000019f0: 6e65 7720 5377 616e 4c61 6220 6578 7065  new SwanLab expe
+00001a00: 7269 6d65 6e74 0a73 7761 6e6c 6162 2e69  riment.swanlab.i
+00001a10: 6e69 7428 0a20 2020 2070 726f 6a65 6374  nit(.    project
+00001a20: 3d22 6d79 2d66 6972 7374 2d6d 6c22 2c0a  ="my-first-ml",.
+00001a30: 2020 2020 636f 6e66 6967 3d7b 276c 6561      config={'lea
+00001a40: 726e 696e 672d 7261 7465 273a 2030 2e30  rning-rate': 0.0
+00001a50: 3033 7d0a 290a 0a23 204c 6f67 206d 6574  03}.)..# Log met
+00001a60: 7269 6373 0a66 6f72 2069 2069 6e20 7261  rics.for i in ra
+00001a70: 6e67 6528 3130 293a 0a20 2020 2073 7761  nge(10):.    swa
+00001a80: 6e6c 6162 2e6c 6f67 287b 226c 6f73 7322  nlab.log({"loss"
+00001a90: 3a20 697d 290a 6060 600a 0a2a 2a41 6c6c  : i}).```..**All
+00001aa0: 2073 6574 212a 2a20 5669 7369 7420 5b53   set!** Visit [S
+00001ab0: 7761 6e4c 6162 5d28 6874 7470 733a 2f2f  wanLab](https://
+00001ac0: 7377 616e 6c61 622e 636e 2920 746f 2073  swanlab.cn) to s
+00001ad0: 6565 2079 6f75 7220 6669 7273 7420 5377  ee your first Sw
+00001ae0: 616e 4c61 6220 6578 7065 7269 6d65 6e74  anLab experiment
+00001af0: 2e0a 0a21 5b4d 4e49 5354 5d28 7265 6164  ...![MNIST](read
+00001b00: 6d65 5f66 696c 6573 2f72 6561 646d 652d  me_files/readme-
+00001b10: 6d6e 6973 742e 706e 6729 0a0a 3c62 723e  mnist.png)..<br>
+00001b20: 0a0a 2323 20f0 9f93 8320 4d6f 7265 2045  ..## .... More E
+00001b30: 7861 6d70 6c65 730a 0a3c 6465 7461 696c  xamples..<detail
+00001b40: 733e 0a3c 7375 6d6d 6172 793e 4d4e 4953  s>.<summary>MNIS
+00001b50: 543c 2f73 756d 6d61 7279 3e0a 0a60 6060  T</summary>..```
+00001b60: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f73  python.import os
+00001b70: 0a69 6d70 6f72 7420 746f 7263 680a 6672  .import torch.fr
+00001b80: 6f6d 2074 6f72 6368 2069 6d70 6f72 7420  om torch import 
+00001b90: 6e6e 2c20 6f70 7469 6d2c 2075 7469 6c73  nn, optim, utils
+00001ba0: 0a69 6d70 6f72 7420 746f 7263 682e 6e6e  .import torch.nn
+00001bb0: 2e66 756e 6374 696f 6e61 6c20 6173 2046  .functional as F
+00001bc0: 0a66 726f 6d20 746f 7263 6876 6973 696f  .from torchvisio
+00001bd0: 6e2e 6461 7461 7365 7473 2069 6d70 6f72  n.datasets impor
+00001be0: 7420 4d4e 4953 540a 6672 6f6d 2074 6f72  t MNIST.from tor
+00001bf0: 6368 7669 7369 6f6e 2e74 7261 6e73 666f  chvision.transfo
+00001c00: 726d 7320 696d 706f 7274 2054 6f54 656e  rms import ToTen
+00001c10: 736f 720a 696d 706f 7274 2073 7761 6e6c  sor.import swanl
+00001c20: 6162 0a0a 0a23 2043 4e4e e7bd 91e7 bb9c  ab...# CNN......
+00001c30: e69e 84e5 bbba 0a63 6c61 7373 2043 6f6e  .......class Con
+00001c40: 764e 6574 286e 6e2e 4d6f 6475 6c65 293a  vNet(nn.Module):
+00001c50: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00001c60: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00001c70: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00001c80: 5f28 290a 2020 2020 2020 2020 2320 312c  _().        # 1,
+00001c90: 3238 7832 380a 2020 2020 2020 2020 7365  28x28.        se
+00001ca0: 6c66 2e63 6f6e 7631 203d 206e 6e2e 436f  lf.conv1 = nn.Co
+00001cb0: 6e76 3264 2831 2c20 3130 2c20 3529 2020  nv2d(1, 10, 5)  
+00001cc0: 2320 3130 2c20 3234 7832 340a 2020 2020  # 10, 24x24.    
+00001cd0: 2020 2020 7365 6c66 2e63 6f6e 7632 203d      self.conv2 =
+00001ce0: 206e 6e2e 436f 6e76 3264 2831 302c 2032   nn.Conv2d(10, 2
+00001cf0: 302c 2033 2920 2023 2031 3238 2c20 3130  0, 3)  # 128, 10
+00001d00: 7831 300a 2020 2020 2020 2020 7365 6c66  x10.        self
+00001d10: 2e66 6331 203d 206e 6e2e 4c69 6e65 6172  .fc1 = nn.Linear
+00001d20: 2832 3020 2a20 3130 202a 2031 302c 2035  (20 * 10 * 10, 5
+00001d30: 3030 290a 2020 2020 2020 2020 7365 6c66  00).        self
+00001d40: 2e66 6332 203d 206e 6e2e 4c69 6e65 6172  .fc2 = nn.Linear
+00001d50: 2835 3030 2c20 3130 290a 0a20 2020 2064  (500, 10)..    d
+00001d60: 6566 2066 6f72 7761 7264 2873 656c 662c  ef forward(self,
+00001d70: 2078 293a 0a20 2020 2020 2020 2069 6e5f   x):.        in_
+00001d80: 7369 7a65 203d 2078 2e73 697a 6528 3029  size = x.size(0)
+00001d90: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+00001da0: 656c 662e 636f 6e76 3128 7829 2020 2320  elf.conv1(x)  # 
+00001db0: 3234 0a20 2020 2020 2020 206f 7574 203d  24.        out =
+00001dc0: 2046 2e72 656c 7528 6f75 7429 0a20 2020   F.relu(out).   
+00001dd0: 2020 2020 206f 7574 203d 2046 2e6d 6178       out = F.max
+00001de0: 5f70 6f6f 6c32 6428 6f75 742c 2032 2c20  _pool2d(out, 2, 
+00001df0: 3229 2020 2320 3132 0a20 2020 2020 2020  2)  # 12.       
+00001e00: 206f 7574 203d 2073 656c 662e 636f 6e76   out = self.conv
+00001e10: 3228 6f75 7429 2020 2320 3130 0a20 2020  2(out)  # 10.   
+00001e20: 2020 2020 206f 7574 203d 2046 2e72 656c       out = F.rel
+00001e30: 7528 6f75 7429 0a20 2020 2020 2020 206f  u(out).        o
+00001e40: 7574 203d 206f 7574 2e76 6965 7728 696e  ut = out.view(in
+00001e50: 5f73 697a 652c 202d 3129 0a20 2020 2020  _size, -1).     
+00001e60: 2020 206f 7574 203d 2073 656c 662e 6663     out = self.fc
+00001e70: 3128 6f75 7429 0a20 2020 2020 2020 206f  1(out).        o
+00001e80: 7574 203d 2046 2e72 656c 7528 6f75 7429  ut = F.relu(out)
+00001e90: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+00001ea0: 656c 662e 6663 3228 6f75 7429 0a20 2020  elf.fc2(out).   
+00001eb0: 2020 2020 206f 7574 203d 2046 2e6c 6f67       out = F.log
+00001ec0: 5f73 6f66 746d 6178 286f 7574 2c20 6469  _softmax(out, di
+00001ed0: 6d3d 3129 0a20 2020 2020 2020 2072 6574  m=1).        ret
+00001ee0: 7572 6e20 6f75 740a 0a0a 2320 e68d 95e8  urn out...# ....
+00001ef0: 8eb7 e5b9 b6e5 8faf e8a7 86e5 8c96 e589  ................
+00001f00: 8d32 30e5 bca0 e59b bee5 838f 0a64 6566  .20..........def
+00001f10: 206c 6f67 5f69 6d61 6765 7328 6c6f 6164   log_images(load
+00001f20: 6572 2c20 6e75 6d5f 696d 6167 6573 3d31  er, num_images=1
+00001f30: 3629 3a0a 2020 2020 696d 6167 6573 5f6c  6):.    images_l
+00001f40: 6f67 6765 6420 3d20 300a 2020 2020 6c6f  ogged = 0.    lo
+00001f50: 6767 6564 5f69 6d61 6765 7320 3d20 5b5d  gged_images = []
+00001f60: 0a20 2020 2066 6f72 2069 6d61 6765 732c  .    for images,
+00001f70: 206c 6162 656c 7320 696e 206c 6f61 6465   labels in loade
+00001f80: 723a 0a20 2020 2020 2020 2023 2069 6d61  r:.        # ima
+00001f90: 6765 733a 2062 6174 6368 206f 6620 696d  ges: batch of im
+00001fa0: 6167 6573 2c20 6c61 6265 6c73 3a20 6261  ages, labels: ba
+00001fb0: 7463 6820 6f66 206c 6162 656c 730a 2020  tch of labels.  
+00001fc0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00001fd0: 616e 6765 2869 6d61 6765 732e 7368 6170  ange(images.shap
+00001fe0: 655b 305d 293a 0a20 2020 2020 2020 2020  e[0]):.         
+00001ff0: 2020 2069 6620 696d 6167 6573 5f6c 6f67     if images_log
+00002000: 6765 6420 3c20 6e75 6d5f 696d 6167 6573  ged < num_images
+00002010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002020: 2020 2320 e4bd bfe7 94a8 7377 616e 6c61    # ......swanla
+00002030: 622e 496d 6167 65e5 b086 e59b bee5 838f  b.Image.........
+00002040: e8bd ace6 8da2 e4b8 ba77 616e 6462 e58f  .........wandb..
+00002050: afe8 a786 e58c 96e6 a0bc e5bc 8f0a 2020  ..............  
+00002060: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00002070: 6767 6564 5f69 6d61 6765 732e 6170 7065  gged_images.appe
+00002080: 6e64 2873 7761 6e6c 6162 2e49 6d61 6765  nd(swanlab.Image
+00002090: 2869 6d61 6765 735b 695d 2c20 6361 7074  (images[i], capt
+000020a0: 696f 6e3d 6622 4c61 6265 6c3a 207b 6c61  ion=f"Label: {la
+000020b0: 6265 6c73 5b69 5d7d 2229 290a 2020 2020  bels[i]}")).    
+000020c0: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+000020d0: 6573 5f6c 6f67 6765 6420 2b3d 2031 0a20  es_logged += 1. 
+000020e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000020f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002100: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
+00002110: 6620 696d 6167 6573 5f6c 6f67 6765 6420  f images_logged 
+00002120: 3e3d 206e 756d 5f69 6d61 6765 733a 0a20  >= num_images:. 
+00002130: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00002140: 0a20 2020 2073 7761 6e6c 6162 2e6c 6f67  .    swanlab.log
+00002150: 287b 224d 4e49 5354 2d50 7265 7669 6577  ({"MNIST-Preview
+00002160: 223a 206c 6f67 6765 645f 696d 6167 6573  ": logged_images
+00002170: 7d29 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  })...if __name__
+00002180: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
+00002190: 0a20 2020 2023 20e5 889d e5a7 8be5 8c96  .    # .........
+000021a0: 7377 616e 6c61 620a 2020 2020 7275 6e20  swanlab.    run 
+000021b0: 3d20 7377 616e 6c61 622e 696e 6974 280a  = swanlab.init(.
+000021c0: 2020 2020 2020 2020 7072 6f6a 6563 743d          project=
+000021d0: 224d 4e49 5354 2d65 7861 6d70 6c65 222c  "MNIST-example",
+000021e0: 0a20 2020 2020 2020 2065 7870 6572 696d  .        experim
+000021f0: 656e 745f 6e61 6d65 3d22 436f 6e76 4e65  ent_name="ConvNe
+00002200: 7422 2c0a 2020 2020 2020 2020 6465 7363  t",.        desc
+00002210: 7269 7074 696f 6e3d 2254 7261 696e 2043  ription="Train C
+00002220: 6f6e 764e 6574 206f 6e20 4d4e 4953 5420  onvNet on MNIST 
+00002230: 6461 7461 7365 742e 222c 0a20 2020 2020  dataset.",.     
+00002240: 2020 2063 6f6e 6669 673d 7b0a 2020 2020     config={.    
+00002250: 2020 2020 2020 2020 226d 6f64 656c 223a          "model":
+00002260: 2022 434e 4e22 2c0a 2020 2020 2020 2020   "CNN",.        
+00002270: 2020 2020 226f 7074 696d 223a 2022 4164      "optim": "Ad
+00002280: 616d 222c 0a20 2020 2020 2020 2020 2020  am",.           
+00002290: 2022 6c72 223a 2030 2e30 3031 2c0a 2020   "lr": 0.001,.  
+000022a0: 2020 2020 2020 2020 2020 2262 6174 6368            "batch
+000022b0: 5f73 697a 6522 3a20 3531 322c 0a20 2020  _size": 512,.   
+000022c0: 2020 2020 2020 2020 2022 6e75 6d5f 6570           "num_ep
+000022d0: 6f63 6873 223a 2031 302c 0a20 2020 2020  ochs": 10,.     
+000022e0: 2020 2020 2020 2022 7472 6169 6e5f 6461         "train_da
+000022f0: 7461 7365 745f 6e75 6d22 3a20 3535 3030  taset_num": 5500
+00002300: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00002310: 7661 6c5f 6461 7461 7365 745f 6e75 6d22  val_dataset_num"
+00002320: 3a20 3530 3030 2c0a 2020 2020 2020 2020  : 5000,.        
+00002330: 7d2c 0a20 2020 2029 0a0a 2020 2020 2320  },.    )..    # 
+00002340: e8ae bee7 bdae e8ae ade7 bb83 e69c bae3  ................
+00002350: 8081 e9aa 8ce8 af81 e99b 86e5 928c e6b5  ................
+00002360: 8be8 af95 e99b 860a 2020 2020 6461 7461  ........    data
+00002370: 7365 7420 3d20 4d4e 4953 5428 6f73 2e67  set = MNIST(os.g
+00002380: 6574 6377 6428 292c 2074 7261 696e 3d54  etcwd(), train=T
+00002390: 7275 652c 2064 6f77 6e6c 6f61 643d 5472  rue, download=Tr
+000023a0: 7565 2c20 7472 616e 7366 6f72 6d3d 546f  ue, transform=To
+000023b0: 5465 6e73 6f72 2829 290a 2020 2020 7472  Tensor()).    tr
+000023c0: 6169 6e5f 6461 7461 7365 742c 2076 616c  ain_dataset, val
+000023d0: 5f64 6174 6173 6574 203d 2075 7469 6c73  _dataset = utils
+000023e0: 2e64 6174 612e 7261 6e64 6f6d 5f73 706c  .data.random_spl
+000023f0: 6974 280a 2020 2020 2020 2020 6461 7461  it(.        data
+00002400: 7365 742c 205b 7275 6e2e 636f 6e66 6967  set, [run.config
+00002410: 2e74 7261 696e 5f64 6174 6173 6574 5f6e  .train_dataset_n
+00002420: 756d 2c20 7275 6e2e 636f 6e66 6967 2e76  um, run.config.v
+00002430: 616c 5f64 6174 6173 6574 5f6e 756d 5d0a  al_dataset_num].
+00002440: 2020 2020 290a 0a20 2020 2074 7261 696e      )..    train
+00002450: 5f6c 6f61 6465 7220 3d20 7574 696c 732e  _loader = utils.
+00002460: 6461 7461 2e44 6174 614c 6f61 6465 7228  data.DataLoader(
+00002470: 7472 6169 6e5f 6461 7461 7365 742c 2062  train_dataset, b
+00002480: 6174 6368 5f73 697a 653d 7275 6e2e 636f  atch_size=run.co
+00002490: 6e66 6967 2e62 6174 6368 5f73 697a 652c  nfig.batch_size,
+000024a0: 2073 6875 6666 6c65 3d54 7275 6529 0a20   shuffle=True). 
+000024b0: 2020 2076 616c 5f6c 6f61 6465 7220 3d20     val_loader = 
+000024c0: 7574 696c 732e 6461 7461 2e44 6174 614c  utils.data.DataL
+000024d0: 6f61 6465 7228 7661 6c5f 6461 7461 7365  oader(val_datase
+000024e0: 742c 2062 6174 6368 5f73 697a 653d 312c  t, batch_size=1,
+000024f0: 2073 6875 6666 6c65 3d46 616c 7365 290a   shuffle=False).
+00002500: 0a20 2020 2023 20e5 889d e5a7 8be5 8c96  .    # .........
+00002510: e6a8 a1e5 9e8b e380 81e6 8d9f e5a4 b1e5  ................
+00002520: 87bd e695 b0e5 928c e4bc 98e5 8c96 e599  ................
+00002530: a80a 2020 2020 6d6f 6465 6c20 3d20 436f  ..    model = Co
+00002540: 6e76 4e65 7428 290a 2020 2020 6372 6974  nvNet().    crit
+00002550: 6572 696f 6e20 3d20 6e6e 2e43 726f 7373  erion = nn.Cross
+00002560: 456e 7472 6f70 794c 6f73 7328 290a 2020  EntropyLoss().  
+00002570: 2020 6f70 7469 6d69 7a65 7220 3d20 6f70    optimizer = op
+00002580: 7469 6d2e 4164 616d 286d 6f64 656c 2e70  tim.Adam(model.p
+00002590: 6172 616d 6574 6572 7328 292c 206c 723d  arameters(), lr=
+000025a0: 7275 6e2e 636f 6e66 6967 2e6c 7229 0a0a  run.config.lr)..
+000025b0: 2020 2020 2320 efbc 88e5 8faf e980 89ef      # ..........
+000025c0: bc89 e79c 8be4 b880 e4b8 8be6 95b0 e68d  ................
+000025d0: aee9 9b86 e79a 84e5 898d 3136 e5bc a0e5  ..........16....
+000025e0: 9bbe e583 8f0a 2020 2020 6c6f 675f 696d  ......    log_im
+000025f0: 6167 6573 2874 7261 696e 5f6c 6f61 6465  ages(train_loade
+00002600: 722c 2031 3629 0a0a 2020 2020 2320 e5bc  r, 16)..    # ..
+00002610: 80e5 a78b e8ae ade7 bb83 0a20 2020 2066  ...........    f
+00002620: 6f72 2065 706f 6368 2069 6e20 7261 6e67  or epoch in rang
+00002630: 6528 312c 2072 756e 2e63 6f6e 6669 672e  e(1, run.config.
+00002640: 6e75 6d5f 6570 6f63 6873 293a 0a20 2020  num_epochs):.   
+00002650: 2020 2020 2073 7761 6e6c 6162 2e6c 6f67       swanlab.log
+00002660: 287b 2274 7261 696e 2f65 706f 6368 223a  ({"train/epoch":
+00002670: 2065 706f 6368 7d29 0a20 2020 2020 2020   epoch}).       
+00002680: 2023 20e8 aead e7bb 83e5 beaa e78e af0a   # .............
+00002690: 2020 2020 2020 2020 666f 7220 6974 6572          for iter
+000026a0: 2c20 6261 7463 6820 696e 2065 6e75 6d65  , batch in enume
+000026b0: 7261 7465 2874 7261 696e 5f6c 6f61 6465  rate(train_loade
+000026c0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000026d0: 782c 2079 203d 2062 6174 6368 0a20 2020  x, y = batch.   
+000026e0: 2020 2020 2020 2020 206f 7074 696d 697a           optimiz
+000026f0: 6572 2e7a 6572 6f5f 6772 6164 2829 0a20  er.zero_grad(). 
+00002700: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00002710: 7420 3d20 6d6f 6465 6c28 7829 0a20 2020  t = model(x).   
+00002720: 2020 2020 2020 2020 206c 6f73 7320 3d20           loss = 
+00002730: 6372 6974 6572 696f 6e28 6f75 7470 7574  criterion(output
+00002740: 2c20 7929 0a20 2020 2020 2020 2020 2020  , y).           
+00002750: 206c 6f73 732e 6261 636b 7761 7264 2829   loss.backward()
+00002760: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+00002770: 696d 697a 6572 2e73 7465 7028 290a 0a20  imizer.step().. 
+00002780: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00002790: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000027a0: 2020 6622 4570 6f63 6820 5b7b 6570 6f63    f"Epoch [{epoc
+000027b0: 687d 2f7b 7275 6e2e 636f 6e66 6967 2e6e  h}/{run.config.n
+000027c0: 756d 5f65 706f 6368 737d 5d2c 2049 7465  um_epochs}], Ite
+000027d0: 7261 7469 6f6e 205b 7b69 7465 7220 2b20  ration [{iter + 
+000027e0: 317d 2f7b 6c65 6e28 7472 6169 6e5f 6c6f  1}/{len(train_lo
+000027f0: 6164 6572 297d 5d2c 204c 6f73 733a 207b  ader)}], Loss: {
+00002800: 6c6f 7373 2e69 7465 6d28 297d 220a 2020  loss.item()}".  
+00002810: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00002820: 2020 2020 2020 2020 2069 6620 6974 6572           if iter
+00002830: 2025 2032 3020 3d3d 2030 3a0a 2020 2020   % 20 == 0:.    
+00002840: 2020 2020 2020 2020 2020 2020 7377 616e              swan
+00002850: 6c61 622e 6c6f 6728 7b22 7472 6169 6e2f  lab.log({"train/
+00002860: 6c6f 7373 223a 206c 6f73 732e 6974 656d  loss": loss.item
+00002870: 2829 7d2c 2073 7465 703d 2865 706f 6368  ()}, step=(epoch
+00002880: 202d 2031 2920 2a20 6c65 6e28 7472 6169   - 1) * len(trai
+00002890: 6e5f 6c6f 6164 6572 2920 2b20 6974 6572  n_loader) + iter
+000028a0: 290a 0a20 2020 2020 2020 2023 20e6 af8f  )..        # ...
+000028b0: 34e4 b8aa 6570 6f63 68e9 aa8c e8af 81e4  4...epoch.......
+000028c0: b880 e6ac a10a 2020 2020 2020 2020 6966  ......        if
+000028d0: 2065 706f 6368 2025 2032 203d 3d20 303a   epoch % 2 == 0:
+000028e0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+000028f0: 656c 2e65 7661 6c28 290a 2020 2020 2020  el.eval().      
+00002900: 2020 2020 2020 636f 7272 6563 7420 3d20        correct = 
+00002910: 300a 2020 2020 2020 2020 2020 2020 746f  0.            to
+00002920: 7461 6c20 3d20 300a 2020 2020 2020 2020  tal = 0.        
+00002930: 2020 2020 7769 7468 2074 6f72 6368 2e6e      with torch.n
+00002940: 6f5f 6772 6164 2829 3a0a 2020 2020 2020  o_grad():.      
+00002950: 2020 2020 2020 2020 2020 666f 7220 6261            for ba
+00002960: 7463 6820 696e 2076 616c 5f6c 6f61 6465  tch in val_loade
+00002970: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00002980: 2020 2020 2020 2078 2c20 7920 3d20 6261         x, y = ba
+00002990: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
+000029a0: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+000029b0: 206d 6f64 656c 2878 290a 2020 2020 2020   model(x).      
+000029c0: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
+000029d0: 2070 7265 6469 6374 6564 203d 2074 6f72   predicted = tor
+000029e0: 6368 2e6d 6178 286f 7574 7075 742c 2031  ch.max(output, 1
+000029f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002a00: 2020 2020 2020 746f 7461 6c20 2b3d 2079        total += y
+00002a10: 2e73 697a 6528 3029 0a20 2020 2020 2020  .size(0).       
+00002a20: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
+00002a30: 7265 6374 202b 3d20 2870 7265 6469 6374  rect += (predict
+00002a40: 6564 203d 3d20 7929 2e73 756d 2829 2e69  ed == y).sum().i
+00002a50: 7465 6d28 290a 0a20 2020 2020 2020 2020  tem()..         
+00002a60: 2020 2061 6363 7572 6163 7920 3d20 636f     accuracy = co
+00002a70: 7272 6563 7420 2f20 746f 7461 6c0a 2020  rrect / total.  
+00002a80: 2020 2020 2020 2020 2020 7377 616e 6c61            swanla
+00002a90: 622e 6c6f 6728 7b22 7661 6c2f 6163 6375  b.log({"val/accu
+00002aa0: 7261 6379 223a 2061 6363 7572 6163 797d  racy": accuracy}
+00002ab0: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
+00002ac0: 3e0a 0a5b 4245 5254 2d49 4d44 425d 2868  >..[BERT-IMDB](h
+00002ad0: 7474 7073 3a2f 2f64 6f63 732e 7377 616e  ttps://docs.swan
+00002ae0: 6c61 622e 636e 2f7a 682f 6578 616d 706c  lab.cn/zh/exampl
+00002af0: 6573 2f62 6572 742e 6874 6d6c 290a 0a5b  es/bert.html)..[
+00002b00: 594f 4c4f 5d28 6874 7470 733a 2f2f 646f  YOLO](https://do
+00002b10: 6373 2e73 7761 6e6c 6162 2e63 6e2f 7a68  cs.swanlab.cn/zh
+00002b20: 2f65 7861 6d70 6c65 732f 796f 6c6f 2e68  /examples/yolo.h
+00002b30: 746d 6c29 0a0a 3c62 723e 0a0a 2323 20f0  tml)..<br>..## .
+00002b40: 9f92 bb20 5365 6c66 2d68 6f73 7465 640a  ... Self-hosted.
+00002b50: 0a54 6865 2063 6f6d 6d75 6e69 7479 2065  .The community e
+00002b60: 6469 7469 6f6e 2073 7570 706f 7274 7320  dition supports 
+00002b70: 6f66 666c 696e 6520 7669 6577 696e 6720  offline viewing 
+00002b80: 6f66 2053 7761 6e4c 6162 2064 6173 6862  of SwanLab dashb
+00002b90: 6f61 7264 732e 0a0a 2323 2320 4f66 666c  oards...### Offl
+00002ba0: 696e 6520 4578 7065 7269 6d65 6e74 2054  ine Experiment T
+00002bb0: 7261 636b 696e 670a 0a53 6574 2074 6865  racking..Set the
+00002bc0: 2070 6172 616d 6574 6572 7320 606c 6f67   parameters `log
+00002bd0: 6972 6020 616e 6420 606d 6f64 6560 2069  ir` and `mode` i
+00002be0: 6e20 7377 616e 6c61 622e 696e 6974 2074  n swanlab.init t
+00002bf0: 6f20 7472 6163 6b20 6578 7065 7269 6d65  o track experime
+00002c00: 6e74 7320 6f66 666c 696e 653a 0a0a 6060  nts offline:..``
+00002c10: 6070 7974 686f 6e0a 2e2e 2e0a 0a73 7761  `python......swa
+00002c20: 6e6c 6162 2e69 6e69 7428 0a20 2020 206c  nlab.init(.    l
+00002c30: 6f67 6469 723d 272e 2f6c 6f67 7327 2c0a  ogdir='./logs',.
+00002c40: 2020 2020 6d6f 6465 3d27 6c6f 6361 6c27      mode='local'
+00002c50: 2c0a 290a 0a2e 2e2e 0a60 6060 0a0a 2d20  ,.)......```..- 
+00002c60: 5468 6520 7061 7261 6d65 7465 7220 606d  The parameter `m
+00002c70: 6f64 6560 2069 7320 7365 7420 746f 2060  ode` is set to `
+00002c80: 6c6f 6361 6c60 2c20 7768 6963 6820 6469  local`, which di
+00002c90: 7361 626c 6573 2073 796e 6368 726f 6e69  sables synchroni
+00002ca0: 7a69 6e67 2074 6865 2065 7870 6572 696d  zing the experim
+00002cb0: 656e 7420 746f 2074 6865 2063 6c6f 7564  ent to the cloud
+00002cc0: 2e0a 0a2d 2054 6865 2073 6574 7469 6e67  ...- The setting
+00002cd0: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
+00002ce0: 7220 606c 6f67 6469 7260 2069 7320 6f70  r `logdir` is op
+00002cf0: 7469 6f6e 616c 2c20 616e 6420 6974 2073  tional, and it s
+00002d00: 7065 6369 6669 6573 2074 6865 206c 6f63  pecifies the loc
+00002d10: 6174 696f 6e20 666f 7220 7361 7669 6e67  ation for saving
+00002d20: 2053 7761 6e4c 6162 206c 6f67 2066 696c   SwanLab log fil
+00002d30: 6573 2028 6279 0a20 2064 6566 6175 6c74  es (by.  default
+00002d40: 2073 6176 6564 2069 6e20 7468 6520 6073   saved in the `s
+00002d50: 7761 6e6c 6f67 6020 666f 6c64 6572 292e  wanlog` folder).
+00002d60: 0a0a 2d20 4c6f 6720 6669 6c65 7320 7769  ..- Log files wi
+00002d70: 6c6c 2062 6520 6372 6561 7465 6420 616e  ll be created an
+00002d80: 6420 7570 6461 7465 6420 6475 7269 6e67  d updated during
+00002d90: 2074 7261 636b 696e 6720 6f66 2065 7870   tracking of exp
+00002da0: 6572 696d 656e 7473 2c20 616e 6420 6c61  eriments, and la
+00002db0: 756e 6368 696e 6720 6f66 666c 696e 6520  unching offline 
+00002dc0: 6461 7368 626f 6172 6473 2077 696c 6c20  dashboards will 
+00002dd0: 616c 736f 2062 650a 2020 6261 7365 6420  also be.  based 
+00002de0: 6f6e 2074 6865 7365 206c 6f67 2066 696c  on these log fil
+00002df0: 6573 2e0a 0a4f 7468 6572 2070 6172 7473  es...Other parts
+00002e00: 2061 7265 2063 6f6d 706c 6574 656c 7920   are completely 
+00002e10: 636f 6e73 6973 7465 6e74 2077 6974 6820  consistent with 
+00002e20: 636c 6f75 6420 7573 6167 652e 0a0a 2323  cloud usage...##
+00002e30: 2320 4f70 656e 204f 6666 6c69 6e65 2042  # Open Offline B
+00002e40: 6f61 7264 0a0a 4f70 656e 2074 6865 2074  oard..Open the t
+00002e50: 6572 6d69 6e61 6c20 616e 6420 7573 6520  erminal and use 
+00002e60: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00002e70: 6d6d 616e 6420 746f 206f 7065 6e20 6120  mmand to open a 
+00002e80: 5377 616e 4c61 6220 6461 7368 626f 6172  SwanLab dashboar
+00002e90: 643a 0a0a 6060 6062 6173 680a 7377 616e  d:..```bash.swan
+00002ea0: 6c61 6220 7761 7463 6820 2d6c 202e 2f6c  lab watch -l ./l
+00002eb0: 6f67 730a 6060 600a 0a41 6674 6572 2074  ogs.```..After t
+00002ec0: 6865 206f 7065 7261 7469 6f6e 2069 7320  he operation is 
+00002ed0: 636f 6d70 6c65 7465 642c 2053 7761 6e4c  completed, SwanL
+00002ee0: 6162 2077 696c 6c20 7072 6f76 6964 6520  ab will provide 
+00002ef0: 796f 7520 7769 7468 2061 206c 6f63 616c  you with a local
+00002f00: 2055 524c 206c 696e 6b20 2864 6566 6175   URL link (defau
+00002f10: 6c74 0a69 7320 5b68 7474 703a 2f2f 3132  lt.is [http://12
+00002f20: 372e 302e 302e 313a 3530 3932 5d28 6874  7.0.0.1:5092](ht
+00002f30: 7470 3a2f 2f31 3237 2e30 2e30 2e31 3a35  tp://127.0.0.1:5
+00002f40: 3039 3229 292e 0a0a 5669 7369 7420 7468  092))...Visit th
+00002f50: 6973 206c 696e 6b20 746f 2076 6965 7720  is link to view 
+00002f60: 7468 6520 6578 7065 7269 6d65 6e74 206f  the experiment o
+00002f70: 6666 6c69 6e65 2069 6e20 7468 6520 6272  ffline in the br
+00002f80: 6f77 7365 7220 6461 7368 626f 6172 642e  owser dashboard.
+00002f90: 0a0a 3c62 723e 0a0a 2323 20f0 9f9a 9720  ..<br>..## .... 
+00002fa0: 496e 7465 6772 6174 696f 6e0a 0a43 6f6d  Integration..Com
+00002fb0: 6269 6e65 2079 6f75 7220 6661 766f 7269  bine your favori
+00002fc0: 7465 2066 7261 6d65 776f 726b 2077 6974  te framework wit
+00002fd0: 680a 5377 616e 4c61 622c 205b 4d6f 7265  h.SwanLab, [More
+00002fe0: 2049 6e74 6567 7261 7469 6f6e 5d28 6874   Integration](ht
+00002ff0: 7470 733a 2f2f 646f 6373 2e73 7761 6e6c  tps://docs.swanl
+00003000: 6162 2e63 6e2f 7a68 2f67 7569 6465 5f63  ab.cn/zh/guide_c
+00003010: 6c6f 7564 2f69 6e74 6567 7261 7469 6f6e  loud/integration
+00003020: 2f69 6e74 6567 7261 7469 6f6e 2d70 7974  /integration-pyt
+00003030: 6f72 6368 2d6c 6967 6874 6e69 6e67 2e68  orch-lightning.h
+00003040: 746d 6c29 2e0a 0a3c 6465 7461 696c 733e  tml)...<details>
+00003050: 0a20 203c 7375 6d6d 6172 793e 0a20 2020  .  <summary>.   
+00003060: 203c 7374 726f 6e67 3ee2 9aa1 efb8 8f20   <strong>...... 
+00003070: 5079 546f 7263 6820 4c69 6768 746e 696e  PyTorch Lightnin
+00003080: 673c 2f73 7472 6f6e 673e 0a20 203c 2f73  g</strong>.  </s
+00003090: 756d 6d61 7279 3e0a 2020 3c62 723e 0a0a  ummary>.  <br>..
+000030a0: 4372 6561 7465 2061 6e20 696e 7374 616e  Create an instan
+000030b0: 6365 2075 7369 6e67 2060 5377 616e 4c61  ce using `SwanLa
+000030c0: 624c 6f67 6765 7260 2061 6e64 2070 6173  bLogger` and pas
+000030d0: 7320 6974 2069 6e74 6f20 7468 6520 606c  s it into the `l
+000030e0: 6f67 6765 7260 2070 6172 616d 6574 6572  ogger` parameter
+000030f0: 206f 6620 6054 7261 696e 6572 6020 746f   of `Trainer` to
+00003100: 2065 6e61 626c 6520 5377 616e 4c61 6220   enable SwanLab 
+00003110: 746f 0a72 6563 6f72 6420 7472 6169 6e69  to.record traini
+00003120: 6e67 206d 6574 7269 6373 2e0a 0a60 6060  ng metrics...```
+00003130: 7079 7468 6f6e 0a66 726f 6d20 7377 616e  python.from swan
+00003140: 6c61 622e 696e 7465 6772 6174 696f 6e2e  lab.integration.
+00003150: 7079 746f 7263 685f 6c69 6768 746e 696e  pytorch_lightnin
+00003160: 6720 696d 706f 7274 2053 7761 6e4c 6162  g import SwanLab
+00003170: 4c6f 6767 6572 0a69 6d70 6f72 7420 696d  Logger.import im
+00003180: 706f 7274 6c69 622e 7574 696c 0a69 6d70  portlib.util.imp
+00003190: 6f72 7420 6f73 0a69 6d70 6f72 7420 7079  ort os.import py
+000031a0: 746f 7263 685f 6c69 6768 746e 696e 6720  torch_lightning 
+000031b0: 6173 2070 6c0a 6672 6f6d 2074 6f72 6368  as pl.from torch
+000031c0: 2069 6d70 6f72 7420 6e6e 2c20 6f70 7469   import nn, opti
+000031d0: 6d2c 2075 7469 6c73 0a66 726f 6d20 746f  m, utils.from to
+000031e0: 7263 6876 6973 696f 6e2e 6461 7461 7365  rchvision.datase
+000031f0: 7473 2069 6d70 6f72 7420 4d4e 4953 540a  ts import MNIST.
+00003200: 6672 6f6d 2074 6f72 6368 7669 7369 6f6e  from torchvision
+00003210: 2e74 7261 6e73 666f 726d 7320 696d 706f  .transforms impo
+00003220: 7274 2054 6f54 656e 736f 720a 0a65 6e63  rt ToTensor..enc
+00003230: 6f64 6572 203d 206e 6e2e 5365 7175 656e  oder = nn.Sequen
+00003240: 7469 616c 286e 6e2e 4c69 6e65 6172 2832  tial(nn.Linear(2
+00003250: 3820 2a20 3238 2c20 3132 3829 2c20 6e6e  8 * 28, 128), nn
+00003260: 2e52 654c 5528 292c 206e 6e2e 4c69 6e65  .ReLU(), nn.Line
+00003270: 6172 2831 3238 2c20 3329 290a 6465 636f  ar(128, 3)).deco
+00003280: 6465 7220 3d20 6e6e 2e53 6571 7565 6e74  der = nn.Sequent
+00003290: 6961 6c28 6e6e 2e4c 696e 6561 7228 332c  ial(nn.Linear(3,
+000032a0: 2031 3238 292c 206e 6e2e 5265 4c55 2829   128), nn.ReLU()
+000032b0: 2c20 6e6e 2e4c 696e 6561 7228 3132 382c  , nn.Linear(128,
+000032c0: 2032 3820 2a20 3238 2929 0a0a 0a63 6c61   28 * 28))...cla
+000032d0: 7373 204c 6974 4175 746f 456e 636f 6465  ss LitAutoEncode
+000032e0: 7228 706c 2e4c 6967 6874 6e69 6e67 4d6f  r(pl.LightningMo
+000032f0: 6475 6c65 293a 0a20 2020 2064 6566 205f  dule):.    def _
+00003300: 5f69 6e69 745f 5f28 7365 6c66 2c20 656e  _init__(self, en
+00003310: 636f 6465 722c 2064 6563 6f64 6572 293a  coder, decoder):
+00003320: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00003330: 2e5f 5f69 6e69 745f 5f28 290a 2020 2020  .__init__().    
+00003340: 2020 2020 7365 6c66 2e65 6e63 6f64 6572      self.encoder
+00003350: 203d 2065 6e63 6f64 6572 0a20 2020 2020   = encoder.     
+00003360: 2020 2073 656c 662e 6465 636f 6465 7220     self.decoder 
+00003370: 3d20 6465 636f 6465 720a 0a20 2020 2064  = decoder..    d
+00003380: 6566 2074 7261 696e 696e 675f 7374 6570  ef training_step
+00003390: 2873 656c 662c 2062 6174 6368 2c20 6261  (self, batch, ba
+000033a0: 7463 685f 6964 7829 3a0a 2020 2020 2020  tch_idx):.      
+000033b0: 2020 2320 7472 6169 6e69 6e67 5f73 7465    # training_ste
+000033c0: 7020 6465 6669 6e65 7320 7468 6520 7472  p defines the tr
+000033d0: 6169 6e20 6c6f 6f70 2e0a 2020 2020 2020  ain loop..      
+000033e0: 2020 2320 6974 2069 7320 696e 6465 7065    # it is indepe
+000033f0: 6e64 656e 7420 6f66 2066 6f72 7761 7264  ndent of forward
+00003400: 0a20 2020 2020 2020 2078 2c20 7920 3d20  .        x, y = 
+00003410: 6261 7463 680a 2020 2020 2020 2020 7820  batch.        x 
+00003420: 3d20 782e 7669 6577 2878 2e73 697a 6528  = x.view(x.size(
+00003430: 3029 2c20 2d31 290a 2020 2020 2020 2020  0), -1).        
+00003440: 7a20 3d20 7365 6c66 2e65 6e63 6f64 6572  z = self.encoder
+00003450: 2878 290a 2020 2020 2020 2020 785f 6861  (x).        x_ha
+00003460: 7420 3d20 7365 6c66 2e64 6563 6f64 6572  t = self.decoder
+00003470: 287a 290a 2020 2020 2020 2020 6c6f 7373  (z).        loss
+00003480: 203d 206e 6e2e 6675 6e63 7469 6f6e 616c   = nn.functional
+00003490: 2e6d 7365 5f6c 6f73 7328 785f 6861 742c  .mse_loss(x_hat,
+000034a0: 2078 290a 2020 2020 2020 2020 2320 4c6f   x).        # Lo
+000034b0: 6767 696e 6720 746f 2054 656e 736f 7242  gging to TensorB
+000034c0: 6f61 7264 2028 6966 2069 6e73 7461 6c6c  oard (if install
+000034d0: 6564 2920 6279 2064 6566 6175 6c74 0a20  ed) by default. 
+000034e0: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+000034f0: 2274 7261 696e 5f6c 6f73 7322 2c20 6c6f  "train_loss", lo
+00003500: 7373 290a 2020 2020 2020 2020 7265 7475  ss).        retu
+00003510: 726e 206c 6f73 730a 0a20 2020 2064 6566  rn loss..    def
+00003520: 2074 6573 745f 7374 6570 2873 656c 662c   test_step(self,
+00003530: 2062 6174 6368 2c20 6261 7463 685f 6964   batch, batch_id
+00003540: 7829 3a0a 2020 2020 2020 2020 2320 7465  x):.        # te
+00003550: 7374 5f73 7465 7020 6465 6669 6e65 7320  st_step defines 
+00003560: 7468 6520 7465 7374 206c 6f6f 702e 0a20  the test loop.. 
+00003570: 2020 2020 2020 2023 2069 7420 6973 2069         # it is i
+00003580: 6e64 6570 656e 6465 6e74 206f 6620 666f  ndependent of fo
+00003590: 7277 6172 640a 2020 2020 2020 2020 782c  rward.        x,
+000035a0: 2079 203d 2062 6174 6368 0a20 2020 2020   y = batch.     
+000035b0: 2020 2078 203d 2078 2e76 6965 7728 782e     x = x.view(x.
+000035c0: 7369 7a65 2830 292c 202d 3129 0a20 2020  size(0), -1).   
+000035d0: 2020 2020 207a 203d 2073 656c 662e 656e       z = self.en
+000035e0: 636f 6465 7228 7829 0a20 2020 2020 2020  coder(x).       
+000035f0: 2078 5f68 6174 203d 2073 656c 662e 6465   x_hat = self.de
+00003600: 636f 6465 7228 7a29 0a20 2020 2020 2020  coder(z).       
+00003610: 206c 6f73 7320 3d20 6e6e 2e66 756e 6374   loss = nn.funct
+00003620: 696f 6e61 6c2e 6d73 655f 6c6f 7373 2878  ional.mse_loss(x
+00003630: 5f68 6174 2c20 7829 0a20 2020 2020 2020  _hat, x).       
+00003640: 2023 204c 6f67 6769 6e67 2074 6f20 5465   # Logging to Te
+00003650: 6e73 6f72 426f 6172 6420 2869 6620 696e  nsorBoard (if in
+00003660: 7374 616c 6c65 6429 2062 7920 6465 6661  stalled) by defa
+00003670: 756c 740a 2020 2020 2020 2020 7365 6c66  ult.        self
+00003680: 2e6c 6f67 2822 7465 7374 5f6c 6f73 7322  .log("test_loss"
+00003690: 2c20 6c6f 7373 290a 2020 2020 2020 2020  , loss).        
+000036a0: 7265 7475 726e 206c 6f73 730a 0a20 2020  return loss..   
+000036b0: 2064 6566 2063 6f6e 6669 6775 7265 5f6f   def configure_o
+000036c0: 7074 696d 697a 6572 7328 7365 6c66 293a  ptimizers(self):
+000036d0: 0a20 2020 2020 2020 206f 7074 696d 697a  .        optimiz
+000036e0: 6572 203d 206f 7074 696d 2e41 6461 6d28  er = optim.Adam(
+000036f0: 7365 6c66 2e70 6172 616d 6574 6572 7328  self.parameters(
+00003700: 292c 206c 723d 3165 2d33 290a 2020 2020  ), lr=1e-3).    
+00003710: 2020 2020 7265 7475 726e 206f 7074 696d      return optim
+00003720: 697a 6572 0a0a 0a23 2069 6e69 7420 7468  izer...# init th
+00003730: 6520 6175 746f 656e 636f 6465 720a 6175  e autoencoder.au
+00003740: 746f 656e 636f 6465 7220 3d20 4c69 7441  toencoder = LitA
+00003750: 7574 6f45 6e63 6f64 6572 2865 6e63 6f64  utoEncoder(encod
+00003760: 6572 2c20 6465 636f 6465 7229 0a0a 2320  er, decoder)..# 
+00003770: 7365 7475 7020 6461 7461 0a64 6174 6173  setup data.datas
+00003780: 6574 203d 204d 4e49 5354 286f 732e 6765  et = MNIST(os.ge
+00003790: 7463 7764 2829 2c20 7472 6169 6e3d 5472  tcwd(), train=Tr
+000037a0: 7565 2c20 646f 776e 6c6f 6164 3d54 7275  ue, download=Tru
+000037b0: 652c 2074 7261 6e73 666f 726d 3d54 6f54  e, transform=ToT
+000037c0: 656e 736f 7228 2929 0a74 7261 696e 5f64  ensor()).train_d
+000037d0: 6174 6173 6574 2c20 7661 6c5f 6461 7461  ataset, val_data
+000037e0: 7365 7420 3d20 7574 696c 732e 6461 7461  set = utils.data
+000037f0: 2e72 616e 646f 6d5f 7370 6c69 7428 6461  .random_split(da
+00003800: 7461 7365 742c 205b 3535 3030 302c 2035  taset, [55000, 5
+00003810: 3030 305d 290a 7465 7374 5f64 6174 6173  000]).test_datas
+00003820: 6574 203d 204d 4e49 5354 286f 732e 6765  et = MNIST(os.ge
+00003830: 7463 7764 2829 2c20 7472 6169 6e3d 4661  tcwd(), train=Fa
+00003840: 6c73 652c 2064 6f77 6e6c 6f61 643d 5472  lse, download=Tr
+00003850: 7565 2c20 7472 616e 7366 6f72 6d3d 546f  ue, transform=To
+00003860: 5465 6e73 6f72 2829 290a 0a74 7261 696e  Tensor())..train
+00003870: 5f6c 6f61 6465 7220 3d20 7574 696c 732e  _loader = utils.
+00003880: 6461 7461 2e44 6174 614c 6f61 6465 7228  data.DataLoader(
+00003890: 7472 6169 6e5f 6461 7461 7365 7429 0a76  train_dataset).v
+000038a0: 616c 5f6c 6f61 6465 7220 3d20 7574 696c  al_loader = util
+000038b0: 732e 6461 7461 2e44 6174 614c 6f61 6465  s.data.DataLoade
+000038c0: 7228 7661 6c5f 6461 7461 7365 7429 0a74  r(val_dataset).t
+000038d0: 6573 745f 6c6f 6164 6572 203d 2075 7469  est_loader = uti
+000038e0: 6c73 2e64 6174 612e 4461 7461 4c6f 6164  ls.data.DataLoad
+000038f0: 6572 2874 6573 745f 6461 7461 7365 7429  er(test_dataset)
+00003900: 0a0a 7377 616e 6c61 625f 6c6f 6767 6572  ..swanlab_logger
+00003910: 203d 2053 7761 6e4c 6162 4c6f 6767 6572   = SwanLabLogger
+00003920: 280a 2020 2020 7072 6f6a 6563 743d 2273  (.    project="s
+00003930: 7761 6e6c 6162 5f65 7861 6d70 6c65 222c  wanlab_example",
+00003940: 0a20 2020 2065 7870 6572 696d 656e 745f  .    experiment_
+00003950: 6e61 6d65 3d22 6578 616d 706c 655f 6578  name="example_ex
+00003960: 7065 7269 6d65 6e74 222c 0a20 2020 2063  periment",.    c
+00003970: 6c6f 7564 3d46 616c 7365 2c0a 290a 0a74  loud=False,.)..t
+00003980: 7261 696e 6572 203d 2070 6c2e 5472 6169  rainer = pl.Trai
+00003990: 6e65 7228 6c69 6d69 745f 7472 6169 6e5f  ner(limit_train_
+000039a0: 6261 7463 6865 733d 3130 302c 206d 6178  batches=100, max
+000039b0: 5f65 706f 6368 733d 352c 206c 6f67 6765  _epochs=5, logge
+000039c0: 723d 7377 616e 6c61 625f 6c6f 6767 6572  r=swanlab_logger
+000039d0: 290a 0a74 7261 696e 6572 2e66 6974 286d  )..trainer.fit(m
+000039e0: 6f64 656c 3d61 7574 6f65 6e63 6f64 6572  odel=autoencoder
+000039f0: 2c20 7472 6169 6e5f 6461 7461 6c6f 6164  , train_dataload
+00003a00: 6572 733d 7472 6169 6e5f 6c6f 6164 6572  ers=train_loader
+00003a10: 2c20 7661 6c5f 6461 7461 6c6f 6164 6572  , val_dataloader
+00003a20: 733d 7661 6c5f 6c6f 6164 6572 290a 7472  s=val_loader).tr
+00003a30: 6169 6e65 722e 7465 7374 2864 6174 616c  ainer.test(datal
+00003a40: 6f61 6465 7273 3d74 6573 745f 6c6f 6164  oaders=test_load
+00003a50: 6572 290a 0a60 6060 0a0a 3c2f 6465 7461  er)..```..</deta
+00003a60: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
+00003a70: 3c73 756d 6d61 7279 3e0a 2020 3c73 7472  <summary>.  <str
+00003a80: 6f6e 673e 20f0 9fa4 9748 7567 6769 6e67  ong> ....Hugging
+00003a90: 4661 6365 2054 7261 6e73 666f 726d 6572  Face Transformer
+00003aa0: 733c 2f73 7472 6f6e 673e 0a3c 2f73 756d  s</strong>.</sum
+00003ab0: 6d61 7279 3e0a 0a3c 6272 3e0a 0a43 7265  mary>..<br>..Cre
+00003ac0: 6174 6520 616e 2069 6e73 7461 6e63 6520  ate an instance 
+00003ad0: 7573 696e 6720 6053 7761 6e4c 6162 4361  using `SwanLabCa
+00003ae0: 6c6c 6261 636b 6020 616e 6420 7061 7373  llback` and pass
+00003af0: 2069 7420 696e 746f 2074 6865 2060 6361   it into the `ca
+00003b00: 6c6c 6261 636b 7360 2070 6172 616d 6574  llbacks` paramet
+00003b10: 6572 206f 6620 6054 7261 696e 6572 6020  er of `Trainer` 
+00003b20: 746f 2065 6e61 626c 6520 5377 616e 4c61  to enable SwanLa
+00003b30: 6220 746f 0a72 6563 6f72 6420 7472 6169  b to.record trai
+00003b40: 6e69 6e67 206d 6574 7269 6373 2e0a 0a60  ning metrics...`
+00003b50: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00003b60: 6576 616c 7561 7465 0a69 6d70 6f72 7420  evaluate.import 
+00003b70: 6e75 6d70 7920 6173 206e 700a 696d 706f  numpy as np.impo
+00003b80: 7274 2073 7761 6e6c 6162 0a66 726f 6d20  rt swanlab.from 
+00003b90: 7377 616e 6c61 622e 696e 7465 6772 6174  swanlab.integrat
+00003ba0: 696f 6e2e 6875 6767 696e 6766 6163 6520  ion.huggingface 
+00003bb0: 696d 706f 7274 2053 7761 6e4c 6162 4361  import SwanLabCa
+00003bc0: 6c6c 6261 636b 0a66 726f 6d20 6461 7461  llback.from data
+00003bd0: 7365 7473 2069 6d70 6f72 7420 6c6f 6164  sets import load
+00003be0: 5f64 6174 6173 6574 0a66 726f 6d20 7472  _dataset.from tr
+00003bf0: 616e 7366 6f72 6d65 7273 2069 6d70 6f72  ansformers impor
+00003c00: 7420 4175 746f 4d6f 6465 6c46 6f72 5365  t AutoModelForSe
+00003c10: 7175 656e 6365 436c 6173 7369 6669 6361  quenceClassifica
+00003c20: 7469 6f6e 2c20 4175 746f 546f 6b65 6e69  tion, AutoTokeni
+00003c30: 7a65 722c 2054 7261 696e 6572 2c20 5472  zer, Trainer, Tr
+00003c40: 6169 6e69 6e67 4172 6775 6d65 6e74 730a  ainingArguments.
+00003c50: 0a0a 6465 6620 746f 6b65 6e69 7a65 5f66  ..def tokenize_f
+00003c60: 756e 6374 696f 6e28 6578 616d 706c 6573  unction(examples
+00003c70: 293a 0a20 2020 2072 6574 7572 6e20 746f  ):.    return to
+00003c80: 6b65 6e69 7a65 7228 6578 616d 706c 6573  kenizer(examples
+00003c90: 5b22 7465 7874 225d 2c20 7061 6464 696e  ["text"], paddin
+00003ca0: 673d 226d 6178 5f6c 656e 6774 6822 2c20  g="max_length", 
+00003cb0: 7472 756e 6361 7469 6f6e 3d54 7275 6529  truncation=True)
+00003cc0: 0a0a 0a64 6566 2063 6f6d 7075 7465 5f6d  ...def compute_m
+00003cd0: 6574 7269 6373 2865 7661 6c5f 7072 6564  etrics(eval_pred
+00003ce0: 293a 0a20 2020 206c 6f67 6974 732c 206c  ):.    logits, l
+00003cf0: 6162 656c 7320 3d20 6576 616c 5f70 7265  abels = eval_pre
+00003d00: 640a 2020 2020 7072 6564 6963 7469 6f6e  d.    prediction
+00003d10: 7320 3d20 6e70 2e61 7267 6d61 7828 6c6f  s = np.argmax(lo
+00003d20: 6769 7473 2c20 6178 6973 3d2d 3129 0a20  gits, axis=-1). 
+00003d30: 2020 2072 6574 7572 6e20 6d65 7472 6963     return metric
+00003d40: 2e63 6f6d 7075 7465 2870 7265 6469 6374  .compute(predict
+00003d50: 696f 6e73 3d70 7265 6469 6374 696f 6e73  ions=predictions
+00003d60: 2c20 7265 6665 7265 6e63 6573 3d6c 6162  , references=lab
+00003d70: 656c 7329 0a0a 0a64 6174 6173 6574 203d  els)...dataset =
+00003d80: 206c 6f61 645f 6461 7461 7365 7428 2279   load_dataset("y
+00003d90: 656c 705f 7265 7669 6577 5f66 756c 6c22  elp_review_full"
+00003da0: 290a 0a74 6f6b 656e 697a 6572 203d 2041  )..tokenizer = A
+00003db0: 7574 6f54 6f6b 656e 697a 6572 2e66 726f  utoTokenizer.fro
+00003dc0: 6d5f 7072 6574 7261 696e 6564 2822 6265  m_pretrained("be
+00003dd0: 7274 2d62 6173 652d 6361 7365 6422 290a  rt-base-cased").
+00003de0: 0a74 6f6b 656e 697a 6564 5f64 6174 6173  .tokenized_datas
+00003df0: 6574 7320 3d20 6461 7461 7365 742e 6d61  ets = dataset.ma
+00003e00: 7028 746f 6b65 6e69 7a65 5f66 756e 6374  p(tokenize_funct
+00003e10: 696f 6e2c 2062 6174 6368 6564 3d54 7275  ion, batched=Tru
+00003e20: 6529 0a0a 736d 616c 6c5f 7472 6169 6e5f  e)..small_train_
+00003e30: 6461 7461 7365 7420 3d20 746f 6b65 6e69  dataset = tokeni
+00003e40: 7a65 645f 6461 7461 7365 7473 5b22 7472  zed_datasets["tr
+00003e50: 6169 6e22 5d2e 7368 7566 666c 6528 7365  ain"].shuffle(se
+00003e60: 6564 3d34 3229 2e73 656c 6563 7428 7261  ed=42).select(ra
+00003e70: 6e67 6528 3130 3030 2929 0a73 6d61 6c6c  nge(1000)).small
+00003e80: 5f65 7661 6c5f 6461 7461 7365 7420 3d20  _eval_dataset = 
+00003e90: 746f 6b65 6e69 7a65 645f 6461 7461 7365  tokenized_datase
+00003ea0: 7473 5b22 7465 7374 225d 2e73 6875 6666  ts["test"].shuff
+00003eb0: 6c65 2873 6565 643d 3432 292e 7365 6c65  le(seed=42).sele
+00003ec0: 6374 2872 616e 6765 2831 3030 3029 290a  ct(range(1000)).
+00003ed0: 0a6d 6574 7269 6320 3d20 6576 616c 7561  .metric = evalua
+00003ee0: 7465 2e6c 6f61 6428 2261 6363 7572 6163  te.load("accurac
+00003ef0: 7922 290a 0a6d 6f64 656c 203d 2041 7574  y")..model = Aut
+00003f00: 6f4d 6f64 656c 466f 7253 6571 7565 6e63  oModelForSequenc
+00003f10: 6543 6c61 7373 6966 6963 6174 696f 6e2e  eClassification.
+00003f20: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
+00003f30: 2262 6572 742d 6261 7365 2d63 6173 6564  "bert-base-cased
+00003f40: 222c 206e 756d 5f6c 6162 656c 733d 3529  ", num_labels=5)
+00003f50: 0a0a 7472 6169 6e69 6e67 5f61 7267 7320  ..training_args 
+00003f60: 3d20 5472 6169 6e69 6e67 4172 6775 6d65  = TrainingArgume
+00003f70: 6e74 7328 0a20 2020 206f 7574 7075 745f  nts(.    output_
+00003f80: 6469 723d 2274 6573 745f 7472 6169 6e65  dir="test_traine
+00003f90: 7222 2c0a 2020 2020 7265 706f 7274 5f74  r",.    report_t
+00003fa0: 6f3d 226e 6f6e 6522 2c0a 2020 2020 6e75  o="none",.    nu
+00003fb0: 6d5f 7472 6169 6e5f 6570 6f63 6873 3d33  m_train_epochs=3
+00003fc0: 2c0a 2020 2020 6c6f 6767 696e 675f 7374  ,.    logging_st
+00003fd0: 6570 733d 3530 2c0a 290a 0a73 7761 6e6c  eps=50,.)..swanl
+00003fe0: 6162 5f63 616c 6c62 6163 6b20 3d20 5377  ab_callback = Sw
+00003ff0: 616e 4c61 6243 616c 6c62 6163 6b28 6578  anLabCallback(ex
+00004000: 7065 7269 6d65 6e74 5f6e 616d 653d 2254  periment_name="T
+00004010: 7261 6e73 666f 726d 6572 7354 6573 7422  ransformersTest"
+00004020: 2c20 636c 6f75 643d 4661 6c73 6529 0a0a  , cloud=False)..
+00004030: 7472 6169 6e65 7220 3d20 5472 6169 6e65  trainer = Traine
+00004040: 7228 0a20 2020 206d 6f64 656c 3d6d 6f64  r(.    model=mod
+00004050: 656c 2c0a 2020 2020 6172 6773 3d74 7261  el,.    args=tra
+00004060: 696e 696e 675f 6172 6773 2c0a 2020 2020  ining_args,.    
+00004070: 7472 6169 6e5f 6461 7461 7365 743d 736d  train_dataset=sm
+00004080: 616c 6c5f 7472 6169 6e5f 6461 7461 7365  all_train_datase
+00004090: 742c 0a20 2020 2065 7661 6c5f 6461 7461  t,.    eval_data
+000040a0: 7365 743d 736d 616c 6c5f 6576 616c 5f64  set=small_eval_d
+000040b0: 6174 6173 6574 2c0a 2020 2020 636f 6d70  ataset,.    comp
+000040c0: 7574 655f 6d65 7472 6963 733d 636f 6d70  ute_metrics=comp
+000040d0: 7574 655f 6d65 7472 6963 732c 0a20 2020  ute_metrics,.   
+000040e0: 2063 616c 6c62 6163 6b73 3d5b 7377 616e   callbacks=[swan
+000040f0: 6c61 625f 6361 6c6c 6261 636b 5d2c 0a29  lab_callback],.)
+00004100: 0a0a 7472 6169 6e65 722e 7472 6169 6e28  ..trainer.train(
+00004110: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
+00004120: 3e0a 0a3c 6465 7461 696c 733e 0a3c 7375  >..<details>.<su
+00004130: 6d6d 6172 793e 0a20 203c 7374 726f 6e67  mmary>.  <strong
+00004140: 3e20 4d4d 456e 6769 6e65 284d 4d44 6574  > MMEngine(MMDet
+00004150: 6563 7469 6f6e 2065 7463 2e29 3c2f 7374  ection etc.)</st
+00004160: 726f 6e67 3e0a 3c2f 7375 6d6d 6172 793e  rong>.</summary>
+00004170: 0a3c 6272 3e0a 0a49 6e74 6567 7261 7465  .<br>..Integrate
+00004180: 2060 5377 616e 6c61 6256 6973 4261 636b   `SwanlabVisBack
+00004190: 656e 6460 2069 6e74 6f20 4d4d 456e 6769  end` into MMEngi
+000041a0: 6e65 2074 6f20 656e 6162 6c65 2061 7574  ne to enable aut
+000041b0: 6f6d 6174 6963 206c 6f67 6769 6e67 206f  omatic logging o
+000041c0: 6620 7472 6169 6e69 6e67 206d 6574 7269  f training metri
+000041d0: 6373 2062 7920 5377 616e 4c61 622e 0a0a  cs by SwanLab...
+000041e0: 4164 6420 7468 6520 666f 6c6c 6f77 696e  Add the followin
+000041f0: 6720 636f 6465 2073 6e69 7070 6574 2074  g code snippet t
+00004200: 6f20 796f 7572 204d 4d20 636f 6e66 6967  o your MM config
+00004210: 2066 696c 6520 746f 2073 7461 7274 2074   file to start t
+00004220: 7261 696e 696e 673a 0a0a 6060 6070 7974  raining:..```pyt
+00004230: 686f 6e0a 6375 7374 6f6d 5f69 6d70 6f72  hon.custom_impor
+00004240: 7473 203d 2064 6963 7428 696d 706f 7274  ts = dict(import
+00004250: 733d 5b22 7377 616e 6c61 622e 696e 7465  s=["swanlab.inte
+00004260: 6772 6174 696f 6e2e 6d6d 656e 6769 6e65  gration.mmengine
+00004270: 225d 2c20 616c 6c6f 775f 6661 696c 6564  "], allow_failed
+00004280: 5f69 6d70 6f72 7473 3d46 616c 7365 290a  _imports=False).
+00004290: 0a76 6973 5f62 6163 6b65 6e64 7320 3d20  .vis_backends = 
+000042a0: 5b0a 2020 2020 6469 6374 280a 2020 2020  [.    dict(.    
+000042b0: 2020 2020 7479 7065 3d22 5377 616e 6c61      type="Swanla
+000042c0: 6256 6973 4261 636b 656e 6422 2c0a 2020  bVisBackend",.  
+000042d0: 2020 2020 2020 7361 7665 5f64 6972 3d22        save_dir="
+000042e0: 7275 6e73 2f73 7761 6e6c 6162 222c 0a20  runs/swanlab",. 
+000042f0: 2020 2020 2020 2069 6e69 745f 6b77 6172         init_kwar
+00004300: 6773 3d7b 0a20 2020 2020 2020 2020 2020  gs={.           
+00004310: 2022 7072 6f6a 6563 7422 3a20 2273 7761   "project": "swa
+00004320: 6e6c 6162 2d6d 6d65 6e67 696e 6522 2c0a  nlab-mmengine",.
+00004330: 2020 2020 2020 2020 7d2c 0a20 2020 2029          },.    )
+00004340: 2c0a 5d0a 0a76 6973 7561 6c69 7a65 7220  ,.]..visualizer 
+00004350: 3d20 6469 6374 280a 2020 2020 7479 7065  = dict(.    type
+00004360: 3d22 5669 7375 616c 697a 6572 222c 0a20  ="Visualizer",. 
+00004370: 2020 2076 6973 5f62 6163 6b65 6e64 733d     vis_backends=
+00004380: 7669 735f 6261 636b 656e 6473 2c0a 290a  vis_backends,.).
+00004390: 6060 600a 3c2f 6465 7461 696c 733e 0a0a  ```.</details>..
+000043a0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+000043b0: 7279 3e0a 2020 3c73 7472 6f6e 673e 2055  ry>.  <strong> U
+000043c0: 6c74 7261 6c79 7469 6373 3c2f 7374 726f  ltralytics</stro
+000043d0: 6e67 3e0a 3c2f 7375 6d6d 6172 793e 0a3c  ng>.</summary>.<
+000043e0: 6272 3e0a 0a49 6e74 6567 7261 7469 6e67  br>..Integrating
+000043f0: 2053 7761 6e4c 6162 2069 6e74 6f20 556c   SwanLab into Ul
+00004400: 7472 616c 7974 6963 7320 6973 2076 6572  tralytics is ver
+00004410: 7920 7369 6d70 6c65 3b20 796f 7520 6361  y simple; you ca
+00004420: 6e20 7573 6520 7468 6520 6061 6464 5f73  n use the `add_s
+00004430: 7761 6e6c 6162 5f63 616c 6c62 6163 6b60  wanlab_callback`
+00004440: 2066 756e 6374 696f 6e3a 0a0a 6060 6070   function:..```p
+00004450: 7974 686f 6e0a 6672 6f6d 2075 6c74 7261  ython.from ultra
+00004460: 6c79 7469 6373 2069 6d70 6f72 7420 594f  lytics import YO
+00004470: 4c4f 0a66 726f 6d20 7377 616e 6c61 622e  LO.from swanlab.
+00004480: 696e 7465 6772 6174 696f 6e2e 756c 7472  integration.ultr
+00004490: 616c 7974 6963 7320 696d 706f 7274 2061  alytics import a
+000044a0: 6464 5f73 7761 6e6c 6162 5f63 616c 6c62  dd_swanlab_callb
+000044b0: 6163 6b0a 0a6d 6f64 656c 203d 2059 4f4c  ack..model = YOL
+000044c0: 4f28 2279 6f6c 6f76 386e 2e79 616d 6c22  O("yolov8n.yaml"
+000044d0: 290a 6d6f 6465 6c2e 6c6f 6164 2829 0a0a  ).model.load()..
+000044e0: 6164 645f 7377 616e 6c61 625f 6361 6c6c  add_swanlab_call
+000044f0: 6261 636b 286d 6f64 656c 290a 0a6d 6f64  back(model)..mod
+00004500: 656c 2e74 7261 696e 280a 2020 2020 6461  el.train(.    da
+00004510: 7461 3d22 2e2f 636f 636f 2e79 616d 6c22  ta="./coco.yaml"
+00004520: 2c0a 2020 2020 6570 6f63 6873 3d35 302c  ,.    epochs=50,
+00004530: 200a 2020 2020 696d 6773 7a3d 3332 302c   .    imgsz=320,
+00004540: 0a29 0a60 6060 0a0a 3c2f 6465 7461 696c  .).```..</detail
+00004550: 733e 0a0a 0a0a 3c62 723e 0a0a 2323 20f0  s>....<br>..## .
+00004560: 9f86 9a20 436f 6d70 6172 6973 6f6e 2077  ... Comparison w
+00004570: 6974 6820 6661 6d69 6c69 6172 2074 6f6f  ith familiar too
+00004580: 6c73 0a0a 2323 2320 5465 6e73 6f72 626f  ls..### Tensorbo
+00004590: 6172 6420 7673 2053 7761 6e4c 6162 0a0a  ard vs SwanLab..
+000045a0: 2d20 2a2a e298 81ef b88f 204f 6e6c 696e  - **...... Onlin
+000045b0: 6520 5573 6167 6520 5375 7070 6f72 742a  e Usage Support*
+000045c0: 2a3a 0a20 2057 6974 6820 5377 616e 4c61  *:.  With SwanLa
+000045d0: 622c 2074 7261 696e 696e 6720 6578 7065  b, training expe
+000045e0: 7269 6d65 6e74 7320 6361 6e20 6265 2063  riments can be c
+000045f0: 6f6e 7665 6e69 656e 746c 7920 7379 6e63  onveniently sync
+00004600: 6872 6f6e 697a 6564 2061 6e64 2073 6176  hronized and sav
+00004610: 6564 2069 6e20 7468 6520 636c 6f75 642c  ed in the cloud,
+00004620: 2061 6c6c 6f77 696e 6720 666f 7220 7265   allowing for re
+00004630: 6d6f 7465 0a20 206d 6f6e 6974 6f72 696e  mote.  monitorin
+00004640: 6720 6f66 2074 7261 696e 696e 6720 7072  g of training pr
+00004650: 6f67 7265 7373 2c20 6d61 6e61 6769 6e67  ogress, managing
+00004660: 2068 6973 746f 7269 6361 6c20 7072 6f6a   historical proj
+00004670: 6563 7473 2c20 7368 6172 696e 6720 6578  ects, sharing ex
+00004680: 7065 7269 6d65 6e74 206c 696e 6b73 2c20  periment links, 
+00004690: 7365 6e64 696e 6720 7265 616c 2d74 696d  sending real-tim
+000046a0: 650a 2020 6e6f 7469 6669 6361 7469 6f6e  e.  notification
+000046b0: 206d 6573 7361 6765 732c 2061 6e64 2076   messages, and v
+000046c0: 6965 7769 6e67 2065 7870 6572 696d 656e  iewing experimen
+000046d0: 7473 2061 6372 6f73 7320 6d75 6c74 6970  ts across multip
+000046e0: 6c65 2064 6576 6963 6573 2e20 496e 2063  le devices. In c
+000046f0: 6f6e 7472 6173 742c 2054 656e 736f 7242  ontrast, TensorB
+00004700: 6f61 7264 2069 7320 616e 206f 6666 6c69  oard is an offli
+00004710: 6e65 0a20 2065 7870 6572 696d 656e 7420  ne.  experiment 
+00004720: 7472 6163 6b69 6e67 2074 6f6f 6c2e 0a0a  tracking tool...
+00004730: 2d20 2a2a f09f 91a5 2043 6f6c 6c61 626f  - **.... Collabo
+00004740: 7261 7469 7665 204d 756c 7469 2d75 7365  rative Multi-use
+00004750: 7220 456e 7669 726f 6e6d 656e 742a 2a3a  r Environment**:
+00004760: 0a20 2053 7761 6e4c 6162 2066 6163 696c  .  SwanLab facil
+00004770: 6974 6174 6573 2065 6173 7920 6d61 6e61  itates easy mana
+00004780: 6765 6d65 6e74 206f 6620 6d75 6c74 692d  gement of multi-
+00004790: 7065 7273 6f6e 2074 7261 696e 696e 6720  person training 
+000047a0: 7072 6f6a 6563 7473 2061 6e64 2073 6861  projects and sha
+000047b0: 7269 6e67 206f 6620 6578 7065 7269 6d65  ring of experime
+000047c0: 6e74 206c 696e 6b73 2066 6f72 0a20 2063  nt links for.  c
+000047d0: 6f6c 6c61 626f 7261 7469 7665 206d 6163  ollaborative mac
+000047e0: 6869 6e65 206c 6561 726e 696e 6720 6163  hine learning ac
+000047f0: 726f 7373 2074 6561 6d73 2e20 4974 2061  ross teams. It a
+00004800: 6c73 6f20 656e 6162 6c65 7320 6372 6f73  lso enables cros
+00004810: 732d 7370 6163 6520 636f 6d6d 756e 6963  s-space communic
+00004820: 6174 696f 6e20 616e 6420 6469 7363 7573  ation and discus
+00004830: 7369 6f6e 2e20 4f6e 2074 6865 206f 7468  sion. On the oth
+00004840: 6572 0a20 2068 616e 642c 2054 656e 736f  er.  hand, Tenso
+00004850: 7242 6f61 7264 2069 7320 7072 696d 6172  rBoard is primar
+00004860: 696c 7920 6465 7369 676e 6564 2066 6f72  ily designed for
+00004870: 2069 6e64 6976 6964 7561 6c20 7573 652c   individual use,
+00004880: 206d 616b 696e 6720 6974 2064 6966 6669   making it diffi
+00004890: 6375 6c74 2074 6f20 636f 6c6c 6162 6f72  cult to collabor
+000048a0: 6174 6520 616e 6420 7368 6172 6520 6578  ate and share ex
+000048b0: 7065 7269 6d65 6e74 730a 2020 7769 7468  periments.  with
+000048c0: 206d 756c 7469 706c 6520 7573 6572 732e   multiple users.
+000048d0: 0a0a 2d20 2a2a f09f 92bb 2050 6572 7369  ..- **.... Persi
+000048e0: 7374 656e 742c 2043 656e 7472 616c 697a  stent, Centraliz
+000048f0: 6564 2044 6173 6862 6f61 7264 2a2a 3a0a  ed Dashboard**:.
+00004900: 2020 5265 6761 7264 6c65 7373 206f 6620    Regardless of 
+00004910: 7768 6572 6520 796f 7520 6172 6520 7472  where you are tr
+00004920: 6169 6e69 6e67 2079 6f75 7220 6d6f 6465  aining your mode
+00004930: 6c73 2c20 6265 2069 7420 6f6e 2061 206c  ls, be it on a l
+00004940: 6f63 616c 2063 6f6d 7075 7465 722c 2061  ocal computer, a
+00004950: 206c 6162 2063 6c75 7374 6572 2c20 6f72   lab cluster, or
+00004960: 206f 6e20 7075 626c 6963 2063 6c6f 7564   on public cloud
+00004970: 2047 5055 0a20 2069 6e73 7461 6e63 6573   GPU.  instances
+00004980: 2c20 796f 7572 2072 6573 756c 7473 2061  , your results a
+00004990: 7265 206c 6f67 6765 6420 746f 2074 6865  re logged to the
+000049a0: 2073 616d 6520 6365 6e74 7261 6c69 7a65   same centralize
+000049b0: 6420 6461 7368 626f 6172 642e 2055 7369  d dashboard. Usi
+000049c0: 6e67 2054 656e 736f 7242 6f61 7264 2c20  ng TensorBoard, 
+000049d0: 6f6e 2074 6865 206f 7468 6572 2068 616e  on the other han
+000049e0: 642c 2072 6571 7569 7265 730a 2020 7370  d, requires.  sp
+000049f0: 656e 6469 6e67 2074 696d 6520 636f 7079  ending time copy
+00004a00: 696e 6720 616e 6420 6d61 6e61 6769 6e67  ing and managing
+00004a10: 2054 4645 7665 6e74 2066 696c 6573 2066   TFEvent files f
+00004a20: 726f 6d20 6469 6666 6572 656e 7420 6d61  rom different ma
+00004a30: 6368 696e 6573 2e0a 0a2d 202a 2af0 9f92  chines...- **...
+00004a40: aa20 4d6f 7265 2050 6f77 6572 6675 6c20  . More Powerful 
+00004a50: 5461 626c 6573 2a2a 3a0a 2020 5377 616e  Tables**:.  Swan
+00004a60: 4c61 6220 7461 626c 6573 2061 6c6c 6f77  Lab tables allow
+00004a70: 2079 6f75 2074 6f20 7669 6577 2c20 7365   you to view, se
+00004a80: 6172 6368 2c20 616e 6420 6669 6c74 6572  arch, and filter
+00004a90: 2072 6573 756c 7473 2066 726f 6d20 7661   results from va
+00004aa0: 7269 6f75 7320 6578 7065 7269 6d65 6e74  rious experiment
+00004ab0: 732c 206d 616b 696e 6720 6974 2065 6173  s, making it eas
+00004ac0: 7920 746f 2072 6576 6965 770a 2020 7468  y to review.  th
+00004ad0: 6f75 7361 6e64 7320 6f66 206d 6f64 656c  ousands of model
+00004ae0: 2076 6572 7369 6f6e 7320 746f 2066 696e   versions to fin
+00004af0: 6420 7468 6520 6265 7374 2d70 6572 666f  d the best-perfo
+00004b00: 726d 696e 6720 6d6f 6465 6c73 2066 6f72  rming models for
+00004b10: 2064 6966 6665 7265 6e74 2074 6173 6b73   different tasks
+00004b20: 2e20 5465 6e73 6f72 426f 6172 6420 6973  . TensorBoard is
+00004b30: 206e 6f74 2077 656c 6c2d 7375 6974 6564   not well-suited
+00004b40: 2066 6f72 0a20 206c 6172 6765 2d73 6361   for.  large-sca
+00004b50: 6c65 2070 726f 6a65 6374 732e 0a0a 2323  le projects...##
+00004b60: 2320 5765 6967 6874 7320 616e 6420 4269  # Weights and Bi
+00004b70: 6173 6573 2076 7320 5377 616e 4c61 620a  ases vs SwanLab.
+00004b80: 0a2d 2057 6569 6768 7473 2061 6e64 2042  .- Weights and B
+00004b90: 6961 7365 7320 6973 2061 6e20 6f6e 6c69  iases is an onli
+00004ba0: 6e65 2d6f 6e6c 792c 2070 726f 7072 6965  ne-only, proprie
+00004bb0: 7461 7279 204d 4c4f 7073 2070 6c61 7466  tary MLOps platf
+00004bc0: 6f72 6d2e 0a0a 2d20 4e6f 7420 6f6e 6c79  orm...- Not only
+00004bd0: 2064 6f65 7320 5377 616e 4c61 6220 7375   does SwanLab su
+00004be0: 7070 6f72 7420 6f6e 6c69 6e65 2075 7361  pport online usa
+00004bf0: 6765 2c20 6275 7420 6974 2061 6c73 6f20  ge, but it also 
+00004c00: 6f66 6665 7273 2061 6e20 6f70 656e 2d73  offers an open-s
+00004c10: 6f75 7263 652c 2066 7265 652c 2061 6e64  ource, free, and
+00004c20: 2073 656c 662d 686f 7374 6564 2076 6572   self-hosted ver
+00004c30: 7369 6f6e 2e0a 0a3c 6272 3e0a 0a23 2320  sion...<br>..## 
+00004c40: f09f 9ba3 efb8 8f20 526f 6164 6d61 700a  ....... Roadmap.
+00004c50: 0a54 6f6f 6c73 2065 766f 6c76 6520 696e  .Tools evolve in
+00004c60: 2069 7465 7261 7469 6f6e 2061 6e64 2066   iteration and f
+00004c70: 6565 6462 6163 6b7e 2c20 7765 6c63 6f6d  eedback~, welcom
+00004c80: 650a 746f 205b 7375 626d 6974 2066 6561  e.to [submit fea
+00004c90: 7475 7265 2073 7567 6765 7374 696f 6e73  ture suggestions
+00004ca0: 5d28 6874 7470 733a 2f2f 6765 656b 7465  ](https://geekte
+00004cb0: 6368 7374 7564 696f 2e66 6569 7368 752e  chstudio.feishu.
+00004cc0: 636e 2f73 6861 7265 2f62 6173 652f 666f  cn/share/base/fo
+00004cd0: 726d 2f73 6872 636e 7942 6c4b 384f 4d44  rm/shrcnyBlK8OMD
+00004ce0: 3065 7765 6f46 6363 3253 7657 4b63 290a  0eweoFcc2SvWKc).
+00004cf0: 0a23 2323 2049 6e20 5072 6f67 7265 7373  .### In Progress
+00004d00: 204e 6f77 0a0a 2d20 6054 6162 6c65 603a   Now..- `Table`:
+00004d10: 204d 6f72 6520 666c 6578 6962 6c65 206d   More flexible m
+00004d20: 756c 7469 6469 6d65 6e73 696f 6e61 6c20  ultidimensional 
+00004d30: 7461 626c 6520 6368 6172 7473 2c20 7375  table charts, su
+00004d40: 6974 6162 6c65 2066 6f72 204c 4c4d 2c20  itable for LLM, 
+00004d50: 4149 4743 2c20 6d6f 6465 6c20 6576 616c  AIGC, model eval
+00004d60: 7561 7469 6f6e 2061 6e64 206f 7468 6572  uation and other
+00004d70: 2073 6365 6e61 7269 6f73 2e0a 0a2d 202a   scenarios...- *
+00004d80: 2a45 6d61 696c 206e 6f74 6966 6963 6174  *Email notificat
+00004d90: 696f 6ef0 9f93 a72a 2a3a 2057 6865 6e20  ion....**: When 
+00004da0: 7472 6169 6e69 6e67 2069 7320 696e 7465  training is inte
+00004db0: 7272 7570 7465 6420 756e 6578 7065 6374  rrupted unexpect
+00004dc0: 6564 6c79 2c20 7768 656e 2074 7261 696e  edly, when train
+00004dd0: 696e 6720 6973 2063 6f6d 706c 6574 6564  ing is completed
+00004de0: 2c20 616e 6420 7768 656e 2063 7573 746f  , and when custo
+00004df0: 6d0a 2020 7369 7475 6174 696f 6e73 206f  m.  situations o
+00004e00: 6363 7572 2c20 7365 6e64 206e 6f74 6966  ccur, send notif
+00004e10: 6963 6174 696f 6e20 656d 6169 6c73 2e0a  ication emails..
+00004e20: 0a23 2323 204e 6578 7420 506c 616e 6e65  .### Next Planne
+00004e30: 640a 0a2d 2060 4d6f 6c65 6375 6c65 603a  d..- `Molecule`:
+00004e40: 2056 6973 7561 6c69 7a61 7469 6f6e 2063   Visualization c
+00004e50: 6861 7274 7320 6f66 2062 696f 6368 656d  harts of biochem
+00004e60: 6973 7472 7920 6d6f 6c65 6375 6c65 730a  istry molecules.
+00004e70: 0a2d 2060 506c 6f74 603a 2046 7265 6520  .- `Plot`: Free 
+00004e80: 6368 6172 7420 6472 6177 696e 6720 6d65  chart drawing me
+00004e90: 7468 6f64 0a0a 2d20 6041 7069 603a 2041  thod..- `Api`: A
+00004ea0: 6363 6573 7320 5377 616e 4c61 6220 6461  ccess SwanLab da
+00004eb0: 7461 2074 6872 6f75 6768 2041 5049 2e0a  ta through API..
+00004ec0: 0a2d 202a 2a53 7973 7465 6d20 6861 7264  .- **System hard
+00004ed0: 7761 7265 2072 6563 6f72 6473 2a2a 3a20  ware records**: 
+00004ee0: 5265 636f 7264 2061 2073 6572 6965 7320  Record a series 
+00004ef0: 6f66 2068 6172 6477 6172 6520 636f 6e64  of hardware cond
+00004f00: 6974 696f 6e73 2073 7563 6820 6173 2047  itions such as G
+00004f10: 5055 2c20 4350 552c 2064 6973 6b2c 206e  PU, CPU, disk, n
+00004f20: 6574 776f 726b 2c20 6574 632e 0a0a 2d20  etwork, etc...- 
+00004f30: 2a2a 436f 6465 2072 6563 6f72 6473 2a2a  **Code records**
+00004f40: 3a20 5265 636f 7264 2074 7261 696e 696e  : Record trainin
+00004f50: 6720 636f 6465 0a0a 2d20 2a2a 4d6f 7265  g code..- **More
+00004f60: 2069 6e74 6567 7261 7469 6f6e 732a 2a3a   integrations**:
+00004f70: 204c 6967 6874 4742 4d2c 2058 4742 6f6f   LightGBM, XGBoo
+00004f80: 7374 2c20 6f70 656e 6169 2c20 6368 6174  st, openai, chat
+00004f90: 676c 6d2c 206d 6d20 7365 7269 6573 2c2e  glm, mm series,.
+00004fa0: 2e2e 0a2d 202e 2e2e 0a0a 2323 2320 4c6f  ...- .....### Lo
+00004fb0: 6e67 2d74 6572 6d20 436f 6e63 6572 6e0a  ng-term Concern.
+00004fc0: 0a2d 2054 6865 206d 6f73 7420 6265 6e65  .- The most bene
+00004fd0: 6669 6369 616c 2063 6f6c 6c61 626f 7261  ficial collabora
+00004fe0: 7469 7665 2077 6179 2066 6f72 2041 4920  tive way for AI 
+00004ff0: 7465 616d 2069 6e6e 6f76 6174 696f 6e0a  team innovation.
+00005000: 0a2d 2054 6865 206d 6f73 7420 7573 6572  .- The most user
+00005010: 2d66 7269 656e 646c 7920 5549 2069 6e74  -friendly UI int
+00005020: 6572 6163 7469 6f6e 0a0a 2d20 5669 6577  eraction..- View
+00005030: 696e 6720 6578 7065 7269 6d65 6e74 7320  ing experiments 
+00005040: 6f6e 206d 6f62 696c 650a 0a3c 6272 3e0a  on mobile..<br>.
+00005050: 0a23 2320 f09f 91a5 2043 6f6d 6d75 6e69  .## .... Communi
+00005060: 7479 0a0a 2323 2320 436f 6d6d 756e 6974  ty..### Communit
+00005070: 7920 616e 6420 7375 7070 6f72 740a 0a2d  y and support..-
+00005080: 205b 4769 7448 7562 2049 7373 7565 735d   [GitHub Issues]
+00005090: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000050a0: 636f 6d2f 5377 616e 4875 6258 2f53 7761  com/SwanHubX/Swa
+000050b0: 6e4c 6162 2f69 7373 7565 7329 efbc 9a45  nLab/issues)...E
+000050c0: 7272 6f72 7320 616e 6420 6973 7375 6573  rrors and issues
+000050d0: 2065 6e63 6f75 6e74 6572 6564 2077 6865   encountered whe
+000050e0: 6e20 7573 696e 6720 5377 616e 4c61 620a  n using SwanLab.
+000050f0: 2d20 5b45 6d61 696c 2073 7570 706f 7274  - [Email support
+00005100: 5d28 7a65 7969 2e6c 696e 4073 7761 6e68  ](zeyi.lin@swanh
+00005110: 7562 2e63 6f29 efbc 9a46 6565 6462 6163  ub.co)...Feedbac
+00005120: 6b20 6f6e 2069 7373 7565 7320 7769 7468  k on issues with
+00005130: 2075 7369 6e67 2053 7761 6e4c 6162 0a2d   using SwanLab.-
+00005140: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00005150: 2f2f 6765 656b 7465 6368 7374 7564 696f  //geektechstudio
+00005160: 2e66 6569 7368 752e 636e 2f77 696b 692f  .feishu.cn/wiki/
+00005170: 4e49 5a39 7770 354c 5269 5371 5179 6b69  NIZ9wp5LRiSqQyki
+00005180: 7a62 4763 567a 554b 6e69 6322 3e57 6543  zbGcVzUKnic">WeC
+00005190: 6861 743c 2f61 3eef bc9a 4469 7363 7573  hat</a>...Discus
+000051a0: 7320 6973 7375 6573 2075 7369 6e67 2053  s issues using S
+000051b0: 7761 6e4c 6162 2c0a 2020 7368 6172 6520  wanLab,.  share 
+000051c0: 7468 6520 6c61 7465 7374 2041 4920 7465  the latest AI te
+000051d0: 6368 6e6f 6c6f 6779 2e0a 0a23 2323 2053  chnology...### S
+000051e0: 7761 6e4c 6162 2052 4541 444d 4520 4261  wanLab README Ba
+000051f0: 6467 650a 0a49 6620 796f 7520 6c69 6b65  dge..If you like
+00005200: 2074 6f20 7573 6520 5377 616e 4c61 6220   to use SwanLab 
+00005210: 696e 2079 6f75 7220 776f 726b 2c20 706c  in your work, pl
+00005220: 6561 7365 2061 6464 2074 6865 2053 7761  ease add the Swa
+00005230: 6e4c 6162 2062 6164 6765 2074 6f20 796f  nLab badge to yo
+00005240: 7572 2052 4541 444d 453a 0a0a 5b21 5b73  ur README:..[![s
+00005250: 7761 6e6c 6162 5d28 6874 7470 733a 2f2f  wanlab](https://
+00005260: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00005270: 6164 6765 2f70 6f77 6572 6564 2532 3062  adge/powered%20b
+00005280: 792d 5377 616e 4c61 622d 3433 3834 3430  y-SwanLab-438440
+00005290: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+000052a0: 622e 636f 6d2f 7377 616e 6875 6278 2f73  b.com/swanhubx/s
+000052b0: 7761 6e6c 6162 290a 0a60 6060 0a5b 215b  wanlab)..```.[![
+000052c0: 7377 616e 6c61 625d 2868 7474 7073 3a2f  swanlab](https:/
+000052d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000052e0: 6261 6467 652f 706f 7765 7265 6425 3230  badge/powered%20
+000052f0: 6279 2d53 7761 6e4c 6162 2d34 3338 3434  by-SwanLab-43844
+00005300: 3029 5d28 6874 7470 733a 2f2f 6769 7468  0)](https://gith
+00005310: 7562 2e63 6f6d 2f73 7761 6e68 7562 782f  ub.com/swanhubx/
+00005320: 7377 616e 6c61 6229 0a60 6060 0a0a 2323  swanlab).```..##
+00005330: 2320 4369 7469 6e67 2053 7761 6e4c 6162  # Citing SwanLab
+00005340: 2069 6e20 7468 6520 7061 7065 720a 0a49   in the paper..I
+00005350: 6620 796f 7520 6669 6e64 2053 7761 6e4c  f you find SwanL
+00005360: 6162 2068 656c 7066 756c 2066 6f72 2079  ab helpful for y
+00005370: 6f75 7220 7265 7365 6172 6368 206a 6f75  our research jou
+00005380: 726e 6579 2c20 706c 6561 7365 2063 6f6e  rney, please con
+00005390: 7369 6465 7220 6369 7469 6e67 2069 6e20  sider citing in 
+000053a0: 7468 6520 666f 6c6c 6f77 696e 6720 666f  the following fo
+000053b0: 726d 6174 3a0a 0a60 6060 6269 6274 6578  rmat:..```bibtex
+000053c0: 0a40 736f 6674 7761 7265 7b5a 6579 696c  .@software{Zeyil
+000053d0: 696e 5f53 7761 6e4c 6162 5f32 3032 332c  in_SwanLab_2023,
+000053e0: 0a20 2061 7574 686f 7220 3d20 7b5a 6579  .  author = {Zey
+000053f0: 6920 4c69 6e2c 2053 6861 6f68 6f6e 6720  i Lin, Shaohong 
+00005400: 4368 656e 2c20 4b61 6e67 204c 692c 2051  Chen, Kang Li, Q
+00005410: 6975 7368 616e 204a 6961 6e67 2c20 5a69  iushan Jiang, Zi
+00005420: 7275 6920 4361 692c 2020 4b61 6966 616e  rui Cai,  Kaifan
+00005430: 6720 4a69 2061 6e64 207b 5468 6520 5377  g Ji and {The Sw
+00005440: 616e 4c61 6220 7465 616d 7d7d 2c0a 2020  anLab team}},.  
+00005450: 646f 6920 3d20 7b31 302e 3532 3831 2f7a  doi = {10.5281/z
+00005460: 656e 6f64 6f2e 3131 3130 3035 3530 7d2c  enodo.11100550},
+00005470: 0a20 206c 6963 656e 7365 203d 207b 4170  .  license = {Ap
+00005480: 6163 6865 2d32 2e30 7d2c 0a20 2074 6974  ache-2.0},.  tit
+00005490: 6c65 203d 207b 7b53 7761 6e4c 6162 7d7d  le = {{SwanLab}}
+000054a0: 2c0a 2020 7572 6c20 3d20 7b68 7474 7073  ,.  url = {https
+000054b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7377  ://github.com/sw
+000054c0: 616e 6875 6278 2f73 7761 6e6c 6162 7d2c  anhubx/swanlab},
+000054d0: 0a20 2079 6561 7220 3d20 7b32 3032 337d  .  year = {2023}
+000054e0: 0a7d 0a60 6060 0a0a 2323 2320 436f 6e74  .}.```..### Cont
+000054f0: 7269 6275 7465 2074 6f20 5377 616e 4c61  ribute to SwanLa
+00005500: 620a 0a43 6f6e 7369 6465 7269 6e67 2063  b..Considering c
+00005510: 6f6e 7472 6962 7574 696e 6720 746f 2053  ontributing to S
+00005520: 7761 6e4c 6162 3f20 4669 7273 742c 2070  wanLab? First, p
+00005530: 6c65 6173 6520 7461 6b65 2073 6f6d 6520  lease take some 
+00005540: 7469 6d65 2074 6f20 7265 6164 0a74 6865  time to read.the
+00005550: 205b 436f 6e74 7269 6275 7469 6f6e 2047   [Contribution G
+00005560: 7569 6465 6c69 6e65 735d 2843 4f4e 5452  uidelines](CONTR
+00005570: 4942 5554 494e 472e 6d64 292e 0a0a 4174  IBUTING.md)...At
+00005580: 2074 6865 2073 616d 6520 7469 6d65 2c20   the same time, 
+00005590: 7765 2077 6172 6d6c 7920 7765 6c63 6f6d  we warmly welcom
+000055a0: 6520 7375 7070 6f72 7420 666f 7220 5377  e support for Sw
+000055b0: 616e 4c61 6220 7468 726f 7567 6820 736f  anLab through so
+000055c0: 6369 616c 206d 6564 6961 2c20 6576 656e  cial media, even
+000055d0: 7473 2c20 616e 6420 636f 6e66 6572 656e  ts, and conferen
+000055e0: 6365 2073 6861 7269 6e67 2e20 5468 616e  ce sharing. Than
+000055f0: 6b20 796f 7521 0a0a 3c62 723e 0a0a 2a2a  k you!..<br>..**
+00005600: 436f 6e74 7269 6275 746f 7273 2a2a 0a0a  Contributors**..
+00005610: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00005620: 2f67 6974 6875 622e 636f 6d2f 7377 616e  /github.com/swan
+00005630: 6875 6278 2f73 7761 6e6c 6162 2f67 7261  hubx/swanlab/gra
+00005640: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
+00005650: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
+00005660: 7474 7073 3a2f 2f63 6f6e 7472 6962 2e72  ttps://contrib.r
+00005670: 6f63 6b73 2f69 6d61 6765 3f72 6570 6f3d  ocks/image?repo=
+00005680: 7377 616e 6875 6278 2f73 7761 6e6c 6162  swanhubx/swanlab
+00005690: 2220 2f3e 0a3c 2f61 3e0a 0a23 2323 2044  " />.</a>..### D
+000056a0: 6f77 6e6c 6f61 6420 4963 6f6e 0a0a 5b53  ownload Icon..[S
+000056b0: 7761 6e4c 6162 2d49 636f 6e2d 5356 475d  wanLab-Icon-SVG]
+000056c0: 2872 6561 646d 655f 6669 6c65 732f 7377  (readme_files/sw
+000056d0: 616e 6c61 622d 6c6f 676f 2e73 7667 290a  anlab-logo.svg).
+000056e0: 0a3c 6272 3e0a 0a23 2320 f09f 9383 204c  .<br>..## .... L
+000056f0: 6963 656e 7365 0a0a 5468 6973 2072 6570  icense..This rep
+00005700: 6f73 6974 6f72 7920 666f 6c6c 6f77 7320  ository follows 
+00005710: 7468 6520 5b41 7061 6368 6520 322e 3020  the [Apache 2.0 
+00005720: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
+00005730: 2f67 6974 6875 622e 636f 6d2f 5377 616e  /github.com/Swan
+00005740: 4875 6258 2f53 7761 6e4c 6162 2f62 6c6f  HubX/SwanLab/blo
+00005750: 622f 6d61 696e 2f4c 4943 454e 5345 2920  b/main/LICENSE) 
+00005760: 6f70 656e 2073 6f75 7263 650a 6c69 6365  open source.lice
+00005770: 6e73 652e 0a                             nse..
```

