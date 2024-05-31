# Comparing `tmp/jupyterlab_amphi-0.3.9.tar.gz` & `tmp/jupyterlab_amphi-0.4.0.tar.gz`

## Comparing `jupyterlab_amphi-0.3.9.tar` & `jupyterlab_amphi-0.4.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/MANIFEST.in
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/install.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/tsconfig.eslint.json
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/tsconfigbase.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/_version.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0   184186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/257.ea9d07d3d9b1dc539e1c.js
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
--rw-r--r--   0        0        0    22287 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js.LICENSE.txt
--rw-r--r--   0        0        0  1442389 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js
--rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js.LICENSE.txt
--rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/remoteEntry.35574e4219000d084bcf.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/third-party-licenses.json
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
--rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js.LICENSE.txt
--rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
--rw-r--r--   0        0        0    58404 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/4.5e053c8b5a64d881fccb.js
--rw-r--r--   0        0        0  1438115 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js
--rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js.LICENSE.txt
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
--rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
--rw-r--r--   0        0        0   440200 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/841.2769366911b2fa008442.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/841.2769366911b2fa008442.js.LICENSE.txt
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/remoteEntry.9806628c0e292205da2d.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
--rw-r--r--   0        0        0    33644 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/412.b356edbd43fafc52ec7f.js
--rw-r--r--   0        0        0    27283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/550.307c83f4ab4a3437a91a.js
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
--rw-r--r--   0        0        0  1448030 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js
--rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js.LICENSE.txt
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/remoteEntry.de9b136c09bb3aee0e22.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/third-party-licenses.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0   754444 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js
--rw-r--r--   0        0        0    13411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js.LICENSE.txt
--rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/401.6e49833ff26e7b1d5be2.js
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/remoteEntry.c67657151333eb6a00a3.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/third-party-licenses.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
--rw-r--r--   0        0        0    25488 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/732.917e4fffb0314b8bdb52.js
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/remoteEntry.40c20234dc9bff58f2c8.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/third-party-licenses.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi_extension/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/install.json
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/PipelineService.tsx
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/RequestService.tsx
--rw-r--r--   0        0        0    21078 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/connectionUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/generatorUtils.tsx
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/InputRegular.tsx
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/dataMapping.tsx
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectColumn.tsx
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectColumns.tsx
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectMultipleCustomizable.tsx
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectRegular.tsx
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/transferData.tsx
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/install.json
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    22755 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    22115 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/README.md
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/MANIFEST.in
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/_version.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/install.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/_version.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0   184281 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/257.c230a33b174cf7dc974a.js
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
+-rw-r--r--   0        0        0    22287 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js.LICENSE.txt
+-rw-r--r--   0        0        0  1442389 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js
+-rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js.LICENSE.txt
+-rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/remoteEntry.d7231541239c291ad96e.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
+-rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js.LICENSE.txt
+-rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
+-rw-r--r--   0        0        0    58404 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/4.5e053c8b5a64d881fccb.js
+-rw-r--r--   0        0        0  1438115 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js
+-rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js.LICENSE.txt
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
+-rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
+-rw-r--r--   0        0        0   440200 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/841.2769366911b2fa008442.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/841.2769366911b2fa008442.js.LICENSE.txt
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/remoteEntry.4882ea2c8e36c63dff28.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
+-rw-r--r--   0        0        0    33644 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/412.b356edbd43fafc52ec7f.js
+-rw-r--r--   0        0        0    27283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/550.307c83f4ab4a3437a91a.js
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
+-rw-r--r--   0        0        0  1448030 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js
+-rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js.LICENSE.txt
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/remoteEntry.5b383a53d7b3b7a9b538.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0   754444 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js
+-rw-r--r--   0        0        0    13411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js.LICENSE.txt
+-rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/401.6e49833ff26e7b1d5be2.js
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/remoteEntry.18aa5b7f97cf5728dfbb.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
+-rw-r--r--   0        0        0    25488 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/732.917e4fffb0314b8bdb52.js
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/remoteEntry.3b97d5a76cb8e65ccc87.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/third-party-licenses.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/install.json
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/RequestService.tsx
+-rw-r--r--   0        0        0    21078 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/connectionUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/generatorUtils.tsx
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/InputRegular.tsx
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/dataMapping.tsx
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectMultipleCustomizable.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/install.json
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    22755 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    22115 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/README.md
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.4.0/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.3.9/output.json` & `jupyterlab_amphi-0.4.0/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/package.json` & `jupyterlab_amphi-0.4.0/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.9",
+    "version": "0.4.0",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.3.9/tsconfigbase.json` & `jupyterlab_amphi-0.4.0/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d7231541239c291ad96e.js'}}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.35574e4219000d084bcf.js",
+            "load": "static/remoteEntry.d7231541239c291ad96e.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/257.ea9d07d3d9b1dc539e1c.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/257.c230a33b174cf7dc974a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -856,15 +856,15 @@
                     manager: r,
                     commands: d,
                     handleChange: u
                 }))
             };
             class Oe extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Parquet File Input", this._id = "parquetFileInput", this._type = "pandas_df_input", this._category = "input", this._icon = d, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Parquet File Input", this._id = "parquetFileInput", this._type = "pandas_df_input", this._fileDrop = ["parquet"], this._category = "input", this._icon = d, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
                             placeholder: "Type file name",
                             validation: "\\.(parquet)$",
@@ -6743,14 +6743,20 @@
                         Icon: fn.Icon,
                         showContent: f,
                         handle: I,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
+                provideDependencies({
+                    config: e
+                }) {
+                    let n = [];
+                    return n.push("pyarrow"), n
+                }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js.LICENSE.txt` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/687.637d40e182f18bc1c388.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/remoteEntry.35574e4219000d084bcf.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/remoteEntry.d7231541239c291ad96e.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, f, u, s, c, p, d, h, v, b, m, g, y, w = {
-            2212: (e, r, t) => {
+    var e, r, t, n, o, a, i, l, u, f, s, c, d, p, h, b, v, m, g, y, w = {
+            2695: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(518), t.e(345), t.e(257)]).then((() => () => t(8257))),
                         "./extension": () => Promise.all([t.e(518), t.e(345), t.e(257)]).then((() => () => t(8257))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -43,23 +43,23 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        257: "ea9d07d3d9b1dc539e1c",
+        257: "c230a33b174cf7dc974a",
         345: "d33854e26caa385d0f56",
         432: "0fc640989ce2150a2305",
         518: "22c1338a13eb80857e8c",
         628: "6bee9242bd295a15f79b",
         687: "637d40e182f18bc1c388",
         713: "986c30f40fc55619b937"
     } [e] + ".js?v=" + {
-        257: "ea9d07d3d9b1dc539e1c",
+        257: "c230a33b174cf7dc974a",
         345: "d33854e26caa385d0f56",
         432: "0fc640989ce2150a2305",
         518: "22c1338a13eb80857e8c",
         628: "6bee9242bd295a15f79b",
         687: "637d40e182f18bc1c388",
         713: "986c30f40fc55619b937"
     } [e], S.g = function() {
@@ -70,28 +70,28 @@
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-components-core:", S.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
-                    var s = f[u];
+                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
+                    var s = u[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var c = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(c.bind(null, void 0, {
+                d = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -116,16 +116,16 @@
                             l = o[r];
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    f = [];
-                return "default" === t && (l("@amphi/pipeline-components-core", "0.3.9", (() => Promise.all([S.e(518), S.e(345), S.e(257)]).then((() => () => S(8257))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                    u = [];
+                return "default" === t && (l("@amphi/pipeline-components-core", "0.4.0", (() => Promise.all([S.e(518), S.e(345), S.e(257)]).then((() => () => S(8257))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -161,106 +161,106 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var l = e[a];
-            i.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
-        return f();
+        return u();
 
-        function f() {
+        function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, l = 1, f = !0;; l++, i++) {
-                var u, s, c = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(u = r[i]))[0])) return !f || ("u" == c ? l > n && !o : "" == c != o);
+            for (var i = 0, l = 1, u = !0;; l++, i++) {
+                var f, s, c = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == c ? l > n && !o : "" == c != o);
                 if ("u" == s) {
-                    if (!f || "u" != c) return !1
-                } else if (f)
+                    if (!u || "u" != c) return !1
+                } else if (u)
                     if (c == s)
                         if (l <= n) {
-                            if (u != e[l]) return !1
+                            if (f != e[l]) return !1
                         } else {
-                            if (o ? u > e[l] : u < e[l]) return !1;
-                            u != e[l] && (f = !1)
+                            if (o ? f > e[l] : f < e[l]) return !1;
+                            f != e[l] && (u = !1)
                         }
                 else if ("s" != c && "n" != c) {
                     if (o || l <= n) return !1;
-                    f = !1, l--
+                    u = !1, l--
                 } else {
                     if (l <= n || s < c != o) return !1;
-                    f = !1
-                } else "s" != c && "n" != c && (f = !1, l--)
+                    u = !1
+                } else "s" != c && "n" != c && (u = !1, l--)
             }
         }
-        var p = [],
-            d = p.pop.bind(p);
+        var d = [],
+            p = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
+            d.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!d()
+        return !!p()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", u = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || c(f(e, t, o, n)), p(e[t][o])
+        return a(n, o) || c(u(e, t, o, n)), d(e[t][o])
     }, s = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, o) {
+    }, d = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
         var a = S.I(r);
         return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), u(r, 0, t, n)))), v = d(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), b = p(((e, r, t, n, o) => {
         var a = r && S.o(r, t) && s(r, t, n);
-        return a ? p(a) : o()
-    })), b = {}, m = {
+        return a ? d(a) : o()
+    })), v = {}, m = {
         3345: () => h("default", "react", [1, 18, 2, 0]),
         1760: () => h("default", "@jupyterlab/ui-components", [1, 4, 2, 1]),
-        2473: () => v("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([S.e(713), S.e(628)]).then((() => () => S(5713))))),
+        2473: () => b("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([S.e(713), S.e(628)]).then((() => () => S(5713))))),
         3254: () => h("default", "@amphi/pipeline-components-manager", [0]),
-        4810: () => v("default", "antd", [4, 5, 16, 4], (() => Promise.all([S.e(687), S.e(628)]).then((() => () => S(7687))))),
+        4810: () => b("default", "antd", [4, 5, 16, 4], (() => Promise.all([S.e(687), S.e(628)]).then((() => () => S(7687))))),
         7628: () => h("default", "react-dom", [1, 18, 2, 0])
     }, g = {
         257: [1760, 2473, 3254, 4810],
         345: [3345],
         628: [7628]
     }, y = {}, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
-            if (S.o(b, e)) return r.push(b[e]);
+            if (S.o(v, e)) return r.push(v[e]);
             if (!y[e]) {
                 var t = r => {
-                    b[e] = 0, S.m[e] = t => {
+                    v[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var n = r => {
-                    delete b[e], S.m[e] = t => {
+                    delete v[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
                 try {
                     var o = m[e]();
-                    o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                    o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
@@ -283,20 +283,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var n, o, [a, i, l] = t,
-                    f = 0;
+                    u = 0;
                 if (a.some((r => 0 !== e[r]))) {
                     for (n in i) S.o(i, n) && (S.m[n] = i[n]);
                     l && l(S)
                 }
-                for (r && r(t); f < a.length; f++) o = a[f], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < a.length; u++) o = a[u], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_amphi_pipeline_components_core = self.webpackChunk_amphi_pipeline_components_core || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(2212);
+    var E = S(2695);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-components-core"] = E
 })();
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-core/static/third-party-licenses.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-core/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4882ea2c8e36c63dff28.js'}}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -49,15 +49,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9806628c0e292205da2d.js",
+            "load": "static/remoteEntry.4882ea2c8e36c63dff28.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/4.5e053c8b5a64d881fccb.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/4.5e053c8b5a64d881fccb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js.LICENSE.txt` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/422.71d1839daa29ac549ae9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/841.2769366911b2fa008442.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/841.2769366911b2fa008442.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/remoteEntry.9806628c0e292205da2d.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/remoteEntry.4882ea2c8e36c63dff28.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, i, f, d, l, u, c, s, p, h, b, m, v, g, y, w = {
-            5548: (e, r, t) => {
+            8695: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(173), t.e(725), t.e(345), t.e(628), t.e(4)]).then((() => () => t(1004))),
                         "./extension": () => Promise.all([t.e(173), t.e(725), t.e(345), t.e(628), t.e(4)]).then((() => () => t(1004))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -132,15 +132,15 @@
                         (!f || !f.loaded && (!a != !f.eager ? a : i > f.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (f("@amphi/pipeline-components-manager", "0.3.9", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(4)]).then((() => () => S(1004))))), f("ace-builds", "1.34.2", (() => S.e(841).then((() => () => S(1841))))), f("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), f("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), f("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), f("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("@amphi/pipeline-components-manager", "0.4.0", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(4)]).then((() => () => S(1004))))), f("ace-builds", "1.34.2", (() => S.e(841).then((() => () => S(1841))))), f("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), f("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), f("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), f("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -316,10 +316,10 @@
                     f && f(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(5548);
+    var E = S(8695);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-components-manager"] = E
 })();
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-components-manager/static/third-party-licenses.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-components-manager/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5b383a53d7b3b7a9b538.js'}}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -47,15 +47,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.de9b136c09bb3aee0e22.js",
+            "load": "static/remoteEntry.5b383a53d7b3b7a9b538.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/412.b356edbd43fafc52ec7f.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/412.b356edbd43fafc52ec7f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/550.307c83f4ab4a3437a91a.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/550.307c83f4ab4a3437a91a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js.LICENSE.txt` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/735.5a196ae4c7d7bbfdf576.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/remoteEntry.de9b136c09bb3aee0e22.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/remoteEntry.5b383a53d7b3b7a9b538.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, i, l, u, f, d, s, p, c, h, b, v, m, g, y, w, j, P, S, E = {
-            8535: (e, r, t) => {
+            5346: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(345), t.e(550), t.e(412)]).then((() => () => t(8412))),
                         "./extension": () => Promise.all([t.e(345), t.e(550), t.e(412)]).then((() => () => t(8412))),
                         "./style": () => Promise.all([t.e(550), t.e(631)]).then((() => () => t(7631)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-editor", "0.3.9", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-editor", "0.4.0", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         _.g.importScripts && (e = _.g.location + "");
         var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -311,10 +311,10 @@
                     l && l(_)
                 }
                 for (r && r(t); u < o.length; u++) n = o[u], _.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amphi_pipeline_editor = self.webpackChunk_amphi_pipeline_editor || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), _.nc = void 0;
-    var x = _(8535);
+    var x = _(5346);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-editor"] = x
 })();
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-editor/static/third-party-licenses.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-editor/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.18aa5b7f97cf5728dfbb.js'}}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -52,15 +52,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c67657151333eb6a00a3.js",
+            "load": "static/remoteEntry.18aa5b7f97cf5728dfbb.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js.LICENSE.txt` & `jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/240.d16054e20c74c77cdbd8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/401.6e49833ff26e7b1d5be2.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/401.6e49833ff26e7b1d5be2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/remoteEntry.c67657151333eb6a00a3.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/remoteEntry.18aa5b7f97cf5728dfbb.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, i, a, l, u, f, s, p, d, c, h, v, m, g = {
-            8383: (e, r, t) => {
+            4938: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(240), t.e(401)]).then((() => () => t(7401))),
                         "./extension": () => Promise.all([t.e(240), t.e(401)]).then((() => () => t(7401))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -108,15 +108,15 @@
                     var o = i[e] = i[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
                         get: () => Promise.all([y.e(240), y.e(401)]).then((() => () => y(7401))),
                         from: a,
                         eager: !1
                     })
-                })("@amphi/pipeline-log-console", "0.3.9"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-log-console", "0.4.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -279,10 +279,10 @@
                     l && l(y)
                 }
                 for (r && r(t); u < i.length; u++) o = i[u], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), y.nc = void 0;
-    var w = y(8383);
+    var w = y(4938);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-log-console"] = w
 })();
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-log-console/static/third-party-licenses.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-log-console/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3b97d5a76cb8e65ccc87.js'}}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -51,15 +51,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.40c20234dc9bff58f2c8.js",
+            "load": "static/remoteEntry.3b97d5a76cb8e65ccc87.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -95,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/732.917e4fffb0314b8bdb52.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/732.917e4fffb0314b8bdb52.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/remoteEntry.40c20234dc9bff58f2c8.js` & `jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/remoteEntry.3b97d5a76cb8e65ccc87.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, a, i, o, l, u, p, d, f, s, c, h, v, m, g = {
-            320: (e, r, t) => {
+            475: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(732).then((() => () => t(732))),
                         "./extension": () => t.e(732).then((() => () => t(732))),
                         "./style": () => t.e(432).then((() => () => t(432)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -106,15 +106,15 @@
                     var a = i[e] = i[e] || {},
                         l = a[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : o > l.from)) && (a[r] = {
                         get: () => y.e(732).then((() => () => y(732))),
                         from: o,
                         eager: !1
                     })
-                })("@amphi/pipeline-metadata-panel", "0.3.9"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-metadata-panel", "0.4.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -276,10 +276,10 @@
                     l && l(y)
                 }
                 for (r && r(t); u < i.length; u++) a = i[u], y.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_amphi_pipeline_metadata_panel = self.webpackChunk_amphi_pipeline_metadata_panel || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), y.nc = void 0;
-    var w = y(320);
+    var w = y(475);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-metadata-panel"] = w
 })();
```

### Comparing `jupyterlab_amphi-0.3.9/amphi/pipeline-metadata-panel/static/third-party-licenses.json` & `jupyterlab_amphi-0.4.0/amphi/pipeline-metadata-panel/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -94,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/CodeGenerator.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/CodeGenerator.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/DndProviderWrapper.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/DndProviderWrapper.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/PipelineService.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/PipelineService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/RequestService.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/RequestService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/configUtils.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/configUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/connectionUtils.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/connectionUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/generatorUtils.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/generatorUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/rendererUtils.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/rendererUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/InputRegular.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/InputRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/connectionSelector.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/connectionSelector.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/dataMapping.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/dataMapping.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectColumn.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectColumn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectColumns.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectMultiple.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectMultiple.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectMultipleCustomizable.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectMultipleCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectRegular.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/selectTokenization.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/selectTokenization.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/transferData.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/transferData.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -98,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/canvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/output.css` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/output.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.4.0/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/LICENSE` & `jupyterlab_amphi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/README.md` & `jupyterlab_amphi-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/pyproject.toml` & `jupyterlab_amphi-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.9/PKG-INFO` & `jupyterlab_amphi-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.3.9
+Version: 0.4.0
 Dynamic: Keywords
 Summary: Amphi is a no-code ETL extension for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```

