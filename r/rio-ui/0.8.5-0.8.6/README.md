# Comparing `tmp/rio_ui-0.8.5.tar.gz` & `tmp/rio_ui-0.8.6.tar.gz`

## Comparing `rio_ui-0.8.5.tar` & `rio_ui-0.8.6.tar`

### file list

```diff
@@ -1,385 +1,385 @@
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.prettierrc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.sassrc
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.8.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 rio_ui-0.8.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.8.5/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 rio_ui-0.8.5/changelog.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 rio_ui-0.8.5/package.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 rio_ui-0.8.5/vite.config.js
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.github/DISCUSSION_TEMPLATE/feature-requests.yml
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/index.html
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/app.ts
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/colorConversion.ts
--rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/componentManagement.ts
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/cssUtils.ts
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/dataModels.ts
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/designApplication.ts
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/easeFunctions.ts
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/eventHandling.ts
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/eventRateLimiter.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/inputBoxTools.ts
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/layoutHelpers.ts
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/layouting.ts
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/rippleEffect.ts
--rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/rpc.ts
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/rpcFunctions.ts
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/utils.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/align.ts
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/buildFailed.ts
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/button.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/card.ts
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/classContainer.ts
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/codeBlock.ts
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/codeExplorer.ts
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/colorPicker.ts
--rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/componentBase.ts
--rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/componentTree.ts
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/customListItem.ts
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/devToolsConnector.ts
--rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/drawer.ts
--rw-r--r--   0        0        0    17182 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/dropdown.ts
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/flowContainer.ts
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/fundamentalRootComponent.ts
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/grid.ts
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/headingListItem.ts
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/html.ts
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/icon.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/image.ts
--rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/keyEventListener.ts
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/linearContainers.ts
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/link.ts
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/listView.ts
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/margin.ts
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/markdown.ts
--rw-r--r--   0        0        0    28001 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/mediaPlayer.ts
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/mouseEventListener.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/multiLineTextInput.ts
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/nodeInput.ts
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/nodeOutput.ts
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/overlay.ts
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/placeholder.ts
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/plot.ts
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/popup.ts
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/progressBar.ts
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/progressCircle.ts
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/rectangle.ts
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/revealer.ts
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/scrollContainer.ts
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/scrollTarget.ts
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/separator.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/separatorListItem.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/singleContainer.ts
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/slider.ts
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/slideshow.ts
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/stack.ts
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/switch.ts
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/switcher.ts
--rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/switcherBar.ts
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/table.ts
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/text.ts
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/textInput.ts
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/themeContextSwitcher.ts
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/tooltip.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/code/components/website.ts
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/css/highlightjs-default-dark.css
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/css/highlightjs-default-light.css
--rw-r--r--   0        0        0    51483 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/css/style.scss
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.8.5/frontend/css/switcheroos.scss
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/custom-material-icons/twinkle.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/custom-material-icons/fill/twinkle.svg
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/logo.svg
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/color/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/color/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/color/logo.svg
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/fill/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/fill/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/rio/fill/logo.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/styling/corner-round-bottom-left.svg
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/styling/corner-round-bottom-right.svg
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/styling/corner-round-top-left.svg
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.8.5/raw-icons/styling/corner-round-top-right.svg
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/__main__.py
--rw-r--r--   0        0        0    19924 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/app.py
--rw-r--r--   0        0        0    33083 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/app_server.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/byte_serving.py
--rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/color.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cursor_style.py
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/dataclass.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/deprecations.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/errors.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/event.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/fills.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/global_state.py
--rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/icon_registry.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/inspection.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/maybes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/py.typed
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/routing.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/self_serializing.py
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/serialization.py
--rw-r--r--   0        0        0    89077 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/session.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/session_attachments.py
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/state_properties.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/testing.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/text_style.py
--rw-r--r--   0        0        0    30066 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/theme.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/user_settings_module.py
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/utils.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/world_units.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/hosted/README.md
--rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/__init__.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/project.py
--rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/rioignore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    26835 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/__init__.py
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/app_root.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/auto_form.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/banner.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/build_failed.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/button.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/card.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/class_container.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/code_block.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/code_explorer.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/color_picker.py
--rw-r--r--   0        0        0    30644 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/component.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/component_tree.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/container.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/dev_tools_connector.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/devel_component.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/drawer.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/dropdown.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/flow_container.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/grid.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/html.py
--rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/icon.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/image.py
--rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/labeled_column.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/linear_containers.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/link.py
--rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/list_items.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/list_view.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/markdown.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/media_player.py
--rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/node_input.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/node_output.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/number_input.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/overlay.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/page_view.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/plot.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/popup.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/progress_circle.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/rectangle.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/revealer.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/root_components.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/scroll_container.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/separator.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/slider.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/slideshow.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/spacer.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/stack.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/switch.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/switcher.py
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/table.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/text.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/text_input.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/tooltip.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/components/website.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/__init__.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/validator.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/__init__.py
--rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/component_details.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/deploy_page.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/dev_tools_sidebar.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/docs_page.py
--rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/icons_page.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/layout_preview.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/project_page.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/sample_icons_grid.py
--rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/debug/dev_tools/tree_page.py
--rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/docs/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/frontend files/index.html
--rw-r--r--   0        0        0    57775 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/frontend files/assets/index-4c436499.css
--rw-r--r--   0        0        0   361126 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/frontend files/assets/index-a8d525bb.js
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/README.md
--rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/core-classes.md
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/debugging-setup.md
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/deployment.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-custom-events.md
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-install.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/persistent-settings.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/project-setup.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/run-project.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos/theming.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos-todo/custom-events.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos-todo/force-refresh.md
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos-todo/layouting.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/README.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
--rw-r--r--   0        0        0   209356 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/README.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/data_models.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/meta.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/root_init.py
--rw-r--r--   0        0        0   136134 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/components/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/pages/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.8.5/scripts/benchmark.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 rio_ui-0.8.5/scripts/build_frontend.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.8.5/scripts/build_material_icon_set.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.8.5/scripts/cloc.sh
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.8.5/scripts/code_coverage.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 rio_ui-0.8.5/scripts/publish_new_release.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_app_build.py
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_attribute_bindings.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_custom_components.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_docstring_code_blocks.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_documentation.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_events.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_project_templates.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_reconciliation.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_refresh.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_session.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_testing_tools.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_user_settings.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/test_zzz_guardrails.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 rio_ui-0.8.5/tests/utils.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rio_ui-0.8.5/.gitignore
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.8.5/LICENSE.txt
--rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 rio_ui-0.8.5/README.md
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.8.5/pyproject.toml
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 rio_ui-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.prettierrc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.sassrc
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.8.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 rio_ui-0.8.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 rio_ui-0.8.6/SECURITY.md
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 rio_ui-0.8.6/changelog.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 rio_ui-0.8.6/package.json
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 rio_ui-0.8.6/vite.config.js
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/DISCUSSION_TEMPLATE/feature-requests.yml
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/index.html
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    20719 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/eventRateLimiter.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/layouting.ts
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/rippleEffect.ts
+-rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/button.ts
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/codeBlock.ts
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/devToolsConnector.ts
+-rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    17182 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    28001 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/website.ts
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    51597 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/style.scss
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/switcheroos.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/__main__.py
+-rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/app.py
+-rw-r--r--   0        0        0    33083 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/app_server.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/byte_serving.py
+-rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/color.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cursor_style.py
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/dataclass.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/deprecations.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/errors.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/event.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/global_state.py
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/icon_registry.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/inspection.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/py.typed
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/self_serializing.py
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/serialization.py
+-rw-r--r--   0        0        0    89510 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/session.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/session_attachments.py
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/state_properties.py
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/testing.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/text_style.py
+-rw-r--r--   0        0        0    30066 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/theme.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/user_settings_module.py
+-rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/utils.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/world_units.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/project.py
+-rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    26835 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/__init__.py
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/app_root.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/auto_form.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/banner.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/build_failed.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/button.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/card.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/class_container.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/code_block.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/color_picker.py
+-rw-r--r--   0        0        0    30717 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/component.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/container.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/dev_tools_connector.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/devel_component.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/drawer.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/dropdown.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/flow_container.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/grid.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/html.py
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/icon.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/image.py
+-rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/labeled_column.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/link.py
+-rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/list_items.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/list_view.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/markdown.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/media_player.py
+-rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/node_input.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/node_output.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/number_input.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/overlay.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/page_view.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/plot.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/popup.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/rectangle.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/revealer.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/root_components.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/separator.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/slider.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/spacer.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/stack.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/switch.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/switcher.py
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/table.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/text.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/text_input.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/tooltip.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/validator.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/__init__.py
+-rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/component_details.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/deploy_page.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/dev_tools_sidebar.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/docs_page.py
+-rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/icons_page.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/project_page.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/sample_icons_grid.py
+-rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/tree_page.py
+-rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/docs/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/frontend files/index.html
+-rw-r--r--   0        0        0   361140 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/frontend files/assets/index-8ca8e5f1.js
+-rw-r--r--   0        0        0    57852 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/frontend files/assets/index-9eba151c.css
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/README.md
+-rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/core-classes.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/debugging-setup.md
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/deployment.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-custom-events.md
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-install.md
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/persistent-settings.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/project-setup.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/run-project.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/theming.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/custom-events.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/force-refresh.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/layouting.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/README.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
+-rw-r--r--   0        0        0   209356 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/README.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/data_models.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/meta.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/root_init.py
+-rw-r--r--   0        0        0   136134 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/pages/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/benchmark.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/build_frontend.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/code_coverage.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_app_build.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_attribute_bindings.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_custom_components.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_documentation.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_project_templates.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_refresh.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_session.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_testing_tools.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_user_settings.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/utils.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.gitignore
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.8.6/LICENSE.txt
+-rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 rio_ui-0.8.6/README.md
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 rio_ui-0.8.6/PKG-INFO
```

### Comparing `rio_ui-0.8.5/CODE_OF_CONDUCT.md` & `rio_ui-0.8.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/CONTRIBUTING.md` & `rio_ui-0.8.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/changelog.md` & `rio_ui-0.8.6/changelog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Changelog
 
 -   Buttons now have a smaller minimum size when using a `rio.Component` as
     content
--   `FrostedGlassFill` added
--   `rio.Fill` deprecated. Most components only support specific fills, so this
-    base class has no purpose any more
+-   `FrostedGlassFill` added (Contributed by MiniTT)
+-   `rio.Fill` and `rio.FillLike` deprecated. Most components only support
+    specific fills, so these have no purpose any more
 -   added `@rio.event.on_window_size_change`
 -   popups now default to the "hud" color
+-   Add HTML meta tags
+-   Add functions for reading and writing clipboard contents to the `Session`
+    (Contributed by MiniTT)
 
 ## 0.8
 
 -   Rectangles now honor the theme's shadow color
 -   Renamed `Banner.markup` to `Banner.markdown`
 -   Removed the "multiline" style from Banners
 -   Removed `Button.initially_disabled_for`
```

### Comparing `rio_ui-0.8.5/.github/PULL_REQUEST_TEMPLATE.md` & `rio_ui-0.8.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/.github/DISCUSSION_TEMPLATE/feature-requests.yml` & `rio_ui-0.8.6/.github/DISCUSSION_TEMPLATE/feature-requests.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `rio_ui-0.8.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/.github/ISSUE_TEMPLATE/config.yml` & `rio_ui-0.8.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/index.html` & `rio_ui-0.8.6/frontend/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/app.ts` & `rio_ui-0.8.6/frontend/code/app.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/colorConversion.ts` & `rio_ui-0.8.6/frontend/code/colorConversion.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/componentManagement.ts` & `rio_ui-0.8.6/frontend/code/componentManagement.ts`

 * *Files 2% similar despite different names*

```diff
@@ -224,16 +224,15 @@
     let entireState = getCurrentComponentState(componentId, deltaState);
     let resultId = componentId;
 
     // Margin
     let margin = entireState['_margin_']!;
     if (margin === undefined) {
         console.error(`Got incomplete state for component ${componentId}`);
-    }
-    if (
+    } else if (
         margin[0] !== 0 ||
         margin[1] !== 0 ||
         margin[2] !== 0 ||
         margin[3] !== 0
     ) {
         let marginId = (componentId * -10) as ComponentId;
         message[marginId] = {
@@ -254,16 +253,15 @@
         resultId = marginId;
     }
 
     // Align
     let align = entireState['_align_']!;
     if (align === undefined) {
         console.error(`Got incomplete state for component ${componentId}`);
-    }
-    if (align[0] !== null || align[1] !== null) {
+    } else if (align[0] !== null || align[1] !== null) {
         let alignId = (componentId * -10 - 1) as ComponentId;
         message[alignId] = {
             _type_: 'Align-builtin',
             _python_type_: 'Align (injected)',
             _key_: null,
             _margin_: [0, 0, 0, 0],
             _size_: [0, 0],
```

### Comparing `rio_ui-0.8.5/frontend/code/cssUtils.ts` & `rio_ui-0.8.6/frontend/code/cssUtils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/dataModels.ts` & `rio_ui-0.8.6/frontend/code/dataModels.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/designApplication.ts` & `rio_ui-0.8.6/frontend/code/designApplication.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/easeFunctions.ts` & `rio_ui-0.8.6/frontend/code/easeFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/eventHandling.ts` & `rio_ui-0.8.6/frontend/code/eventHandling.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/eventRateLimiter.ts` & `rio_ui-0.8.6/frontend/code/eventRateLimiter.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/inputBoxTools.ts` & `rio_ui-0.8.6/frontend/code/inputBoxTools.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/layoutHelpers.ts` & `rio_ui-0.8.6/frontend/code/layoutHelpers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/layouting.ts` & `rio_ui-0.8.6/frontend/code/layouting.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/rippleEffect.ts` & `rio_ui-0.8.6/frontend/code/rippleEffect.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/rpc.ts` & `rio_ui-0.8.6/frontend/code/rpc.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/rpcFunctions.ts` & `rio_ui-0.8.6/frontend/code/rpcFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/utils.ts` & `rio_ui-0.8.6/frontend/code/utils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/align.ts` & `rio_ui-0.8.6/frontend/code/components/align.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/buildFailed.ts` & `rio_ui-0.8.6/frontend/code/components/buildFailed.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/button.ts` & `rio_ui-0.8.6/frontend/code/components/button.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/card.ts` & `rio_ui-0.8.6/frontend/code/components/card.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/classContainer.ts` & `rio_ui-0.8.6/frontend/code/components/classContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/codeBlock.ts` & `rio_ui-0.8.6/frontend/code/components/codeBlock.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/codeExplorer.ts` & `rio_ui-0.8.6/frontend/code/components/codeExplorer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/colorPicker.ts` & `rio_ui-0.8.6/frontend/code/components/colorPicker.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/componentBase.ts` & `rio_ui-0.8.6/frontend/code/components/componentBase.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/componentTree.ts` & `rio_ui-0.8.6/frontend/code/components/componentTree.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/customListItem.ts` & `rio_ui-0.8.6/frontend/code/components/customListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/devToolsConnector.ts` & `rio_ui-0.8.6/frontend/code/components/devToolsConnector.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/drawer.ts` & `rio_ui-0.8.6/frontend/code/components/drawer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/dropdown.ts` & `rio_ui-0.8.6/frontend/code/components/dropdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/flowContainer.ts` & `rio_ui-0.8.6/frontend/code/components/flowContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/fundamentalRootComponent.ts` & `rio_ui-0.8.6/frontend/code/components/fundamentalRootComponent.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/grid.ts` & `rio_ui-0.8.6/frontend/code/components/grid.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/headingListItem.ts` & `rio_ui-0.8.6/frontend/code/components/headingListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/html.ts` & `rio_ui-0.8.6/frontend/code/components/html.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/icon.ts` & `rio_ui-0.8.6/frontend/code/components/icon.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/image.ts` & `rio_ui-0.8.6/frontend/code/components/image.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/keyEventListener.ts` & `rio_ui-0.8.6/frontend/code/components/keyEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/linearContainers.ts` & `rio_ui-0.8.6/frontend/code/components/linearContainers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/link.ts` & `rio_ui-0.8.6/frontend/code/components/link.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/listView.ts` & `rio_ui-0.8.6/frontend/code/components/listView.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/margin.ts` & `rio_ui-0.8.6/frontend/code/components/margin.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/markdown.ts` & `rio_ui-0.8.6/frontend/code/components/markdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/mediaPlayer.ts` & `rio_ui-0.8.6/frontend/code/components/mediaPlayer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/mouseEventListener.ts` & `rio_ui-0.8.6/frontend/code/components/mouseEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/multiLineTextInput.ts` & `rio_ui-0.8.6/frontend/code/components/multiLineTextInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/nodeInput.ts` & `rio_ui-0.8.6/frontend/code/components/nodeInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/nodeOutput.ts` & `rio_ui-0.8.6/frontend/code/components/nodeOutput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/overlay.ts` & `rio_ui-0.8.6/frontend/code/components/overlay.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/placeholder.ts` & `rio_ui-0.8.6/frontend/code/components/placeholder.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/plot.ts` & `rio_ui-0.8.6/frontend/code/components/plot.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/popup.ts` & `rio_ui-0.8.6/frontend/code/components/popup.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/progressBar.ts` & `rio_ui-0.8.6/frontend/code/components/progressBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/progressCircle.ts` & `rio_ui-0.8.6/frontend/code/components/progressCircle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/rectangle.ts` & `rio_ui-0.8.6/frontend/code/components/rectangle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/revealer.ts` & `rio_ui-0.8.6/frontend/code/components/revealer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/scrollContainer.ts` & `rio_ui-0.8.6/frontend/code/components/scrollContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/scrollTarget.ts` & `rio_ui-0.8.6/frontend/code/components/scrollTarget.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/separator.ts` & `rio_ui-0.8.6/frontend/code/components/separator.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/separatorListItem.ts` & `rio_ui-0.8.6/frontend/code/components/separatorListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/singleContainer.ts` & `rio_ui-0.8.6/frontend/code/components/singleContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/slider.ts` & `rio_ui-0.8.6/frontend/code/components/slider.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/slideshow.ts` & `rio_ui-0.8.6/frontend/code/components/slideshow.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/stack.ts` & `rio_ui-0.8.6/frontend/code/components/stack.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/switch.ts` & `rio_ui-0.8.6/frontend/code/components/switch.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/switcher.ts` & `rio_ui-0.8.6/frontend/code/components/switcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/switcherBar.ts` & `rio_ui-0.8.6/frontend/code/components/switcherBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/table.ts` & `rio_ui-0.8.6/frontend/code/components/table.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/text.ts` & `rio_ui-0.8.6/frontend/code/components/text.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/textInput.ts` & `rio_ui-0.8.6/frontend/code/components/textInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/themeContextSwitcher.ts` & `rio_ui-0.8.6/frontend/code/components/themeContextSwitcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/tooltip.ts` & `rio_ui-0.8.6/frontend/code/components/tooltip.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/code/components/website.ts` & `rio_ui-0.8.6/frontend/code/components/website.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/css/highlightjs-default-dark.css` & `rio_ui-0.8.6/frontend/css/highlightjs-default-dark.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/css/highlightjs-default-light.css` & `rio_ui-0.8.6/frontend/css/highlightjs-default-light.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/frontend/css/style.scss` & `rio_ui-0.8.6/frontend/css/style.scss`

 * *Files 1% similar despite different names*

```diff
@@ -835,14 +835,19 @@
     overflow: hidden;
 }
 
 // Icon
 .rio-icon {
     pointer-events: auto;
     @include center-content;
+
+    svg {
+        width: 100%;
+        height: 100%;
+    }
 }
 
 // Slider
 .rio-slider {
     pointer-events: auto;
 
     --rio-slider-position-transition-time: 0.3s;
@@ -2034,14 +2039,16 @@
     text-align: left;
 
     font-size: 1.8rem;
     color: var(--rio-global-danger-bg);
 }
 
 .rio-traceback-traceback {
+    pointer-events: auto;
+
     font-family: $monospace-fonts;
     font-size: 0.9rem;
     white-space: pre-wrap;
     overflow-wrap: break-word;
     padding: 0.5rem 1rem;
     background-color: var(--rio-local-bg-variant);
     border-radius: var(--rio-global-corner-radius-small);
@@ -2318,14 +2325,16 @@
 .rio-dev-tools-background {
     position: relative;
 
     background: var(--rio-local-bg);
 }
 
 .rio-dev-tools-background::after {
+    pointer-events: none;
+
     content: '';
     position: absolute;
     display: block;
     z-index: 1;
 
     left: 0;
     top: 0;
```

### Comparing `rio_ui-0.8.5/frontend/css/switcheroos.scss` & `rio_ui-0.8.6/frontend/css/switcheroos.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/custom-material-icons/twinkle.svg` & `rio_ui-0.8.6/raw-icons/custom-material-icons/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/custom-material-icons/fill/twinkle.svg` & `rio_ui-0.8.6/raw-icons/custom-material-icons/fill/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/logo-and-text-horizontal.svg` & `rio_ui-0.8.6/raw-icons/rio/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/logo-and-text-vertical.svg` & `rio_ui-0.8.6/raw-icons/rio/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/logo.svg` & `rio_ui-0.8.6/raw-icons/rio/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/color/logo-and-text-horizontal.svg` & `rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/color/logo-and-text-vertical.svg` & `rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/color/logo.svg` & `rio_ui-0.8.6/raw-icons/rio/color/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/fill/logo-and-text-horizontal.svg` & `rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/fill/logo-and-text-vertical.svg` & `rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/rio/fill/logo.svg` & `rio_ui-0.8.6/raw-icons/rio/fill/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/styling/corner-round-bottom-left.svg` & `rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/styling/corner-round-bottom-right.svg` & `rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/styling/corner-round-top-left.svg` & `rio_ui-0.8.6/raw-icons/styling/corner-round-top-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/raw-icons/styling/corner-round-top-right.svg` & `rio_ui-0.8.6/raw-icons/styling/corner-round-top-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/__init__.py` & `rio_ui-0.8.6/rio/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-__version__ = "0.8.5"
-
-import logging
-
-_logger = logging.getLogger(__name__)
-
-# Re-export dataclass stuff for easy use.
-from dataclasses import KW_ONLY as KW_ONLY
-from dataclasses import field as field
-
-# URLs are used as an important datatype within rio. Re-export them for easy
-# use.
-from yarl import URL as URL
-
-from . import event as event
-from . import patches_for_3rd_party_stuff
-from .app import *
-from .color import *
-from .components import *
-from .cursor_style import *
-from .errors import *
-from .fills import *
-from .routing import *
-from .session import *
-from .text_style import *
-from .theme import *
-from .user_settings_module import *
-from .utils import *
-
-del patches_for_3rd_party_stuff
+__version__ = "0.8.6"
+
+import logging
+
+_logger = logging.getLogger(__name__)
+
+# Re-export dataclass stuff for easy use.
+from dataclasses import KW_ONLY as KW_ONLY
+from dataclasses import field as field
+
+# URLs are used as an important datatype within rio. Re-export them for easy
+# use.
+from yarl import URL as URL
+
+from . import event as event
+from . import patches_for_3rd_party_stuff
+from .app import *
+from .color import *
+from .components import *
+from .cursor_style import *
+from .errors import *
+from .fills import *
+from .routing import *
+from .session import *
+from .text_style import *
+from .theme import *
+from .user_settings_module import *
+from .utils import *
+
+del patches_for_3rd_party_stuff
```

### Comparing `rio_ui-0.8.5/rio/app.py` & `rio_ui-0.8.6/rio/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                         "material/signal-disconnected",
                         fill="danger",
                         width=1.6,
                         height=1.6,
                     ),
                     rio.Text(
                         "Disconnected",
+                        selectable=False,
                         style=rio.TextStyle(
                             fill=self.session.theme.hud_palette.foreground,
                             font_weight="bold",
                         ),
                     ),
                     spacing=0.5,
                     margin_x=2.5,
```

### Comparing `rio_ui-0.8.5/rio/app_server.py` & `rio_ui-0.8.6/rio/app_server.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets.py` & `rio_ui-0.8.6/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/byte_serving.py` & `rio_ui-0.8.6/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/color.py` & `rio_ui-0.8.6/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/dataclass.py` & `rio_ui-0.8.6/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/deprecations.py` & `rio_ui-0.8.6/rio/deprecations.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/errors.py` & `rio_ui-0.8.6/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/event.py` & `rio_ui-0.8.6/rio/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -69,14 +69,49 @@
     events. The method will be called whenever the component is added to the
     component tree.
 
     This may be triggered multiple times if the component is removed and then
     re-added.
 
 
+    ## Example
+
+    Here's an example of a component being conditionally included in the
+    component tree. The `Switch` controls whether the `EventComponent` exists or
+    not, so turning on the switch will mount the `EventComponent` and print
+    "Mounted" to the console.
+
+    ```python
+    class OnMountPrinter(rio.Component):
+        @rio.event.on_mount
+        def on_mount(self):
+            print("Mounted")
+
+        def build(self):
+            return rio.Text("hello")
+
+
+    class Toggler(rio.Component):
+        child: rio.Component
+        show_child: bool = False
+
+        def build(self) -> rio.Component:
+            return rio.Column(
+                # Depending on the Switch state, show either the
+                # child or a placeholder
+                self.child if self.show_child else rio.Spacer(),
+                rio.Switch(is_on=self.bind().show_child),
+            )
+
+
+    app = rio.App(build=lambda: Toggler(OnMountPrinter()))
+    app.run_in_browser()
+    ```
+
+
     ## Metadata
 
     `decorator`: True
     """
     _tag_as_event_handler(handler, EventTag.ON_MOUNT, None)
     return handler
```

### Comparing `rio_ui-0.8.5/rio/fills.py` & `rio_ui-0.8.6/rio/fills.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,18 @@
 
 @dataclass(frozen=True, eq=True)
 class FrostedGlassFill(Fill):
     """
     Fills a shape with a frosted glass effect.
 
     `FrostedGlassFill` fills the shape with a color and applies a blur effect to
-    create a frosted glass appearance.
+    the background, creating a frosted glass appearance.
+
+    Make sure to use a color with transparency, otherwise it will look like a
+    `SolidFill`.
 
     ## Attributes
 
     `color`: The color to fill the shape with.
     `blur_size`: The amount of blur applied to the fill.
     """
```

### Comparing `rio_ui-0.8.5/rio/global_state.py` & `rio_ui-0.8.6/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/icon_registry.py` & `rio_ui-0.8.6/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/inspection.py` & `rio_ui-0.8.6/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/maybes.py` & `rio_ui-0.8.6/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/routing.py` & `rio_ui-0.8.6/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/serialization.py` & `rio_ui-0.8.6/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/session.py` & `rio_ui-0.8.6/rio/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -841,15 +841,17 @@
             self._register_dirty_component(
                 child,
                 include_children_recursively=True,
             )
 
     def _refresh_sync(
         self,
-    ) -> tuple[set[rio.Component], set[rio.Component], set[rio.Component]]:
+    ) -> tuple[
+        set[rio.Component], Iterable[rio.Component], Iterable[rio.Component]
+    ]:
         """
         See `refresh` for details on what this function does.
 
         The refresh process must be performed atomically, without ever yielding
         control flow to the async event loop. TODO WHY
 
         To make sure async isn't used unintentionally this part of the refresh
@@ -992,16 +994,16 @@
 
         visited_and_live_components: set[rio.Component] = {
             component
             for component in visited_components
             if component._is_in_component_tree(is_in_component_tree_cache)
         }
 
-        all_children_old = set()
-        all_children_new = set()
+        all_children_old = set[rio.Component]()
+        all_children_new = set[rio.Component]()
 
         for component in visited_and_live_components:
             # Fundamental components aren't tracked, since they are never built
             if isinstance(
                 component, fundamental_component.FundamentalComponent
             ):
                 continue
@@ -1011,18 +1013,42 @@
             )
             all_children_new.update(
                 self._weak_component_data_by_component[
                     component
                 ].all_children_in_build_boundary
             )
 
+        # Find out which components were mounted or unmounted
+        mounted_components = all_children_new - all_children_old
+        unmounted_components = all_children_old - all_children_new
+
+        # The state/children of newly mounted components must also be sent to
+        # the client.
+        unvisited_mounted_components = (
+            mounted_components - visited_and_live_components
+        )
+
+        while unvisited_mounted_components:
+            visited_and_live_components.update(unvisited_mounted_components)
+
+            new_children = list[rio.Component]()
+            for component in unvisited_mounted_components:
+                if not isinstance(
+                    component, fundamental_component.FundamentalComponent
+                ):
+                    new_children += component._iter_component_tree(
+                        include_root=False
+                    )
+
+            unvisited_mounted_components = new_children
+
         return (
             visited_and_live_components,
-            all_children_old,
-            all_children_new,
+            mounted_components,
+            unmounted_components,
         )
 
     async def _refresh(self) -> None:
         """
         Make sure the session state is up to date. Specifically:
 
         - Call build on all components marked as dirty
@@ -1039,29 +1065,18 @@
             # Clear the dict of crashed build functions
             self._crashed_build_functions.clear()
 
             while self._dirty_components:
                 # Refresh and get a set of all components which have been visited
                 (
                     visited_components,
-                    all_children_old,
-                    all_children_new,
+                    mounted_components,
+                    unmounted_components,
                 ) = self._refresh_sync()
 
-                # Find all components which have recently been added to or
-                # removed from the component tree
-                mounted_components = all_children_new - all_children_old
-                unmounted_components = all_children_old - all_children_new
-
-                # Any components which were previously unmounted, and are now
-                # mounted may not show up in the `visited_components` set, but
-                # must be sent to the client because it considers them to be
-                # dead.
-                visited_components |= mounted_components
-
                 # Avoid sending empty messages
                 if not visited_components:
                     return
 
                 # Serialize all components which have been visited
                 delta_states: dict[int, JsonDoc] = {
                     component._id: serialization.serialize_and_host_component(
```

### Comparing `rio_ui-0.8.5/rio/session_attachments.py` & `rio_ui-0.8.6/rio/session_attachments.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/state_properties.py` & `rio_ui-0.8.6/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/testing.py` & `rio_ui-0.8.6/rio/testing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/text_style.py` & `rio_ui-0.8.6/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/theme.py` & `rio_ui-0.8.6/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/user_settings_module.py` & `rio_ui-0.8.6/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/utils.py` & `rio_ui-0.8.6/rio/utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/world_units.py` & `rio_ui-0.8.6/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto/LICENSE.txt` & `rio_ui-0.8.6/rio/assets/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.8.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.8.6/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.8.6/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.8.6/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.8.6/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/__init__.py` & `rio_ui-0.8.6/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/cli_instance.py` & `rio_ui-0.8.6/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/nice_traceback.py` & `rio_ui-0.8.6/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/project.py` & `rio_ui-0.8.6/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/project_setup.py` & `rio_ui-0.8.6/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/rio_api.py` & `rio_ui-0.8.6/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/rioignore.py` & `rio_ui-0.8.6/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/tomlconfig.py` & `rio_ui-0.8.6/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/run_project/app_loading.py` & `rio_ui-0.8.6/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/run_project/arbiter.py` & `rio_ui-0.8.6/rio/cli/run_project/arbiter.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.8.6/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.8.6/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/cli/run_project/webview_worker.py` & `rio_ui-0.8.6/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/__init__.py` & `rio_ui-0.8.6/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/app_root.py` & `rio_ui-0.8.6/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/auto_form.py` & `rio_ui-0.8.6/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/banner.py` & `rio_ui-0.8.6/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/build_failed.py` & `rio_ui-0.8.6/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/button.py` & `rio_ui-0.8.6/rio/components/button.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/card.py` & `rio_ui-0.8.6/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/class_container.py` & `rio_ui-0.8.6/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/code_block.py` & `rio_ui-0.8.6/rio/components/code_block.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/color_picker.py` & `rio_ui-0.8.6/rio/components/color_picker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/component.py` & `rio_ui-0.8.6/rio/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -631,21 +631,24 @@
             yield cur
 
             if recurse_into_high_level_components or isinstance(
                 cur, fundamental_component.FundamentalComponent
             ):
                 to_do.extend(cur._iter_direct_children())
 
-    def _iter_component_tree(self) -> Iterable[Component]:
+    def _iter_component_tree(
+        self, *, include_root: bool = True
+    ) -> Iterable[Component]:
         """
         Iterate over all components in the component tree, with this component as the root.
         """
         from . import fundamental_component  # Avoid circular import problem
 
-        yield self
+        if include_root:
+            yield self
 
         if isinstance(self, fundamental_component.FundamentalComponent):
             for child in self._iter_direct_children():
                 yield from child._iter_component_tree()
         else:
             build_result = self.session._weak_component_data_by_component[
                 self
```

### Comparing `rio_ui-0.8.5/rio/components/component_tree.py` & `rio_ui-0.8.6/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/container.py` & `rio_ui-0.8.6/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/devel_component.py` & `rio_ui-0.8.6/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/drawer.py` & `rio_ui-0.8.6/rio/components/drawer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/dropdown.py` & `rio_ui-0.8.6/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/flow_container.py` & `rio_ui-0.8.6/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/fundamental_component.py` & `rio_ui-0.8.6/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/grid.py` & `rio_ui-0.8.6/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/html.py` & `rio_ui-0.8.6/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/icon.py` & `rio_ui-0.8.6/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/image.py` & `rio_ui-0.8.6/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/key_event_listener.py` & `rio_ui-0.8.6/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/labeled_column.py` & `rio_ui-0.8.6/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/linear_containers.py` & `rio_ui-0.8.6/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/link.py` & `rio_ui-0.8.6/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/list_items.py` & `rio_ui-0.8.6/rio/components/list_items.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/list_view.py` & `rio_ui-0.8.6/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/markdown.py` & `rio_ui-0.8.6/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/media_player.py` & `rio_ui-0.8.6/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/mouse_event_listener.py` & `rio_ui-0.8.6/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/multi_line_text_input.py` & `rio_ui-0.8.6/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/node_input.py` & `rio_ui-0.8.6/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/node_output.py` & `rio_ui-0.8.6/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/number_input.py` & `rio_ui-0.8.6/rio/components/number_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/overlay.py` & `rio_ui-0.8.6/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/page_view.py` & `rio_ui-0.8.6/rio/components/page_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/plot.py` & `rio_ui-0.8.6/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/popup.py` & `rio_ui-0.8.6/rio/components/popup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/progress_bar.py` & `rio_ui-0.8.6/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/progress_circle.py` & `rio_ui-0.8.6/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/rectangle.py` & `rio_ui-0.8.6/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/revealer.py` & `rio_ui-0.8.6/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/root_components.py` & `rio_ui-0.8.6/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/scroll_container.py` & `rio_ui-0.8.6/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/scroll_target.py` & `rio_ui-0.8.6/rio/components/scroll_target.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/separator.py` & `rio_ui-0.8.6/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/slider.py` & `rio_ui-0.8.6/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/slideshow.py` & `rio_ui-0.8.6/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/spacer.py` & `rio_ui-0.8.6/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/stack.py` & `rio_ui-0.8.6/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/switch.py` & `rio_ui-0.8.6/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/switcher_bar.py` & `rio_ui-0.8.6/rio/components/switcher_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/table.py` & `rio_ui-0.8.6/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/text.py` & `rio_ui-0.8.6/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/text_input.py` & `rio_ui-0.8.6/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/theme_context_switcher.py` & `rio_ui-0.8.6/rio/components/theme_context_switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/tooltip.py` & `rio_ui-0.8.6/rio/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/components/website.py` & `rio_ui-0.8.6/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/monkeypatches.py` & `rio_ui-0.8.6/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/typing_utils.py` & `rio_ui-0.8.6/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/validator.py` & `rio_ui-0.8.6/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/component_details.py` & `rio_ui-0.8.6/rio/debug/dev_tools/component_details.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/deploy_page.py` & `rio_ui-0.8.6/rio/debug/dev_tools/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/dev_tools_sidebar.py` & `rio_ui-0.8.6/rio/debug/dev_tools/dev_tools_sidebar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/docs_page.py` & `rio_ui-0.8.6/rio/debug/dev_tools/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/icons_page.py` & `rio_ui-0.8.6/rio/debug/dev_tools/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/layout_preview.py` & `rio_ui-0.8.6/rio/debug/dev_tools/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/project_page.py` & `rio_ui-0.8.6/rio/debug/dev_tools/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/sample_icons_grid.py` & `rio_ui-0.8.6/rio/debug/dev_tools/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/theme_picker_page.py` & `rio_ui-0.8.6/rio/debug/dev_tools/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/debug/dev_tools/tree_page.py` & `rio_ui-0.8.6/rio/debug/dev_tools/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/docs/__init__.py` & `rio_ui-0.8.6/rio/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/frontend files/index.html` & `rio_ui-0.8.6/rio/frontend files/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 
             // Create a Promise that resolves when the CSS is done loading
             let { cssLoaded, resolveCssLoaded, rejectCssLoaded } =
                 Promise.withResolvers();
         </script>
         
         
-      <script type="module" crossorigin src="/rio/frontend/assets/index-a8d525bb.js"></script>
-      <link rel="stylesheet" href="/rio/frontend/assets/index-4c436499.css">
+      <script type="module" crossorigin src="/rio/frontend/assets/index-8ca8e5f1.js"></script>
+      <link rel="stylesheet" href="/rio/frontend/assets/index-9eba151c.css">
     </head>
 
     <body class="rio-switcheroo-background"></body>
 </html>
```

### Comparing `rio_ui-0.8.5/rio/frontend files/assets/index-4c436499.css` & `rio_ui-0.8.6/rio/frontend files/assets/index-9eba151c.css`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-@charset "UTF-8";.rio-switcheroo-background{--rio-local-bg: var(--rio-global-background-bg);--rio-local-bg-variant: var(--rio-global-background-bg-variant);--rio-local-bg-active: var(--rio-global-background-bg-active);--rio-local-fg: var(--rio-global-background-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-global-heading1-color);--rio-local-heading1-background: var(--rio-global-heading1-background);--rio-local-heading1-background-clip: var( --rio-global-heading1-background-clip );--rio-local-heading1-fill-color: var(--rio-global-heading1-fill-color);--rio-local-heading1-font-weight: var(--rio-global-heading1-font-weight);--rio-local-heading2-color: var(--rio-global-heading2-color);--rio-local-heading2-background: var(--rio-global-heading2-background);--rio-local-heading2-background-clip: var( --rio-global-heading2-background-clip );--rio-local-heading2-fill-color: var(--rio-global-heading2-fill-color);--rio-local-heading2-font-weight: var(--rio-global-heading2-font-weight);--rio-local-heading3-color: var(--rio-global-heading3-color);--rio-local-heading3-background: var(--rio-global-heading3-background);--rio-local-heading3-background-clip: var( --rio-global-heading3-background-clip );--rio-local-heading3-fill-color: var(--rio-global-heading3-fill-color);--rio-local-heading3-font-weight: var(--rio-global-heading3-font-weight);--rio-local-text-color: var(--rio-global-text-color);--rio-local-text-background: var(--rio-global-text-background);--rio-local-text-background-clip: var(--rio-global-text-background-clip);--rio-local-text-fill-color: var(--rio-global-text-fill-color);--rio-local-text-font-weight: var(--rio-global-text-font-weight);color:var(--rio-local-fg)}.rio-switcheroo-neutral{--rio-local-bg: var(--rio-global-neutral-bg);--rio-local-bg-variant: var(--rio-global-neutral-bg-variant);--rio-local-bg-active: var(--rio-global-neutral-bg-active);--rio-local-fg: var(--rio-global-neutral-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-global-heading1-color);--rio-local-heading1-background: var(--rio-global-heading1-background);--rio-local-heading1-background-clip: var( --rio-global-heading1-background-clip );--rio-local-heading1-fill-color: var(--rio-global-heading1-fill-color);--rio-local-heading1-font-weight: var(--rio-global-heading1-font-weight);--rio-local-heading2-color: var(--rio-global-heading2-color);--rio-local-heading2-background: var(--rio-global-heading2-background);--rio-local-heading2-background-clip: var( --rio-global-heading2-background-clip );--rio-local-heading2-fill-color: var(--rio-global-heading2-fill-color);--rio-local-heading2-font-weight: var(--rio-global-heading2-font-weight);--rio-local-heading3-color: var(--rio-global-heading3-color);--rio-local-heading3-background: var(--rio-global-heading3-background);--rio-local-heading3-background-clip: var( --rio-global-heading3-background-clip );--rio-local-heading3-fill-color: var(--rio-global-heading3-fill-color);--rio-local-heading3-font-weight: var(--rio-global-heading3-font-weight);--rio-local-text-color: var(--rio-global-text-color);--rio-local-text-background: var(--rio-global-text-background);--rio-local-text-background-clip: var(--rio-global-text-background-clip);--rio-local-text-fill-color: var(--rio-global-text-fill-color);--rio-local-text-font-weight: var(--rio-global-text-font-weight);color:var(--rio-local-fg)}.rio-switcheroo-hud{--rio-local-bg: var(--rio-global-hud-bg);--rio-local-bg-variant: var(--rio-global-hud-bg-variant);--rio-local-bg-active: var(--rio-global-hud-bg-active);--rio-local-fg: var(--rio-global-hud-fg);--rio-local-level-2-bg: var(--rio-global-primary-bg);--rio-local-level-2-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-2-fg: var(--rio-global-primary-fg);--rio-local-level-3-bg: var(--rio-global-secondary-bg);--rio-local-level-3-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-3-fg: var(--rio-global-secondary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-primary{--rio-local-bg: var(--rio-global-primary-bg);--rio-local-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-bg-active: var(--rio-global-primary-bg-active);--rio-local-fg: var(--rio-global-primary-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-secondary{--rio-local-bg: var(--rio-global-secondary-bg);--rio-local-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-bg-active: var(--rio-global-secondary-bg-active);--rio-local-fg: var(--rio-global-secondary-fg);--rio-local-level-2-bg: var(--rio-global-primary-bg);--rio-local-level-2-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-2-fg: var(--rio-global-primary-fg);--rio-local-level-3-bg: var(--rio-global-secondary-bg);--rio-local-level-3-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-3-fg: var(--rio-global-secondary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-success{--rio-local-bg: var(--rio-global-success-bg);--rio-local-bg-variant: var(--rio-global-success-bg-variant);--rio-local-bg-active: var(--rio-global-success-bg-active);--rio-local-fg: var(--rio-global-success-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-warning{--rio-local-bg: var(--rio-global-warning-bg);--rio-local-bg-variant: var(--rio-global-warning-bg-variant);--rio-local-bg-active: var(--rio-global-warning-bg-active);--rio-local-fg: var(--rio-global-warning-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-danger{--rio-local-bg: var(--rio-global-danger-bg);--rio-local-bg-variant: var(--rio-global-danger-bg-variant);--rio-local-bg-active: var(--rio-global-danger-bg-active);--rio-local-fg: var(--rio-global-danger-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-disabled{--rio-local-bg: var(--rio-global-disabled-bg);--rio-local-bg-variant: var(--rio-global-disabled-bg-variant);--rio-local-bg-active: var(--rio-global-disabled-bg-active);--rio-local-fg: var(--rio-global-disabled-fg);--rio-local-level-2-bg: var(--rio-global-disabled-bg);--rio-local-level-2-bg-variant: var(--rio-global-disabled-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-disabled-bg-active);--rio-local-level-2-fg: var(--rio-global-disabled-fg);--rio-local-level-3-bg: var(--rio-global-disabled-bg);--rio-local-level-3-bg-variant: var(--rio-global-disabled-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-disabled-bg-active);--rio-local-level-3-fg: var(--rio-global-disabled-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-custom{--rio-local-bg: var(--rio-custom-local-bg);--rio-local-bg-variant: var(--rio-custom-local-bg-variant);--rio-local-bg-active: var(--rio-custom-local-bg-active);--rio-local-fg: var(--rio-custom-local-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-background>*,.rio-switcheroo-neutral>*,.rio-switcheroo-hud>*,.rio-switcheroo-primary>*,.rio-switcheroo-secondary>*,.rio-switcheroo-success>*,.rio-switcheroo-warning>*,.rio-switcheroo-danger>*,.rio-switcheroo-disabled>*,.rio-switcheroo-custom>*,.rio-switcheroo-bump>*{--rio-buffer-level-2-bg: var(--rio-local-level-2-bg);--rio-buffer-level-2-bg-variant: var(--rio-local-level-2-bg-variant);--rio-buffer-level-2-bg-active: var(--rio-local-level-2-bg-active);--rio-buffer-level-2-fg: var(--rio-local-level-2-fg);--rio-buffer-level-3-bg: var(--rio-local-level-3-bg);--rio-buffer-level-3-bg-variant: var(--rio-local-level-3-bg-variant);--rio-buffer-level-3-bg-active: var(--rio-local-level-3-bg-active);--rio-buffer-level-3-fg: var(--rio-local-level-3-fg)}.rio-switcheroo-bump{--rio-local-bg: var(--rio-buffer-level-2-bg);--rio-local-bg-variant: var(--rio-buffer-level-2-bg-variant);--rio-local-bg-active: var(--rio-buffer-level-2-bg-active);--rio-local-fg: var(--rio-buffer-level-2-fg);--rio-local-level-2-bg: var(--rio-buffer-level-3-bg);--rio-local-level-2-bg-variant: var(--rio-buffer-level-3-bg-variant);--rio-local-level-2-bg-active: var(--rio-buffer-level-3-bg-active);--rio-local-level-2-fg: var(--rio-buffer-level-3-fg);--rio-local-level-3-bg: var(--rio-buffer-level-2-bg);--rio-local-level-3-bg-variant: var(--rio-buffer-level-2-bg-variant);--rio-local-level-3-bg-active: var(--rio-buffer-level-2-bg-active);--rio-local-level-3-fg: var(--rio-buffer-level-2-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}html[data-theme=light] pre code.hljs{display:block;overflow-x:auto;padding:1rem}html[data-theme=light] code.hljs{padding:3px 5px}html[data-theme=light] .hljs{background:#f3f3f3;color:#444}html[data-theme=light] .hljs-comment{color:#697070}html[data-theme=light] .hljs-punctuation,html[data-theme=light] .hljs-tag{color:#444a}html[data-theme=light] .hljs-tag .hljs-attr,html[data-theme=light] .hljs-tag .hljs-name{color:#444}html[data-theme=light] .hljs-attribute,html[data-theme=light] .hljs-doctag,html[data-theme=light] .hljs-keyword,html[data-theme=light] .hljs-meta .hljs-keyword,html[data-theme=light] .hljs-name,html[data-theme=light] .hljs-selector-tag{font-weight:700}html[data-theme=light] .hljs-deletion,html[data-theme=light] .hljs-number,html[data-theme=light] .hljs-quote,html[data-theme=light] .hljs-selector-class,html[data-theme=light] .hljs-selector-id,html[data-theme=light] .hljs-string,html[data-theme=light] .hljs-template-tag,html[data-theme=light] .hljs-type{color:#800}html[data-theme=light] .hljs-section,html[data-theme=light] .hljs-title{color:#800;font-weight:700}html[data-theme=light] .hljs-link,html[data-theme=light] .hljs-operator,html[data-theme=light] .hljs-regexp,html[data-theme=light] .hljs-selector-attr,html[data-theme=light] .hljs-selector-pseudo,html[data-theme=light] .hljs-symbol,html[data-theme=light] .hljs-template-variable,html[data-theme=light] .hljs-variable{color:#ab5656}html[data-theme=light] .hljs-literal{color:#695}html[data-theme=light] .hljs-addition,html[data-theme=light] .hljs-built_in,html[data-theme=light] .hljs-bullet,html[data-theme=light] .hljs-code{color:#397300}html[data-theme=light] .hljs-meta{color:#1f7199}html[data-theme=light] .hljs-meta .hljs-string{color:#38a}html[data-theme=light] .hljs-emphasis{font-style:italic}html[data-theme=light] .hljs-strong{font-weight:700}html[data-theme=dark] .hljs{color:#ddd;background:#303030}html[data-theme=dark] .hljs-keyword,html[data-theme=dark] .hljs-selector-tag,html[data-theme=dark] .hljs-literal,html[data-theme=dark] .hljs-section,html[data-theme=dark] .hljs-link{color:#fff}html[data-theme=dark] .hljs-string,html[data-theme=dark] .hljs-title,html[data-theme=dark] .hljs-name,html[data-theme=dark] .hljs-type,html[data-theme=dark] .hljs-attribute,html[data-theme=dark] .hljs-symbol,html[data-theme=dark] .hljs-bullet,html[data-theme=dark] .hljs-built_in,html[data-theme=dark] .hljs-addition,html[data-theme=dark] .hljs-variable,html[data-theme=dark] .hljs-template-tag,html[data-theme=dark] .hljs-template-variable{color:#d88}html[data-theme=dark] .hljs-comment,html[data-theme=dark] .hljs-quote,html[data-theme=dark] .hljs-deletion,html[data-theme=dark] .hljs-meta{color:#979797}html[data-theme=dark] .hljs-keyword,html[data-theme=dark] .hljs-selector-tag,html[data-theme=dark] .hljs-literal,html[data-theme=dark] .hljs-title,html[data-theme=dark] .hljs-section,html[data-theme=dark] .hljs-doctag,html[data-theme=dark] .hljs-type,html[data-theme=dark] .hljs-name,html[data-theme=dark] .hljs-strong{font-weight:700}html[data-theme=dark] .hljs-emphasis{font-style:italic}@keyframes content-loading{0%{background-position:-100rem 0}to{background-position:0 0}}.rio-content-loading{background-image:linear-gradient(to right,transparent 10%,var(--rio-local-level-2-bg) 12%,transparent 14%);background-size:100rem 5rem;animation:content-loading 3s linear infinite}@keyframes barber-pole{0%{background-position:0 0}to{background-position:3rem 0rem}}a{color:var(--rio-local-level-2-bg)}a:hover{color:var(--rio-local-level-2-bg-active)}code{font-family:var(--rio-global-monospace-font),monospace}html{background:var(--rio-global-background-bg);overflow:hidden}body{margin:0;padding:0;font-family:var(--rio-global-font, sans-serif)}input,textarea,select{font-family:inherit;font-size:1rem}.rio-component{position:absolute}.rio-fundamental-root-component{position:relative!important;width:100vw;height:100vh}.rio-dev-tools{pointer-events:auto}.rio-dev-tools-hidden:after{pointer-events:none;position:fixed;top:0;right:.1rem;bottom:0;content:"Screen too small for Dev Tools";color:var(--rio-global-neutral-fg);font-size:.8rem;writing-mode:vertical-rl;text-align:center;opacity:.5}.rio-linear-child-container{pointer-events:none;display:flex;align-items:stretch}.rio-linear-child-container>*{position:relative!important}.rio-list-view>div>*:first-child{position:relative!important}.rio-column{flex-direction:column}.rio-grid{pointer-events:none;display:grid}.rio-text{pointer-events:auto;display:flex;align-items:center;color:var(--rio-local-text-color)}.rio-text>div{flex-grow:1;overflow:hidden}.rio-rectangle{pointer-events:auto;border-style:solid;transition-property:background,stroke-color,stroke-width,border-radius,shadow-color,shadow-radius,shadow-offset;transition-timing-function:ease;background:var(--rio-rectangle-background);-webkit-backdrop-filter:var(--rio-rectangle-backdrop-filter);backdrop-filter:var(--rio-rectangle-backdrop-filter);border-color:var(--rio-rectangle-stroke_color);border-width:var(--rio-rectangle-stroke_width);border-radius:var(--rio-rectangle-corner_radius);box-shadow:var(--rio-rectangle-shadow_offset_x) var(--rio-rectangle-shadow_offset_y) var(--rio-rectangle-shadow_radius) var(--rio-rectangle-shadow_color);box-sizing:border-box}.rio-rectangle:hover{background:var(--rio-rectangle-hover-background);-webkit-backdrop-filter:var(--rio-rectangle-hover-backdrop-filter);backdrop-filter:var(--rio-rectangle-hover-backdrop-filter);border-color:var(--rio-rectangle-hover-stroke_color);border-width:var(--rio-rectangle-hover-stroke_width);border-radius:var(--rio-rectangle-hover-corner_radius);box-shadow:var(--rio-rectangle-hover-shadow_offset_x) var(--rio-rectangle-hover-shadow_offset_y) var(--rio-rectangle-hover-shadow_radius) var(--rio-rectangle-hover-shadow_color)}.rio-rectangle-ripple{overflow:hidden}.rio-text-input{cursor:text}.rio-text-input-hint-text{display:flex;align-items:end;-webkit-user-select:none;user-select:none;padding-bottom:.6rem;color:var(--rio-local-text-color);opacity:0;transition:all .13s linear}.rio-text-input-prefix-text{padding-left:.8rem;margin-right:.2rem}.rio-text-input-suffix-text{padding-right:.8rem;margin-left:.2rem}input:not(:placeholder-shown)~.rio-text-input-hint-text,.rio-input-box:focus-within>.rio-text-input-hint-text,.rio-input-box-focused>.rio-text-input-hint-text{opacity:.5}.rio-text-input.rio-input-box{padding-left:0!important;padding-right:0!important}.rio-input-box{pointer-events:auto;display:flex;flex-direction:row;align-items:stretch;padding-left:.8rem;padding-right:.8rem;box-sizing:border-box;background-color:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small) var(--rio-global-corner-radius-small) 0 0}.rio-input-box:not(.rio-disabled-input){overflow:hidden}.rio-input-box:focus-within,.rio-input-box.rio-input-box-focused{outline:none;background-color:var(--rio-local-bg-active)}.rio-input-box>input,.rio-input-box>textarea{flex-grow:1;min-width:0;background-color:transparent;color:var(--rio-local-text-color);caret-color:var(--rio-local-level-2-bg);border:none}.rio-input-box>input{height:calc(200% - 2.38rem)}.rio-input-box>textarea{margin-top:1.5rem;width:100%;resize:none;padding:0 .8rem}.rio-input-box>input:active,.rio-input-box>textarea:active{background-color:transparent}.rio-input-box>input:focus-visible,.rio-input-box>textarea:focus-visible{outline:none}.rio-input-box-label{pointer-events:none;position:absolute;left:.8rem;top:calc(50% - .5rem);font-size:1rem;color:var(--rio-local-text-color);opacity:.5;transition:all .13s linear}input:not(:placeholder-shown)~.rio-input-box-label,textarea:not(:placeholder-shown)~.rio-input-box-label,.rio-input-box:focus-within>.rio-input-box-label,.rio-input-box-focused>.rio-input-box-label{opacity:1;top:.4rem;bottom:unset;font-size:.8rem}.rio-input-box:focus-within>.rio-input-box-label,.rio-input-box-focused>.rio-input-box-label{color:var(--rio-local-level-2-bg)}.rio-input-box-plain-bar,.rio-input-box-color-bar{position:absolute;bottom:0;height:.12rem}.rio-input-box-plain-bar{background-color:var(--rio-local-text-color);left:0;right:0;opacity:.15}.rio-input-box-color-bar{background-color:var(--rio-local-level-2-bg);left:40%;right:40%;opacity:0;transition:all .2s ease-in-out}.rio-input-box:focus-within .rio-input-box-color-bar,.rio-input-box-focused .rio-input-box-color-bar{left:0;right:0;opacity:1}.rio-stack{pointer-events:none;display:inline-grid}.rio-stack>*{grid-column-start:1;grid-row-start:1}.rio-switch{display:flex}.rio-switch>*{pointer-events:auto;position:relative;width:3.18rem;height:1.54rem;margin:auto;border-radius:4.3rem;background-color:var(--rio-global-disabled-bg-variant);transition:.3s ease all;z-index:1}.rio-switch.is-on>*{background-color:var(--rio-local-level-2-bg)}.rio-switch input{position:relative;width:100%;height:100%;padding:0;margin:0;opacity:0;cursor:pointer;z-index:3}.rio-switch .knob{z-index:2;position:absolute;top:.17rem;left:.17rem;width:.86rem;height:.43rem;padding:.39rem .17rem;background-color:var(--rio-global-disabled-bg);border-radius:50%;transition:.3s ease all,left .3s cubic-bezier(.18,.89,.35,1.15)}.rio-switch input:active+.knob{width:1.98rem;border-radius:4.3rem}.rio-switch.is-on input:active+.knob{margin-left:-1.12rem}.rio-switch.is-on input+.knob{left:1.8rem;background-color:var(--rio-local-bg)}.rio-dropdown{pointer-events:auto}.rio-dropdown:not(.rio-disabled-input),.rio-dropdown:not(.rio-disabled-input)>input{cursor:pointer}.rio-dropdown-popup{position:absolute;z-index:10003;height:0;max-height:100vh;background-color:var(--rio-global-background-bg);color:var(--rio-global-text-color);border-radius:0 0 var(--rio-global-corner-radius-small) var(--rio-global-corner-radius-small);box-shadow:0 0 .8rem var(--rio-global-shadow-color);transition:height .2s ease-in-out}.rio-dropdown-popup-above{border-radius:var(--rio-global-corner-radius-small)!important}.rio-dropdown.rio-input-box>.rio-dropdown-arrow{pointer-events:none;order:2;display:flex;align-items:center}.rio-dropdown.rio-input-box>.rio-dropdown-arrow svg{width:1.3rem;height:1.3rem}.rio-dropdown-option-highlight{font-weight:700;color:var(--rio-local-level-2-bg)}.rio-dropdown-options{position:relative;display:flex;flex-direction:column;align-items:stretch;cursor:pointer}.rio-dropdown-options>div{position:relative}.rio-dropdown-options>svg{position:relative;width:4rem;height:4rem;margin:1.5rem auto;opacity:.2}.rio-dropdown-option:after{content:"";pointer-events:none;position:absolute;top:0;left:0;right:0;bottom:0;background-color:var(--rio-global-primary-bg);opacity:0;transition:opacity .1s ease-in-out}.rio-dropdown-option-highlighted:after{opacity:.2}.rio-progress-bar{pointer-events:none;overflow:hidden}.rio-progress-bar-track{position:absolute;width:100%;height:100%;background:var(--rio-local-text-color);opacity:.3}.rio-progress-bar-fill{position:absolute;height:100%;background:var(--rio-local-bg)}@keyframes rio-progress-bar-animation-indeterminate{0%{left:-20%;width:6%}50%{width:30%}to{left:120%;width:6%}}.rio-progress-bar-indeterminate .rio-progress-bar-fill{transform:translate(-50%);animation:rio-progress-bar-animation-indeterminate 1.5s ease-in-out infinite}.rio-progress-bar:not(.rio-progress-bar-indeterminate) .rio-progress-bar-fill{left:0;width:var(--rio-progress-bar-fraction);transition:width .3s ease-in-out}.rio-progress-circle{pointer-events:auto;stroke:var(--rio-local-bg);display:flex;justify-content:center;overflow:hidden}.rio-progress-circle circle{fill:none;stroke-width:3.5;color:var(--rio-local-bg)}.spinning svg{transform-origin:center;animation:rotate 2s linear infinite}.spinning .progress{stroke-dasharray:1,200;stroke-dashoffset:0;stroke-linecap:round;animation:dash 1.5s ease-in-out infinite}.rio-progress-circle:not(.spinning) .progress{stroke-dashoffset:-94.25;stroke-dasharray:var(--dasharray);transition:stroke-dasharray .5s ease}@keyframes rotate{to{transform:rotate(360deg)}}@keyframes dash{0%{stroke-dasharray:1,200;stroke-dashoffset:0}50%{stroke-dasharray:90,200;stroke-dashoffset:-35px}to{stroke-dashoffset:-125px}}.rio-button{--outer-text-color: var(--rio-local-text-color)}.rio-button>*{pointer-events:auto;position:relative;width:100%;height:100%;overflow:hidden;transition:color .1s ease-in-out,border-color .1s ease-in-out}.rio-buttonstyle-major{background-color:var(--rio-local-bg);box-shadow:0 0 0 transparent;transition:background-color .1s ease-in-out,box-shadow .2s ease-in-out}.rio-buttonstyle-major:hover:not(.rio-switcheroo-disabled){background-color:var(--rio-local-bg-active);cursor:pointer;box-shadow:0 .1rem .22rem #00000059}.rio-buttonstyle-minor:not(:hover){outline:.1rem solid var(--rio-local-bg);--rio-local-text-color: var(--rio-local-bg)}.rio-buttonstyle-minor:hover:not(.rio-switcheroo-disabled){background-color:var(--rio-local-bg);cursor:pointer}.rio-buttonstyle-plain{--rio-local-text-color: var(--outer-text-color)}.rio-buttonstyle-plain:hover:not(.rio-switcheroo-disabled){cursor:pointer;--rio-local-text-color: var(--rio-local-bg)}.rio-shape-pill{border-radius:99999px}.rio-shape-rounded{border-radius:var(--rio-global-corner-radius-small)}.rio-shape-rectangle{border-radius:0}.rio-shape-circle{border-radius:50%}.rio-revealer{display:flex;flex-direction:column;align-items:stretch;justify-content:stretch;border-radius:var(--rio-global-corner-radius-small);transition:background-color .15s ease-out;overflow:hidden}.rio-revealer-header{pointer-events:auto;cursor:pointer;display:flex;align-items:center;justify-content:space-between;color:var(--rio-local-text-color)}.rio-revealer-label{flex-grow:1}.rio-revealer-arrow{transform:rotate(90deg);transition:transform .25s ease-in-out}.rio-revealer-open .rio-revealer-arrow{transform:rotate(0)}.rio-revealer-content-outer{flex-grow:1;position:relative;overflow:hidden}.rio-revealer-content-inner{position:absolute;bottom:0;opacity:0;transform:translateY(-50%);transition:opacity .45s ease-in-out,transform .35s ease}.rio-revealer-open .rio-revealer-content-inner{opacity:1;transform:translateY(0)}.rio-revealer-content-inner>*{position:relative!important}.rio-plot{display:inline-block;display:flex;justify-content:center;align-items:center;overflow:hidden}.rio-icon{pointer-events:auto;display:flex;justify-content:center;align-items:center}.rio-slider{pointer-events:auto;--rio-slider-position-transition-time: .3s}.rio-slider:not(.rio-switcheroo-disabled){cursor:pointer}.rio-slider-inner{pointer-events:none;position:absolute;left:.6rem;right:.6rem;height:.25rem;top:50%;transform:translateY(-50%)}.rio-slider-track{position:absolute;width:100%;height:100%;opacity:.3;background:var(--rio-local-text-color);border-radius:99999px}.rio-slider-fill{position:absolute;left:0;width:var(--rio-slider-fraction);height:100%;background:var(--rio-local-level-2-bg);border-radius:99999px;transition:width var(--rio-slider-position-transition-time) ease-in-out}.rio-slider-glow{position:absolute;left:var(--rio-slider-fraction);top:50%;width:1.1rem;height:1.1rem;transform:translate(-50%,-50%);border-radius:50%;background-color:var(--rio-local-level-2-bg);opacity:0%;transition:left var(--rio-slider-position-transition-time) ease-in-out,width .15s ease-in-out,height .15s ease-in-out,opacity .15s ease-in-out}.rio-slider:hover:not(.rio-switcheroo-disabled) .rio-slider-glow{width:2.8rem;height:2.8rem;opacity:20%}.rio-slider-knob{position:absolute;left:var(--rio-slider-fraction);top:50%;width:1.2rem;height:1.2rem;transform:translate(-50%,-50%);border-radius:50%;background-color:var(--rio-local-level-2-bg);box-shadow:0 .1rem .2rem var(--rio-global-shadow-color);transition:left var(--rio-slider-position-transition-time) ease-in-out,background-color .1s ease-in-out}.rio-slideshow{pointer-events:auto;overflow:hidden}.slideshow-child-container{position:relative;display:grid;width:100%;height:100%}.slideshow-child-container>div{grid-column-start:1;grid-row-start:1;width:100%;height:100%}.slideshow-child-container>div>*{grid-column-start:1;grid-row-start:1;width:100%;height:100%}.slideshow-progress{position:absolute;bottom:0;width:100%;height:.3rem;background-color:var(--rio-local-level-2-bg)}.rio-overlay{pointer-events:none;position:fixed!important;top:0!important;left:0!important;width:unset!important;height:unset!important;z-index:10000}.rio-spacer{pointer-events:none}.rio-media-player{pointer-events:auto}.rio-media-player video{pointer-events:none;width:100%;height:100%;object-fit:contain}.rio-media-player-alt-display{pointer-events:none;position:absolute;left:50%;top:50%;width:50%;height:50%;max-width:20rem;max-height:20rem;aspect-ratio:1;opacity:.5;transform:translate(-50%,-50%)}.rio-media-player-controls{position:absolute;left:0;bottom:0;right:0;background:linear-gradient(rgba(0,0,0,0),rgba(0,0,0,.6));padding-top:2.5rem;display:flex;flex-direction:column;gap:0rem;align-items:stretch;transition:opacity .4s ease-in-out}.rio-media-player-timeline{pointer-events:auto;cursor:pointer;position:relative;height:2rem;margin:0 .5rem}.rio-media-player-timeline>div{pointer-events:none;position:relative;top:50%;height:.2rem;transform:translateY(-50%);transition:height .2s ease-in-out}.rio-media-player-timeline:hover>div{height:.4rem}.rio-media-player-timeline-knob{position:absolute;width:0rem;height:0rem;left:100%;top:50%;background-color:var(--rio-global-primary-bg);border-radius:50%;transform:translate(-50%,-50%);transition:width .2s ease-in-out,height .2s ease-in-out}.rio-media-player-timeline:hover .rio-media-player-timeline-knob{width:.9rem;height:.9rem}.rio-media-player-timeline-background,.rio-media-player-timeline-loaded,.rio-media-player-timeline-hover,.rio-media-player-timeline-played{position:absolute;width:0%;height:100%;background-color:#fff;border-radius:99999px}.rio-media-player-timeline-background{width:100%;opacity:.2}.rio-media-player-timeline-loaded{opacity:.3}.rio-media-player-timeline-hover{opacity:0;transition:opacity .2s ease-in-out}.rio-media-player-timeline-played{background-color:var(--rio-global-primary-bg)}.rio-media-player-controls-row{display:flex;gap:1.2rem;align-items:center;padding:.5rem;padding-top:0}.rio-media-player-button{pointer-events:auto;cursor:pointer;width:2rem;height:2rem}.rio-media-player-button>img{width:100%;height:100%}.rio-media-player-volume{pointer-events:auto;cursor:pointer;position:relative;width:5rem;height:1.5rem}.rio-media-player-volume>div{pointer-events:none;position:relative;top:50%;height:.2rem;transform:translateY(-50%)}.rio-media-player-volume-background,.rio-media-player-volume-current{position:absolute;width:100%;height:100%;border-radius:99999px;background-color:#fff}.rio-media-player-volume-background{opacity:.2}.rio-media-player-volume-knob{position:absolute;width:.9rem;height:.9rem;left:100%;top:50%;background-color:#fff;border-radius:50%;transform:translate(-50%,-50%)}.rio-media-player-volume>div{position:relative;top:50%;height:.2rem;transform:translateY(-50%)}.rio-media-player-playtime-label{color:#fff;opacity:.6}.rio-markdown{pointer-events:auto;color:var(--rio-local-text-color)}.rio-markdown>*,.rio-markdown li>*{margin-top:0;margin-bottom:0}.rio-markdown>*+*,.rio-markdown li>*+*{margin-top:.8rem}.rio-markdown ul{padding-left:1rem;list-style-type:none}.rio-markdown ul>li:before{content:"-";font-weight:700;position:absolute;transform:translate(-.6rem,.1rem)}.rio-markdown li+li{margin-top:.2rem}.rio-markdown code{font-family:var(--rio-global-monospace-font),monospace;background:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small);padding:.1rem .3rem}.rio-markdown h1{font-family:var(--rio-global-heading1-font-name);color:var(--rio-local-heading1-color);font-size:var(--rio-global-heading1-font-size);font-style:var(--rio-global-heading1-italic);font-weight:var(--rio-global-heading1-font-weight);text-decoration:var(--rio-global-heading1-underlined);text-transform:var(--rio-global-heading1-all-caps)}.rio-markdown h1:not(:first-child){margin-top:2rem}.rio-markdown h1:not(:last-child){margin-bottom:1rem}.rio-markdown h2{font-family:var(--rio-global-heading2-font-name);color:var(--rio-local-heading2-color);font-size:var(--rio-global-heading2-font-size);font-style:var(--rio-global-heading2-italic);font-weight:var(--rio-global-heading2-font-weight);text-decoration:var(--rio-global-heading2-underlined);text-transform:var(--rio-global-heading2-all-caps);margin-top:0}.rio-markdown h2:not(:first-child){margin-top:1.5rem}.rio-markdown h2:not(:last-child){margin-bottom:.8rem}.rio-markdown h3{font-family:var(--rio-global-heading3-font-name);color:var(--rio-local-heading3-color);font-size:var(--rio-global-heading3-font-size);font-style:var(--rio-global-heading3-italic);font-weight:var(--rio-global-heading3-font-weight);text-decoration:var(--rio-global-heading3-underlined);text-transform:var(--rio-global-heading3-all-caps);margin-top:0}.rio-markdown h3:not(:first-child){margin-top:1rem}.rio-markdown h3:not(:last-child){margin-bottom:.5rem}.rio-markdown p{font-family:var(--rio-global-font);color:var(--rio-local-text-color);font-size:var(--rio-global-text-font-size);line-height:1.35em;font-style:var(--rio-global-text-italic);font-weight:var(--rio-global-text-font-weight);text-decoration:var(--rio-global-text-underlined);text-transform:var(--rio-global-text-all-caps)}.rio-code-block{pointer-events:auto;display:flex;flex-direction:column;align-items:stretch;gap:.5rem;padding:.5rem;background:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small);box-sizing:border-box}.rio-code-block-header{display:flex;flex-direction:row;align-items:center;justify-content:space-between;gap:1rem;color:var(--rio-local-text-color);font-size:.8rem}.rio-code-block-language{font-weight:700;opacity:.4}.rio-code-block-copy-button{width:1.3rem;height:1.3rem;cursor:pointer;border:none;background:none;border-radius:var(--rio-global-corner-radius-small);margin:0;padding:0;opacity:.4;transition:opacity .2s ease-in-out}.rio-code-block-copy-button:hover{color:var(--rio-local-level-2-bg);opacity:1}.rio-code-block>pre{margin:0;font-size:var(--rio-global-text-font-size);font-family:var(--rio-global-monospace-font),monospace;display:block}.rio-link{pointer-events:auto;cursor:pointer;display:block}.rio-text-link{color:var(--rio-local-level-2-bg);display:flex;align-items:center;justify-content:center}.rio-scroll-container{pointer-events:auto;scroll-behavior:smooth}.rio-scroll-target{pointer-events:auto}.rio-scroll-target>.rio-scroll-target-url-copy-button{display:none}.rio-scroll-target>.rio-scroll-target-url-copy-button>*{position:absolute;cursor:pointer}.rio-scroll-target:hover>.rio-scroll-target-url-copy-button{display:block}.rio-color-picker{pointer-events:none;display:flex;flex-direction:column;align-items:stretch}.rio-color-picker-color-square{pointer-events:auto;position:relative;min-height:6rem;cursor:crosshair;margin-bottom:.7rem;border-radius:var(--rio-global-corner-radius-small);flex-grow:1}.rio-color-picker-slider-outer{pointer-events:auto;position:relative;padding:.7rem 0}.rio-color-slider-inner{height:.9rem;cursor:crosshair;border-radius:99999px}.rio-color-picker-knob{pointer-events:none;cursor:crosshair;width:1.4rem;height:1.4rem;border-radius:50%;border:.2rem solid var(--rio-local-text-color);position:absolute;transform:translate(-50%,-50%);box-sizing:border-box;background:var(--chosen-color-opaque)}.rio-color-picker-slider-outer>.rio-color-picker-knob{top:50%}.color-slider-checkers{border-radius:99999px}.rio-color-picker-hue-bar>.rio-color-slider-inner{background:linear-gradient(to right,red,yellow,lime,aqua,blue,magenta,red)}.rio-color-picker-opacity-bar>.rio-color-slider-inner:not(.rio-checkered){position:absolute;top:.7rem;left:0;right:0;bottom:.7rem;background:linear-gradient(to right,transparent,var(--chosen-color-opaque))}.rio-color-picker-result-container{margin-top:.5rem;margin-left:auto;margin-right:auto;display:flex;align-items:center;gap:.8rem}.rio-color-picker-selected-color-circle{position:relative;width:2.5rem;height:2.5rem}.rio-color-picker-selected-color-circle>*{width:100%;height:100%;border-radius:50%;box-sizing:border-box;border:.2rem solid var(--rio-local-text-color)}.rio-color-picker-selected-color-circle>div:first-child{position:absolute;top:0;left:0;right:0;bottom:0;background:var(--chosen-color-transparent)}.rio-color-picker-selected-color-circle-color{background:var(--chosen-color-transparent)}.rio-color-picker-selected-color-label{pointer-events:auto;opacity:.5;width:5rem;color:var(--rio-local-text-color);font-size:.9rem;text-align:center;font-weight:700;background:transparent;border:none;padding:.3rem;border-radius:.5rem;transition:opacity .1s ease-in-out,color .1s ease-in-out,background-color .1s ease-in-out}.rio-color-picker-selected-color-label:focus{outline:none;opacity:1;color:var(--rio-local-level-2-bg);background:var(--rio-local-bg-variant)}.rio-checkered{--checker-color: #888;--checker-size: .9rem;background-image:linear-gradient(45deg,var(--checker-color) 25%,transparent 25%),linear-gradient(45deg,transparent 75%,var(--checker-color) 75%),linear-gradient(45deg,transparent 75%,var(--checker-color) 75%),linear-gradient(45deg,var(--checker-color) 25%,transparent 25%);background-size:var(--checker-size) var(--checker-size);background-position:0 0,0 0,calc(var(--checker-size) * -.5) calc(var(--checker-size) * -.5),calc(var(--checker-size) * .5) calc(var(--checker-size) * .5)}.rio-drawer{pointer-events:auto;overflow:hidden;display:flex;align-items:stretch}.rio-drawer-shade{pointer-events:none;position:absolute;left:0;top:0;right:0;bottom:0;transition:background-color .3s ease-in-out}.rio-drawer-anchor{pointer-events:none;flex-grow:1}.rio-drawer-content-outer{pointer-events:auto;display:flex;position:absolute;background-color:var(--rio-global-neutral-bg);box-shadow:0 0 1rem var(--rio-global-shadow-color);transition:transform .3s ease-out}.rio-drawer-content-inner{order:1}.rio-drawer-content-inner>*{position:relative!important}.rio-drawer-knob{align-self:center;margin:.5rem;border-radius:99999px;background:var(--rio-local-text-color);opacity:.15}.rio-drawer-left .rio-drawer-knob,.rio-drawer-right .rio-drawer-knob{width:.4rem;height:4rem}.rio-drawer-top .rio-drawer-knob,.rio-drawer-bottom .rio-drawer-knob{width:4rem;height:.4rem}.rio-drawer-top .rio-drawer-content-outer,.rio-drawer-bottom .rio-drawer-content-outer{flex-direction:column}.rio-drawer-left .rio-drawer-knob,.rio-drawer-top .rio-drawer-knob{order:2}.rio-drawer-right .rio-drawer-knob,.rio-drawer-bottom .rio-drawer-knob{order:0}.rio-drawer-left>.rio-drawer-content-outer{top:0;left:0;bottom:0;width:fit-content;border-radius:0 var(--rio-global-corner-radius-large) var(--rio-global-corner-radius-large) 0}.rio-drawer-right>.rio-drawer-content-outer{top:0;right:0;bottom:0;width:fit-content;border-radius:var(--rio-global-corner-radius-large) 0 0 var(--rio-global-corner-radius-large)}.rio-drawer-top>.rio-drawer-content-outer{left:0;top:0;right:0;height:fit-content;border-radius:0 0 var(--rio-global-corner-radius-large) var(--rio-global-corner-radius-large)}.rio-drawer-bottom>.rio-drawer-content-outer{left:0;bottom:0;right:0;height:fit-content;border-radius:var(--rio-global-corner-radius-large) var(--rio-global-corner-radius-large) 0 0}.rio-drawer-no-transition{transition:none!important}.rio-drawer-no-transition>*{transition:none!important}.rio-popup{z-index:10003}.rio-popup-anchor>*,.rio-popup-content>*{position:relative!important}.rio-popup-content{position:fixed;width:min-content;height:min-content;background-color:var(--rio-local-bg);border-radius:var(--rio-global-corner-radius-medium);box-shadow:0 0 1rem var(--rio-global-shadow-color);transform:scale(0);opacity:0;transition:transform .2s linear,opacity .1s ease-in-out}.rio-popup-open>.rio-popup-content{transform:scale(1);opacity:1;transition:transform .2s cubic-bezier(.5,.5,.2,1.14),opacity .1s ease-in-out}.rio-image{pointer-events:auto;display:flex;justify-content:center;align-items:center}.rio-image img{width:100%;height:100%;object-fit:contain}.rio-image svg{max-width:3rem}.rio-card{pointer-events:auto;background-color:var(--rio-local-bg);box-shadow:0 0 0 var(--rio-global-shadow-color);transition:box-shadow .15s ease-out,background-color .1s ease-out}.rio-card-elevate-on-hover:hover{box-shadow:0 .15rem .3rem var(--rio-global-shadow-color)}.rio-card-colorize-on-hover:hover{background-color:var(--rio-local-bg-active)}.rio-card-ripple{overflow:hidden}.rio-switcher-bar{display:flex;align-items:center}.rio-switcher-bar>div{position:relative}.rio-switcher-bar>div>.rio-switcher-bar-options{position:relative!important}.rio-switcher-bar-options{pointer-events:auto;position:absolute;display:flex;align-items:stretch;justify-content:space-between}.rio-switcher-bar-option{display:flex;flex-direction:column;align-items:center;justify-content:space-between;cursor:pointer;border-radius:var(--rio-global-corner-radius-large);color:var(--rio-local-text-color);transition:background-color .1s ease-out}.rio-switcher-bar-option:hover{background-color:var(--rio-local-bg-active)}.rio-switcher-bar-marker>.rio-switcher-bar-options>.rio-switcher-bar-option{background-color:unset!important}.rio-switcher-bar-option>div{margin-left:auto;margin-right:auto;white-space:nowrap}.rio-switcher-bar-marker{pointer-events:none;background:var(--rio-local-bg);overflow:hidden;position:absolute;left:0;top:0;border-radius:var(--rio-global-corner-radius-large)}.rio-table{pointer-events:auto;display:grid}.rio-table>*{padding:.5rem .8rem}.rio-table .header{display:flex;cursor:pointer}.rio-table .header:after{content:"▴";display:inline-block;margin-left:.3rem;opacity:0}.rio-table .header[data-sort=ascending]:after{content:"▴";opacity:1}.rio-table .header[data-sort=descending]:after{content:"▾";opacity:1}.rio-list-view{pointer-events:none;display:flex;flex-direction:column;align-items:stretch}.rio-heading-list-item{pointer-events:none;box-sizing:border-box}.rio-listview-grouped{pointer-events:auto;background-color:var(--rio-local-bg-variant);transition:background-color .1s ease-out}.rio-listview-grouped+.rio-listview-grouped:after{content:"";position:absolute;top:0;left:0;right:0;height:1px;background-color:var(--rio-local-text-color);opacity:.2}.rio-list-item-ripple{overflow:hidden}.rio-list-item-ripple:hover{background:var(--rio-local-bg-active)}.rio-flow-container{display:flex;flex-wrap:wrap}.rio-flow-container>*{transition:left .2s ease-out,top .2s ease-out}.rio-connection-lost-popup{pointer-events:none;position:fixed;left:0;top:0;width:100vw;height:100vh;z-index:10004;background-color:transparent;transition:background-color 1s ease-in-out}.rio-connection-lost-popup.rio-connection-lost-popup-visible{display:flex;align-items:stretch;background-color:#00000080}.rio-connection-lost-popup>*{position:absolute;flex-grow:1;left:0;top:0;width:100%;height:100%;opacity:0;transform:translateY(-5rem);transition:opacity .3s ease-in-out,transform .3s cubic-bezier(.5,.5,.2,1.14)}.rio-connection-lost-popup.rio-connection-lost-popup-visible>*{opacity:1;transform:translateY(0)}.rio-traceback{pointer-events:auto;position:relative;left:50%;top:5rem;width:fit-content;max-width:50rem;padding:2.2rem;overflow:hidden;display:flex;flex-direction:column;align-items:stretch;gap:1.5rem;border-radius:var(--rio-global-corner-radius-large);box-shadow:0 .4rem 1rem var(--rio-global-shadow-color);transform:translate(-50%)}.rio-traceback-header{display:flex;align-items:center;gap:.6rem}.rio-traceback-header>svg{width:2.5rem;height:2.5rem;fill:var(--rio-global-danger-bg)}.rio-traceback-header>div{flex-grow:1;text-align:left;font-size:1.8rem;color:var(--rio-global-danger-bg)}.rio-traceback-traceback{font-family:var(--rio-global-monospace-font),monospace;font-size:.9rem;white-space:pre-wrap;overflow-wrap:break-word;padding:.5rem 1rem;background-color:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small)}.rio-traceback-footer{display:flex;flex-direction:column;gap:.5rem}.rio-traceback-footer-links{display:flex;flex-direction:row;gap:.5rem;justify-content:space-between}.rio-traceback-footer>a{flex:1}.rio-traceback-bold{font-weight:700}.rio-traceback-dim{opacity:.5}.rio-traceback-red{color:var(--rio-global-danger-bg)}.rio-traceback-yellow{color:var(--rio-global-warning-bg)}.rio-dev-tools-connector{pointer-events:auto;display:flex;flex-direction:column;align-items:center;justify-content:end;gap:.1rem;z-index:2;text-decoration:none}.rio-dev-tools-connector img{width:2.5rem;height:2.5rem;object-fit:contain;margin-bottom:.25rem}.rio-dev-tools-connector div{color:var(--rio-local-text-color);transition:color 1s ease-in-out}.rio-dev-tools-connector div:last-child{margin-bottom:1rem}.rio-dev-tools-connector:hover div{color:var(--rio-global-secondary-fg);transition:color .1s ease-in-out}.rio-dev-tools-connector:before{content:"";position:absolute;top:0;right:0;bottom:0;left:0;z-index:-1;background:linear-gradient(to top,var(--rio-global-secondary-bg),transparent);opacity:0;transition:opacity 1s ease-out}.rio-dev-tools-connector:hover:before{opacity:1;transition:opacity .1s ease-out}.rio-dev-tools-component-tree{overflow-x:hidden;overflow-y:auto}.rio-dev-tools-component-tree>*{position:absolute;width:100%;height:100%}.rio-dev-tools-component-tree-item{display:flex;flex-direction:column;gap:.2rem}@keyframes flash-text{0%{color:initial}20%{color:var(--rio-global-warning-bg)}to{color:initial}}.rio-dev-tools-component-tree-flash{animation:flash-text 3s linear}.rio-dev-tools-component-tree-item-header{pointer-events:auto;cursor:pointer;z-index:1;position:relative;padding:.3rem .6rem;display:flex;flex-direction:row;align-items:center;gap:.5rem}.rio-dev-tools-component-tree-item>.rio-dev-tools-component-tree-item-header>div:first-child{width:1rem;height:1rem;transition:transform .1s ease-in-out}.rio-dev-tools-component-tree-item[data-expanded=true]>.rio-dev-tools-component-tree-item-header>div:first-child{transform:rotate(90deg)}.rio-dev-tools-component-tree-item-header:after{pointer-events:none;content:"";display:block;z-index:-1;position:absolute;left:0;top:0;right:0;bottom:0;background:var(--rio-global-secondary-bg);border-radius:99999px;opacity:0;transition:opacity .1s ease-in-out}.rio-dev-tools-component-tree-item-header>div>svg{width:1rem;height:1rem}.rio-dev-tools-component-tree-item-header-weakly-selected{font-weight:700}.rio-dev-tools-component-tree-item-header-strongly-selected{font-weight:700;color:var(--rio-global-secondary-fg)}.rio-dev-tools-component-tree-item-header:hover:after{opacity:.4}.rio-dev-tools-component-tree-item-header-weakly-selected:after{opacity:.15}.rio-dev-tools-component-tree-item-header-strongly-selected:after{opacity:.6}.rio-dev-tools-component-tree-item-header-strongly-selected:hover:after{opacity:.8}.rio-dev-tools-component-tree-item-children{margin-left:.7rem;display:none;flex-direction:column;gap:.2rem}.rio-dev-tools-component-tree-item[data-has-children=true][data-expanded=true]>.rio-dev-tools-component-tree-item-children{display:flex}.rio-dev-tools-component-highlighter{pointer-events:none;position:fixed;z-index:10001;transition:left .3s ease-in-out,top .3s ease-in-out,width .3s ease-in-out,height .3s ease-in-out}@keyframes pulse{0%{left:-.3rem;top:-.3rem;right:-.3rem;bottom:-.3rem;border-width:.4rem}50%{left:-.7rem;top:-.7rem;right:-.7rem;bottom:-.7rem;border-width:.3rem}to{left:-.3rem;top:-.3rem;right:-.3rem;bottom:-.3rem;border-width:.4rem}}.rio-dev-tools-component-highlighter:after{content:"";position:absolute;display:block;border-radius:1rem;box-shadow:0 0 0 9999rem #0009;border-style:solid;border-color:var(--rio-global-secondary-bg);animation:pulse 1.4s infinite}.rio-dev-tools-background{position:relative;background:var(--rio-local-bg)}.rio-dev-tools-background:after{content:"";position:absolute;display:block;z-index:1;left:0;top:0;bottom:0;right:0;background-image:linear-gradient(-45deg,var(--rio-local-bg) 25%,var(--rio-global-secondary-bg) 25%,var(--rio-global-secondary-bg) 50%,var(--rio-local-bg) 50%,var(--rio-local-bg) 75%,var(--rio-global-secondary-bg) 75%,var(--rio-global-secondary-bg));background-size:3rem 3rem;opacity:.03}.rio-switcher{overflow:hidden}.rio-tooltip{pointer-events:none;position:relative}.rio-tooltip-anchor{pointer-events:auto;position:relative}.rio-tooltip-anchor>*,.rio-tooltip-label>*{position:relative!important}.rio-tooltip-label{position:absolute;width:max-content;padding:.5rem;border-radius:var(--rio-global-corner-radius-small);background:var(--rio-global-hud-bg);box-shadow:0 .1rem .2rem var(--rio-global-shadow-color);opacity:0;transition:opacity .15s ease-in-out}.rio-build-failed{pointer-events:auto;color:var(--rio-global-danger-fg);display:flex;flex-direction:column;align-items:stretch;background:var(--rio-global-danger-bg);border-radius:var(--rio-global-corner-radius-small);overflow:hidden;background-image:linear-gradient(-45deg,var(--rio-global-danger-bg-variant) 15%,transparent 15%,transparent 50%,var(--rio-global-danger-bg-variant) 50%,var(--rio-global-danger-bg-variant) 65%,transparent 65%);background-size:3rem 3rem;animation:barber-pole 1s linear infinite}.rio-build-failed-top,.rio-build-failed-bottom{flex-grow:1}.rio-build-failed-top{background:linear-gradient(to top,var(--rio-global-danger-bg),var(--rio-global-danger-bg) 30%,transparent)}.rio-build-failed-bottom{background:linear-gradient(to bottom,var(--rio-global-danger-bg),var(--rio-global-danger-bg) 30%,transparent)}.rio-build-failed-content{padding:1rem;display:flex;flex-direction:column;align-items:stretch;gap:1rem;background:var(--rio-global-danger-bg)}.rio-build-failed-header{align-self:center;display:flex;align-items:center;gap:.5rem}.rio-build-failed-icon{width:2rem;height:2rem}.rio-build-failed-summary{font-weight:700}.rio-build-failed-details{align-self:center}.rio-code-explorer{pointer-events:none;display:flex;align-items:center;justify-content:space-between}.rio-code-explorer-source-code{pointer-events:auto;display:block;cursor:text;white-space:pre;font-size:1rem;font-family:var(--rio-global-monospace-font),monospace;position:relative;width:min-content;background:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-medium)}.rio-code-explorer-build-result{position:relative}.rio-code-explorer-build-result>*:not(.rio-code-explorer-highlighter){position:relative!important}.rio-code-explorer-highlighter{pointer-events:none;position:absolute;opacity:0;transition:opacity .3s ease-in-out,left .3s ease-in-out,top .3s ease-in-out,width .3s ease-in-out,height .3s ease-in-out}.rio-code-explorer-highlighter:after{content:"";z-index:10001;position:absolute;border-radius:1rem;border-style:solid;border-width:.2rem!important;border-color:var(--rio-global-secondary-bg);box-shadow:0 0 4rem 1rem var(--rio-global-secondary-bg);opacity:.4;animation:pulse 1.4s infinite}.rio-separator{position:relative;background-color:var(--rio-local-bg)}.rio-separator:after{content:"";position:absolute;left:0;top:0;right:0;bottom:0;background-color:var(--separator-color);opacity:var(--separator-opacity)}.rio-ripple-effect{pointer-events:none;position:absolute;background:var(--rio-ripple-color);border-radius:50%;transform:translate(-50%,-50%);transition:top var(--rio-ripple-duration),left var(--rio-ripple-duration),width var(--rio-ripple-duration),height var(--rio-ripple-duration),opacity var(--rio-ripple-duration)}
+@charset "UTF-8";.rio-switcheroo-background{--rio-local-bg: var(--rio-global-background-bg);--rio-local-bg-variant: var(--rio-global-background-bg-variant);--rio-local-bg-active: var(--rio-global-background-bg-active);--rio-local-fg: var(--rio-global-background-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-global-heading1-color);--rio-local-heading1-background: var(--rio-global-heading1-background);--rio-local-heading1-background-clip: var( --rio-global-heading1-background-clip );--rio-local-heading1-fill-color: var(--rio-global-heading1-fill-color);--rio-local-heading1-font-weight: var(--rio-global-heading1-font-weight);--rio-local-heading2-color: var(--rio-global-heading2-color);--rio-local-heading2-background: var(--rio-global-heading2-background);--rio-local-heading2-background-clip: var( --rio-global-heading2-background-clip );--rio-local-heading2-fill-color: var(--rio-global-heading2-fill-color);--rio-local-heading2-font-weight: var(--rio-global-heading2-font-weight);--rio-local-heading3-color: var(--rio-global-heading3-color);--rio-local-heading3-background: var(--rio-global-heading3-background);--rio-local-heading3-background-clip: var( --rio-global-heading3-background-clip );--rio-local-heading3-fill-color: var(--rio-global-heading3-fill-color);--rio-local-heading3-font-weight: var(--rio-global-heading3-font-weight);--rio-local-text-color: var(--rio-global-text-color);--rio-local-text-background: var(--rio-global-text-background);--rio-local-text-background-clip: var(--rio-global-text-background-clip);--rio-local-text-fill-color: var(--rio-global-text-fill-color);--rio-local-text-font-weight: var(--rio-global-text-font-weight);color:var(--rio-local-fg)}.rio-switcheroo-neutral{--rio-local-bg: var(--rio-global-neutral-bg);--rio-local-bg-variant: var(--rio-global-neutral-bg-variant);--rio-local-bg-active: var(--rio-global-neutral-bg-active);--rio-local-fg: var(--rio-global-neutral-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-global-heading1-color);--rio-local-heading1-background: var(--rio-global-heading1-background);--rio-local-heading1-background-clip: var( --rio-global-heading1-background-clip );--rio-local-heading1-fill-color: var(--rio-global-heading1-fill-color);--rio-local-heading1-font-weight: var(--rio-global-heading1-font-weight);--rio-local-heading2-color: var(--rio-global-heading2-color);--rio-local-heading2-background: var(--rio-global-heading2-background);--rio-local-heading2-background-clip: var( --rio-global-heading2-background-clip );--rio-local-heading2-fill-color: var(--rio-global-heading2-fill-color);--rio-local-heading2-font-weight: var(--rio-global-heading2-font-weight);--rio-local-heading3-color: var(--rio-global-heading3-color);--rio-local-heading3-background: var(--rio-global-heading3-background);--rio-local-heading3-background-clip: var( --rio-global-heading3-background-clip );--rio-local-heading3-fill-color: var(--rio-global-heading3-fill-color);--rio-local-heading3-font-weight: var(--rio-global-heading3-font-weight);--rio-local-text-color: var(--rio-global-text-color);--rio-local-text-background: var(--rio-global-text-background);--rio-local-text-background-clip: var(--rio-global-text-background-clip);--rio-local-text-fill-color: var(--rio-global-text-fill-color);--rio-local-text-font-weight: var(--rio-global-text-font-weight);color:var(--rio-local-fg)}.rio-switcheroo-hud{--rio-local-bg: var(--rio-global-hud-bg);--rio-local-bg-variant: var(--rio-global-hud-bg-variant);--rio-local-bg-active: var(--rio-global-hud-bg-active);--rio-local-fg: var(--rio-global-hud-fg);--rio-local-level-2-bg: var(--rio-global-primary-bg);--rio-local-level-2-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-2-fg: var(--rio-global-primary-fg);--rio-local-level-3-bg: var(--rio-global-secondary-bg);--rio-local-level-3-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-3-fg: var(--rio-global-secondary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-primary{--rio-local-bg: var(--rio-global-primary-bg);--rio-local-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-bg-active: var(--rio-global-primary-bg-active);--rio-local-fg: var(--rio-global-primary-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-secondary{--rio-local-bg: var(--rio-global-secondary-bg);--rio-local-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-bg-active: var(--rio-global-secondary-bg-active);--rio-local-fg: var(--rio-global-secondary-fg);--rio-local-level-2-bg: var(--rio-global-primary-bg);--rio-local-level-2-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-2-fg: var(--rio-global-primary-fg);--rio-local-level-3-bg: var(--rio-global-secondary-bg);--rio-local-level-3-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-3-fg: var(--rio-global-secondary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-success{--rio-local-bg: var(--rio-global-success-bg);--rio-local-bg-variant: var(--rio-global-success-bg-variant);--rio-local-bg-active: var(--rio-global-success-bg-active);--rio-local-fg: var(--rio-global-success-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-warning{--rio-local-bg: var(--rio-global-warning-bg);--rio-local-bg-variant: var(--rio-global-warning-bg-variant);--rio-local-bg-active: var(--rio-global-warning-bg-active);--rio-local-fg: var(--rio-global-warning-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-danger{--rio-local-bg: var(--rio-global-danger-bg);--rio-local-bg-variant: var(--rio-global-danger-bg-variant);--rio-local-bg-active: var(--rio-global-danger-bg-active);--rio-local-fg: var(--rio-global-danger-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-disabled{--rio-local-bg: var(--rio-global-disabled-bg);--rio-local-bg-variant: var(--rio-global-disabled-bg-variant);--rio-local-bg-active: var(--rio-global-disabled-bg-active);--rio-local-fg: var(--rio-global-disabled-fg);--rio-local-level-2-bg: var(--rio-global-disabled-bg);--rio-local-level-2-bg-variant: var(--rio-global-disabled-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-disabled-bg-active);--rio-local-level-2-fg: var(--rio-global-disabled-fg);--rio-local-level-3-bg: var(--rio-global-disabled-bg);--rio-local-level-3-bg-variant: var(--rio-global-disabled-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-disabled-bg-active);--rio-local-level-3-fg: var(--rio-global-disabled-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-custom{--rio-local-bg: var(--rio-custom-local-bg);--rio-local-bg-variant: var(--rio-custom-local-bg-variant);--rio-local-bg-active: var(--rio-custom-local-bg-active);--rio-local-fg: var(--rio-custom-local-fg);--rio-local-level-2-bg: var(--rio-global-secondary-bg);--rio-local-level-2-bg-variant: var(--rio-global-secondary-bg-variant);--rio-local-level-2-bg-active: var(--rio-global-secondary-bg-active);--rio-local-level-2-fg: var(--rio-global-secondary-fg);--rio-local-level-3-bg: var(--rio-global-primary-bg);--rio-local-level-3-bg-variant: var(--rio-global-primary-bg-variant);--rio-local-level-3-bg-active: var(--rio-global-primary-bg-active);--rio-local-level-3-fg: var(--rio-global-primary-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}.rio-switcheroo-background>*,.rio-switcheroo-neutral>*,.rio-switcheroo-hud>*,.rio-switcheroo-primary>*,.rio-switcheroo-secondary>*,.rio-switcheroo-success>*,.rio-switcheroo-warning>*,.rio-switcheroo-danger>*,.rio-switcheroo-disabled>*,.rio-switcheroo-custom>*,.rio-switcheroo-bump>*{--rio-buffer-level-2-bg: var(--rio-local-level-2-bg);--rio-buffer-level-2-bg-variant: var(--rio-local-level-2-bg-variant);--rio-buffer-level-2-bg-active: var(--rio-local-level-2-bg-active);--rio-buffer-level-2-fg: var(--rio-local-level-2-fg);--rio-buffer-level-3-bg: var(--rio-local-level-3-bg);--rio-buffer-level-3-bg-variant: var(--rio-local-level-3-bg-variant);--rio-buffer-level-3-bg-active: var(--rio-local-level-3-bg-active);--rio-buffer-level-3-fg: var(--rio-local-level-3-fg)}.rio-switcheroo-bump{--rio-local-bg: var(--rio-buffer-level-2-bg);--rio-local-bg-variant: var(--rio-buffer-level-2-bg-variant);--rio-local-bg-active: var(--rio-buffer-level-2-bg-active);--rio-local-fg: var(--rio-buffer-level-2-fg);--rio-local-level-2-bg: var(--rio-buffer-level-3-bg);--rio-local-level-2-bg-variant: var(--rio-buffer-level-3-bg-variant);--rio-local-level-2-bg-active: var(--rio-buffer-level-3-bg-active);--rio-local-level-2-fg: var(--rio-buffer-level-3-fg);--rio-local-level-3-bg: var(--rio-buffer-level-2-bg);--rio-local-level-3-bg-variant: var(--rio-buffer-level-2-bg-variant);--rio-local-level-3-bg-active: var(--rio-buffer-level-2-bg-active);--rio-local-level-3-fg: var(--rio-buffer-level-2-fg);--rio-local-heading1-color: var(--rio-local-fg);--rio-local-heading1-background: "none";--rio-local-heading1-background-clip: "border-box";--rio-local-heading1-fill-color: "transparent";--rio-local-heading2-color: var(--rio-local-fg);--rio-local-heading2-background: "none";--rio-local-heading2-background-clip: "border-box";--rio-local-heading2-fill-color: "transparent";--rio-local-heading3-color: var(--rio-local-fg);--rio-local-heading3-background: "none";--rio-local-heading3-background-clip: "border-box";--rio-local-heading3-fill-color: "transparent";--rio-local-text-color: var(--rio-local-fg);--rio-local-text-background: "none";--rio-local-text-background-clip: "border-box";--rio-local-text-fill-color: "transparent";color:var(--rio-local-fg)}html[data-theme=light] pre code.hljs{display:block;overflow-x:auto;padding:1rem}html[data-theme=light] code.hljs{padding:3px 5px}html[data-theme=light] .hljs{background:#f3f3f3;color:#444}html[data-theme=light] .hljs-comment{color:#697070}html[data-theme=light] .hljs-punctuation,html[data-theme=light] .hljs-tag{color:#444a}html[data-theme=light] .hljs-tag .hljs-attr,html[data-theme=light] .hljs-tag .hljs-name{color:#444}html[data-theme=light] .hljs-attribute,html[data-theme=light] .hljs-doctag,html[data-theme=light] .hljs-keyword,html[data-theme=light] .hljs-meta .hljs-keyword,html[data-theme=light] .hljs-name,html[data-theme=light] .hljs-selector-tag{font-weight:700}html[data-theme=light] .hljs-deletion,html[data-theme=light] .hljs-number,html[data-theme=light] .hljs-quote,html[data-theme=light] .hljs-selector-class,html[data-theme=light] .hljs-selector-id,html[data-theme=light] .hljs-string,html[data-theme=light] .hljs-template-tag,html[data-theme=light] .hljs-type{color:#800}html[data-theme=light] .hljs-section,html[data-theme=light] .hljs-title{color:#800;font-weight:700}html[data-theme=light] .hljs-link,html[data-theme=light] .hljs-operator,html[data-theme=light] .hljs-regexp,html[data-theme=light] .hljs-selector-attr,html[data-theme=light] .hljs-selector-pseudo,html[data-theme=light] .hljs-symbol,html[data-theme=light] .hljs-template-variable,html[data-theme=light] .hljs-variable{color:#ab5656}html[data-theme=light] .hljs-literal{color:#695}html[data-theme=light] .hljs-addition,html[data-theme=light] .hljs-built_in,html[data-theme=light] .hljs-bullet,html[data-theme=light] .hljs-code{color:#397300}html[data-theme=light] .hljs-meta{color:#1f7199}html[data-theme=light] .hljs-meta .hljs-string{color:#38a}html[data-theme=light] .hljs-emphasis{font-style:italic}html[data-theme=light] .hljs-strong{font-weight:700}html[data-theme=dark] .hljs{color:#ddd;background:#303030}html[data-theme=dark] .hljs-keyword,html[data-theme=dark] .hljs-selector-tag,html[data-theme=dark] .hljs-literal,html[data-theme=dark] .hljs-section,html[data-theme=dark] .hljs-link{color:#fff}html[data-theme=dark] .hljs-string,html[data-theme=dark] .hljs-title,html[data-theme=dark] .hljs-name,html[data-theme=dark] .hljs-type,html[data-theme=dark] .hljs-attribute,html[data-theme=dark] .hljs-symbol,html[data-theme=dark] .hljs-bullet,html[data-theme=dark] .hljs-built_in,html[data-theme=dark] .hljs-addition,html[data-theme=dark] .hljs-variable,html[data-theme=dark] .hljs-template-tag,html[data-theme=dark] .hljs-template-variable{color:#d88}html[data-theme=dark] .hljs-comment,html[data-theme=dark] .hljs-quote,html[data-theme=dark] .hljs-deletion,html[data-theme=dark] .hljs-meta{color:#979797}html[data-theme=dark] .hljs-keyword,html[data-theme=dark] .hljs-selector-tag,html[data-theme=dark] .hljs-literal,html[data-theme=dark] .hljs-title,html[data-theme=dark] .hljs-section,html[data-theme=dark] .hljs-doctag,html[data-theme=dark] .hljs-type,html[data-theme=dark] .hljs-name,html[data-theme=dark] .hljs-strong{font-weight:700}html[data-theme=dark] .hljs-emphasis{font-style:italic}@keyframes content-loading{0%{background-position:-100rem 0}to{background-position:0 0}}.rio-content-loading{background-image:linear-gradient(to right,transparent 10%,var(--rio-local-level-2-bg) 12%,transparent 14%);background-size:100rem 5rem;animation:content-loading 3s linear infinite}@keyframes barber-pole{0%{background-position:0 0}to{background-position:3rem 0rem}}a{color:var(--rio-local-level-2-bg)}a:hover{color:var(--rio-local-level-2-bg-active)}code{font-family:var(--rio-global-monospace-font),monospace}html{background:var(--rio-global-background-bg);overflow:hidden}body{margin:0;padding:0;font-family:var(--rio-global-font, sans-serif)}input,textarea,select{font-family:inherit;font-size:1rem}.rio-component{position:absolute}.rio-fundamental-root-component{position:relative!important;width:100vw;height:100vh}.rio-dev-tools{pointer-events:auto}.rio-dev-tools-hidden:after{pointer-events:none;position:fixed;top:0;right:.1rem;bottom:0;content:"Screen too small for Dev Tools";color:var(--rio-global-neutral-fg);font-size:.8rem;writing-mode:vertical-rl;text-align:center;opacity:.5}.rio-linear-child-container{pointer-events:none;display:flex;align-items:stretch}.rio-linear-child-container>*{position:relative!important}.rio-list-view>div>*:first-child{position:relative!important}.rio-column{flex-direction:column}.rio-grid{pointer-events:none;display:grid}.rio-text{pointer-events:auto;display:flex;align-items:center;color:var(--rio-local-text-color)}.rio-text>div{flex-grow:1;overflow:hidden}.rio-rectangle{pointer-events:auto;border-style:solid;transition-property:background,stroke-color,stroke-width,border-radius,shadow-color,shadow-radius,shadow-offset;transition-timing-function:ease;background:var(--rio-rectangle-background);-webkit-backdrop-filter:var(--rio-rectangle-backdrop-filter);backdrop-filter:var(--rio-rectangle-backdrop-filter);border-color:var(--rio-rectangle-stroke_color);border-width:var(--rio-rectangle-stroke_width);border-radius:var(--rio-rectangle-corner_radius);box-shadow:var(--rio-rectangle-shadow_offset_x) var(--rio-rectangle-shadow_offset_y) var(--rio-rectangle-shadow_radius) var(--rio-rectangle-shadow_color);box-sizing:border-box}.rio-rectangle:hover{background:var(--rio-rectangle-hover-background);-webkit-backdrop-filter:var(--rio-rectangle-hover-backdrop-filter);backdrop-filter:var(--rio-rectangle-hover-backdrop-filter);border-color:var(--rio-rectangle-hover-stroke_color);border-width:var(--rio-rectangle-hover-stroke_width);border-radius:var(--rio-rectangle-hover-corner_radius);box-shadow:var(--rio-rectangle-hover-shadow_offset_x) var(--rio-rectangle-hover-shadow_offset_y) var(--rio-rectangle-hover-shadow_radius) var(--rio-rectangle-hover-shadow_color)}.rio-rectangle-ripple{overflow:hidden}.rio-text-input{cursor:text}.rio-text-input-hint-text{display:flex;align-items:end;-webkit-user-select:none;user-select:none;padding-bottom:.6rem;color:var(--rio-local-text-color);opacity:0;transition:all .13s linear}.rio-text-input-prefix-text{padding-left:.8rem;margin-right:.2rem}.rio-text-input-suffix-text{padding-right:.8rem;margin-left:.2rem}input:not(:placeholder-shown)~.rio-text-input-hint-text,.rio-input-box:focus-within>.rio-text-input-hint-text,.rio-input-box-focused>.rio-text-input-hint-text{opacity:.5}.rio-text-input.rio-input-box{padding-left:0!important;padding-right:0!important}.rio-input-box{pointer-events:auto;display:flex;flex-direction:row;align-items:stretch;padding-left:.8rem;padding-right:.8rem;box-sizing:border-box;background-color:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small) var(--rio-global-corner-radius-small) 0 0}.rio-input-box:not(.rio-disabled-input){overflow:hidden}.rio-input-box:focus-within,.rio-input-box.rio-input-box-focused{outline:none;background-color:var(--rio-local-bg-active)}.rio-input-box>input,.rio-input-box>textarea{flex-grow:1;min-width:0;background-color:transparent;color:var(--rio-local-text-color);caret-color:var(--rio-local-level-2-bg);border:none}.rio-input-box>input{height:calc(200% - 2.38rem)}.rio-input-box>textarea{margin-top:1.5rem;width:100%;resize:none;padding:0 .8rem}.rio-input-box>input:active,.rio-input-box>textarea:active{background-color:transparent}.rio-input-box>input:focus-visible,.rio-input-box>textarea:focus-visible{outline:none}.rio-input-box-label{pointer-events:none;position:absolute;left:.8rem;top:calc(50% - .5rem);font-size:1rem;color:var(--rio-local-text-color);opacity:.5;transition:all .13s linear}input:not(:placeholder-shown)~.rio-input-box-label,textarea:not(:placeholder-shown)~.rio-input-box-label,.rio-input-box:focus-within>.rio-input-box-label,.rio-input-box-focused>.rio-input-box-label{opacity:1;top:.4rem;bottom:unset;font-size:.8rem}.rio-input-box:focus-within>.rio-input-box-label,.rio-input-box-focused>.rio-input-box-label{color:var(--rio-local-level-2-bg)}.rio-input-box-plain-bar,.rio-input-box-color-bar{position:absolute;bottom:0;height:.12rem}.rio-input-box-plain-bar{background-color:var(--rio-local-text-color);left:0;right:0;opacity:.15}.rio-input-box-color-bar{background-color:var(--rio-local-level-2-bg);left:40%;right:40%;opacity:0;transition:all .2s ease-in-out}.rio-input-box:focus-within .rio-input-box-color-bar,.rio-input-box-focused .rio-input-box-color-bar{left:0;right:0;opacity:1}.rio-stack{pointer-events:none;display:inline-grid}.rio-stack>*{grid-column-start:1;grid-row-start:1}.rio-switch{display:flex}.rio-switch>*{pointer-events:auto;position:relative;width:3.18rem;height:1.54rem;margin:auto;border-radius:4.3rem;background-color:var(--rio-global-disabled-bg-variant);transition:.3s ease all;z-index:1}.rio-switch.is-on>*{background-color:var(--rio-local-level-2-bg)}.rio-switch input{position:relative;width:100%;height:100%;padding:0;margin:0;opacity:0;cursor:pointer;z-index:3}.rio-switch .knob{z-index:2;position:absolute;top:.17rem;left:.17rem;width:.86rem;height:.43rem;padding:.39rem .17rem;background-color:var(--rio-global-disabled-bg);border-radius:50%;transition:.3s ease all,left .3s cubic-bezier(.18,.89,.35,1.15)}.rio-switch input:active+.knob{width:1.98rem;border-radius:4.3rem}.rio-switch.is-on input:active+.knob{margin-left:-1.12rem}.rio-switch.is-on input+.knob{left:1.8rem;background-color:var(--rio-local-bg)}.rio-dropdown{pointer-events:auto}.rio-dropdown:not(.rio-disabled-input),.rio-dropdown:not(.rio-disabled-input)>input{cursor:pointer}.rio-dropdown-popup{position:absolute;z-index:10003;height:0;max-height:100vh;background-color:var(--rio-global-background-bg);color:var(--rio-global-text-color);border-radius:0 0 var(--rio-global-corner-radius-small) var(--rio-global-corner-radius-small);box-shadow:0 0 .8rem var(--rio-global-shadow-color);transition:height .2s ease-in-out}.rio-dropdown-popup-above{border-radius:var(--rio-global-corner-radius-small)!important}.rio-dropdown.rio-input-box>.rio-dropdown-arrow{pointer-events:none;order:2;display:flex;align-items:center}.rio-dropdown.rio-input-box>.rio-dropdown-arrow svg{width:1.3rem;height:1.3rem}.rio-dropdown-option-highlight{font-weight:700;color:var(--rio-local-level-2-bg)}.rio-dropdown-options{position:relative;display:flex;flex-direction:column;align-items:stretch;cursor:pointer}.rio-dropdown-options>div{position:relative}.rio-dropdown-options>svg{position:relative;width:4rem;height:4rem;margin:1.5rem auto;opacity:.2}.rio-dropdown-option:after{content:"";pointer-events:none;position:absolute;top:0;left:0;right:0;bottom:0;background-color:var(--rio-global-primary-bg);opacity:0;transition:opacity .1s ease-in-out}.rio-dropdown-option-highlighted:after{opacity:.2}.rio-progress-bar{pointer-events:none;overflow:hidden}.rio-progress-bar-track{position:absolute;width:100%;height:100%;background:var(--rio-local-text-color);opacity:.3}.rio-progress-bar-fill{position:absolute;height:100%;background:var(--rio-local-bg)}@keyframes rio-progress-bar-animation-indeterminate{0%{left:-20%;width:6%}50%{width:30%}to{left:120%;width:6%}}.rio-progress-bar-indeterminate .rio-progress-bar-fill{transform:translate(-50%);animation:rio-progress-bar-animation-indeterminate 1.5s ease-in-out infinite}.rio-progress-bar:not(.rio-progress-bar-indeterminate) .rio-progress-bar-fill{left:0;width:var(--rio-progress-bar-fraction);transition:width .3s ease-in-out}.rio-progress-circle{pointer-events:auto;stroke:var(--rio-local-bg);display:flex;justify-content:center;overflow:hidden}.rio-progress-circle circle{fill:none;stroke-width:3.5;color:var(--rio-local-bg)}.spinning svg{transform-origin:center;animation:rotate 2s linear infinite}.spinning .progress{stroke-dasharray:1,200;stroke-dashoffset:0;stroke-linecap:round;animation:dash 1.5s ease-in-out infinite}.rio-progress-circle:not(.spinning) .progress{stroke-dashoffset:-94.25;stroke-dasharray:var(--dasharray);transition:stroke-dasharray .5s ease}@keyframes rotate{to{transform:rotate(360deg)}}@keyframes dash{0%{stroke-dasharray:1,200;stroke-dashoffset:0}50%{stroke-dasharray:90,200;stroke-dashoffset:-35px}to{stroke-dashoffset:-125px}}.rio-button{--outer-text-color: var(--rio-local-text-color)}.rio-button>*{pointer-events:auto;position:relative;width:100%;height:100%;overflow:hidden;transition:color .1s ease-in-out,border-color .1s ease-in-out}.rio-buttonstyle-major{background-color:var(--rio-local-bg);box-shadow:0 0 0 transparent;transition:background-color .1s ease-in-out,box-shadow .2s ease-in-out}.rio-buttonstyle-major:hover:not(.rio-switcheroo-disabled){background-color:var(--rio-local-bg-active);cursor:pointer;box-shadow:0 .1rem .22rem #00000059}.rio-buttonstyle-minor:not(:hover){outline:.1rem solid var(--rio-local-bg);--rio-local-text-color: var(--rio-local-bg)}.rio-buttonstyle-minor:hover:not(.rio-switcheroo-disabled){background-color:var(--rio-local-bg);cursor:pointer}.rio-buttonstyle-plain{--rio-local-text-color: var(--outer-text-color)}.rio-buttonstyle-plain:hover:not(.rio-switcheroo-disabled){cursor:pointer;--rio-local-text-color: var(--rio-local-bg)}.rio-shape-pill{border-radius:99999px}.rio-shape-rounded{border-radius:var(--rio-global-corner-radius-small)}.rio-shape-rectangle{border-radius:0}.rio-shape-circle{border-radius:50%}.rio-revealer{display:flex;flex-direction:column;align-items:stretch;justify-content:stretch;border-radius:var(--rio-global-corner-radius-small);transition:background-color .15s ease-out;overflow:hidden}.rio-revealer-header{pointer-events:auto;cursor:pointer;display:flex;align-items:center;justify-content:space-between;color:var(--rio-local-text-color)}.rio-revealer-label{flex-grow:1}.rio-revealer-arrow{transform:rotate(90deg);transition:transform .25s ease-in-out}.rio-revealer-open .rio-revealer-arrow{transform:rotate(0)}.rio-revealer-content-outer{flex-grow:1;position:relative;overflow:hidden}.rio-revealer-content-inner{position:absolute;bottom:0;opacity:0;transform:translateY(-50%);transition:opacity .45s ease-in-out,transform .35s ease}.rio-revealer-open .rio-revealer-content-inner{opacity:1;transform:translateY(0)}.rio-revealer-content-inner>*{position:relative!important}.rio-plot{display:inline-block;display:flex;justify-content:center;align-items:center;overflow:hidden}.rio-icon{pointer-events:auto;display:flex;justify-content:center;align-items:center}.rio-icon svg{width:100%;height:100%}.rio-slider{pointer-events:auto;--rio-slider-position-transition-time: .3s}.rio-slider:not(.rio-switcheroo-disabled){cursor:pointer}.rio-slider-inner{pointer-events:none;position:absolute;left:.6rem;right:.6rem;height:.25rem;top:50%;transform:translateY(-50%)}.rio-slider-track{position:absolute;width:100%;height:100%;opacity:.3;background:var(--rio-local-text-color);border-radius:99999px}.rio-slider-fill{position:absolute;left:0;width:var(--rio-slider-fraction);height:100%;background:var(--rio-local-level-2-bg);border-radius:99999px;transition:width var(--rio-slider-position-transition-time) ease-in-out}.rio-slider-glow{position:absolute;left:var(--rio-slider-fraction);top:50%;width:1.1rem;height:1.1rem;transform:translate(-50%,-50%);border-radius:50%;background-color:var(--rio-local-level-2-bg);opacity:0%;transition:left var(--rio-slider-position-transition-time) ease-in-out,width .15s ease-in-out,height .15s ease-in-out,opacity .15s ease-in-out}.rio-slider:hover:not(.rio-switcheroo-disabled) .rio-slider-glow{width:2.8rem;height:2.8rem;opacity:20%}.rio-slider-knob{position:absolute;left:var(--rio-slider-fraction);top:50%;width:1.2rem;height:1.2rem;transform:translate(-50%,-50%);border-radius:50%;background-color:var(--rio-local-level-2-bg);box-shadow:0 .1rem .2rem var(--rio-global-shadow-color);transition:left var(--rio-slider-position-transition-time) ease-in-out,background-color .1s ease-in-out}.rio-slideshow{pointer-events:auto;overflow:hidden}.slideshow-child-container{position:relative;display:grid;width:100%;height:100%}.slideshow-child-container>div{grid-column-start:1;grid-row-start:1;width:100%;height:100%}.slideshow-child-container>div>*{grid-column-start:1;grid-row-start:1;width:100%;height:100%}.slideshow-progress{position:absolute;bottom:0;width:100%;height:.3rem;background-color:var(--rio-local-level-2-bg)}.rio-overlay{pointer-events:none;position:fixed!important;top:0!important;left:0!important;width:unset!important;height:unset!important;z-index:10000}.rio-spacer{pointer-events:none}.rio-media-player{pointer-events:auto}.rio-media-player video{pointer-events:none;width:100%;height:100%;object-fit:contain}.rio-media-player-alt-display{pointer-events:none;position:absolute;left:50%;top:50%;width:50%;height:50%;max-width:20rem;max-height:20rem;aspect-ratio:1;opacity:.5;transform:translate(-50%,-50%)}.rio-media-player-controls{position:absolute;left:0;bottom:0;right:0;background:linear-gradient(rgba(0,0,0,0),rgba(0,0,0,.6));padding-top:2.5rem;display:flex;flex-direction:column;gap:0rem;align-items:stretch;transition:opacity .4s ease-in-out}.rio-media-player-timeline{pointer-events:auto;cursor:pointer;position:relative;height:2rem;margin:0 .5rem}.rio-media-player-timeline>div{pointer-events:none;position:relative;top:50%;height:.2rem;transform:translateY(-50%);transition:height .2s ease-in-out}.rio-media-player-timeline:hover>div{height:.4rem}.rio-media-player-timeline-knob{position:absolute;width:0rem;height:0rem;left:100%;top:50%;background-color:var(--rio-global-primary-bg);border-radius:50%;transform:translate(-50%,-50%);transition:width .2s ease-in-out,height .2s ease-in-out}.rio-media-player-timeline:hover .rio-media-player-timeline-knob{width:.9rem;height:.9rem}.rio-media-player-timeline-background,.rio-media-player-timeline-loaded,.rio-media-player-timeline-hover,.rio-media-player-timeline-played{position:absolute;width:0%;height:100%;background-color:#fff;border-radius:99999px}.rio-media-player-timeline-background{width:100%;opacity:.2}.rio-media-player-timeline-loaded{opacity:.3}.rio-media-player-timeline-hover{opacity:0;transition:opacity .2s ease-in-out}.rio-media-player-timeline-played{background-color:var(--rio-global-primary-bg)}.rio-media-player-controls-row{display:flex;gap:1.2rem;align-items:center;padding:.5rem;padding-top:0}.rio-media-player-button{pointer-events:auto;cursor:pointer;width:2rem;height:2rem}.rio-media-player-button>img{width:100%;height:100%}.rio-media-player-volume{pointer-events:auto;cursor:pointer;position:relative;width:5rem;height:1.5rem}.rio-media-player-volume>div{pointer-events:none;position:relative;top:50%;height:.2rem;transform:translateY(-50%)}.rio-media-player-volume-background,.rio-media-player-volume-current{position:absolute;width:100%;height:100%;border-radius:99999px;background-color:#fff}.rio-media-player-volume-background{opacity:.2}.rio-media-player-volume-knob{position:absolute;width:.9rem;height:.9rem;left:100%;top:50%;background-color:#fff;border-radius:50%;transform:translate(-50%,-50%)}.rio-media-player-volume>div{position:relative;top:50%;height:.2rem;transform:translateY(-50%)}.rio-media-player-playtime-label{color:#fff;opacity:.6}.rio-markdown{pointer-events:auto;color:var(--rio-local-text-color)}.rio-markdown>*,.rio-markdown li>*{margin-top:0;margin-bottom:0}.rio-markdown>*+*,.rio-markdown li>*+*{margin-top:.8rem}.rio-markdown ul{padding-left:1rem;list-style-type:none}.rio-markdown ul>li:before{content:"-";font-weight:700;position:absolute;transform:translate(-.6rem,.1rem)}.rio-markdown li+li{margin-top:.2rem}.rio-markdown code{font-family:var(--rio-global-monospace-font),monospace;background:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small);padding:.1rem .3rem}.rio-markdown h1{font-family:var(--rio-global-heading1-font-name);color:var(--rio-local-heading1-color);font-size:var(--rio-global-heading1-font-size);font-style:var(--rio-global-heading1-italic);font-weight:var(--rio-global-heading1-font-weight);text-decoration:var(--rio-global-heading1-underlined);text-transform:var(--rio-global-heading1-all-caps)}.rio-markdown h1:not(:first-child){margin-top:2rem}.rio-markdown h1:not(:last-child){margin-bottom:1rem}.rio-markdown h2{font-family:var(--rio-global-heading2-font-name);color:var(--rio-local-heading2-color);font-size:var(--rio-global-heading2-font-size);font-style:var(--rio-global-heading2-italic);font-weight:var(--rio-global-heading2-font-weight);text-decoration:var(--rio-global-heading2-underlined);text-transform:var(--rio-global-heading2-all-caps);margin-top:0}.rio-markdown h2:not(:first-child){margin-top:1.5rem}.rio-markdown h2:not(:last-child){margin-bottom:.8rem}.rio-markdown h3{font-family:var(--rio-global-heading3-font-name);color:var(--rio-local-heading3-color);font-size:var(--rio-global-heading3-font-size);font-style:var(--rio-global-heading3-italic);font-weight:var(--rio-global-heading3-font-weight);text-decoration:var(--rio-global-heading3-underlined);text-transform:var(--rio-global-heading3-all-caps);margin-top:0}.rio-markdown h3:not(:first-child){margin-top:1rem}.rio-markdown h3:not(:last-child){margin-bottom:.5rem}.rio-markdown p{font-family:var(--rio-global-font);color:var(--rio-local-text-color);font-size:var(--rio-global-text-font-size);line-height:1.35em;font-style:var(--rio-global-text-italic);font-weight:var(--rio-global-text-font-weight);text-decoration:var(--rio-global-text-underlined);text-transform:var(--rio-global-text-all-caps)}.rio-code-block{pointer-events:auto;display:flex;flex-direction:column;align-items:stretch;gap:.5rem;padding:.5rem;background:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small);box-sizing:border-box}.rio-code-block-header{display:flex;flex-direction:row;align-items:center;justify-content:space-between;gap:1rem;color:var(--rio-local-text-color);font-size:.8rem}.rio-code-block-language{font-weight:700;opacity:.4}.rio-code-block-copy-button{width:1.3rem;height:1.3rem;cursor:pointer;border:none;background:none;border-radius:var(--rio-global-corner-radius-small);margin:0;padding:0;opacity:.4;transition:opacity .2s ease-in-out}.rio-code-block-copy-button:hover{color:var(--rio-local-level-2-bg);opacity:1}.rio-code-block>pre{margin:0;font-size:var(--rio-global-text-font-size);font-family:var(--rio-global-monospace-font),monospace;display:block}.rio-link{pointer-events:auto;cursor:pointer;display:block}.rio-text-link{color:var(--rio-local-level-2-bg);display:flex;align-items:center;justify-content:center}.rio-scroll-container{pointer-events:auto;scroll-behavior:smooth}.rio-scroll-target{pointer-events:auto}.rio-scroll-target>.rio-scroll-target-url-copy-button{display:none}.rio-scroll-target>.rio-scroll-target-url-copy-button>*{position:absolute;cursor:pointer}.rio-scroll-target:hover>.rio-scroll-target-url-copy-button{display:block}.rio-color-picker{pointer-events:none;display:flex;flex-direction:column;align-items:stretch}.rio-color-picker-color-square{pointer-events:auto;position:relative;min-height:6rem;cursor:crosshair;margin-bottom:.7rem;border-radius:var(--rio-global-corner-radius-small);flex-grow:1}.rio-color-picker-slider-outer{pointer-events:auto;position:relative;padding:.7rem 0}.rio-color-slider-inner{height:.9rem;cursor:crosshair;border-radius:99999px}.rio-color-picker-knob{pointer-events:none;cursor:crosshair;width:1.4rem;height:1.4rem;border-radius:50%;border:.2rem solid var(--rio-local-text-color);position:absolute;transform:translate(-50%,-50%);box-sizing:border-box;background:var(--chosen-color-opaque)}.rio-color-picker-slider-outer>.rio-color-picker-knob{top:50%}.color-slider-checkers{border-radius:99999px}.rio-color-picker-hue-bar>.rio-color-slider-inner{background:linear-gradient(to right,red,yellow,lime,aqua,blue,magenta,red)}.rio-color-picker-opacity-bar>.rio-color-slider-inner:not(.rio-checkered){position:absolute;top:.7rem;left:0;right:0;bottom:.7rem;background:linear-gradient(to right,transparent,var(--chosen-color-opaque))}.rio-color-picker-result-container{margin-top:.5rem;margin-left:auto;margin-right:auto;display:flex;align-items:center;gap:.8rem}.rio-color-picker-selected-color-circle{position:relative;width:2.5rem;height:2.5rem}.rio-color-picker-selected-color-circle>*{width:100%;height:100%;border-radius:50%;box-sizing:border-box;border:.2rem solid var(--rio-local-text-color)}.rio-color-picker-selected-color-circle>div:first-child{position:absolute;top:0;left:0;right:0;bottom:0;background:var(--chosen-color-transparent)}.rio-color-picker-selected-color-circle-color{background:var(--chosen-color-transparent)}.rio-color-picker-selected-color-label{pointer-events:auto;opacity:.5;width:5rem;color:var(--rio-local-text-color);font-size:.9rem;text-align:center;font-weight:700;background:transparent;border:none;padding:.3rem;border-radius:.5rem;transition:opacity .1s ease-in-out,color .1s ease-in-out,background-color .1s ease-in-out}.rio-color-picker-selected-color-label:focus{outline:none;opacity:1;color:var(--rio-local-level-2-bg);background:var(--rio-local-bg-variant)}.rio-checkered{--checker-color: #888;--checker-size: .9rem;background-image:linear-gradient(45deg,var(--checker-color) 25%,transparent 25%),linear-gradient(45deg,transparent 75%,var(--checker-color) 75%),linear-gradient(45deg,transparent 75%,var(--checker-color) 75%),linear-gradient(45deg,var(--checker-color) 25%,transparent 25%);background-size:var(--checker-size) var(--checker-size);background-position:0 0,0 0,calc(var(--checker-size) * -.5) calc(var(--checker-size) * -.5),calc(var(--checker-size) * .5) calc(var(--checker-size) * .5)}.rio-drawer{pointer-events:auto;overflow:hidden;display:flex;align-items:stretch}.rio-drawer-shade{pointer-events:none;position:absolute;left:0;top:0;right:0;bottom:0;transition:background-color .3s ease-in-out}.rio-drawer-anchor{pointer-events:none;flex-grow:1}.rio-drawer-content-outer{pointer-events:auto;display:flex;position:absolute;background-color:var(--rio-global-neutral-bg);box-shadow:0 0 1rem var(--rio-global-shadow-color);transition:transform .3s ease-out}.rio-drawer-content-inner{order:1}.rio-drawer-content-inner>*{position:relative!important}.rio-drawer-knob{align-self:center;margin:.5rem;border-radius:99999px;background:var(--rio-local-text-color);opacity:.15}.rio-drawer-left .rio-drawer-knob,.rio-drawer-right .rio-drawer-knob{width:.4rem;height:4rem}.rio-drawer-top .rio-drawer-knob,.rio-drawer-bottom .rio-drawer-knob{width:4rem;height:.4rem}.rio-drawer-top .rio-drawer-content-outer,.rio-drawer-bottom .rio-drawer-content-outer{flex-direction:column}.rio-drawer-left .rio-drawer-knob,.rio-drawer-top .rio-drawer-knob{order:2}.rio-drawer-right .rio-drawer-knob,.rio-drawer-bottom .rio-drawer-knob{order:0}.rio-drawer-left>.rio-drawer-content-outer{top:0;left:0;bottom:0;width:fit-content;border-radius:0 var(--rio-global-corner-radius-large) var(--rio-global-corner-radius-large) 0}.rio-drawer-right>.rio-drawer-content-outer{top:0;right:0;bottom:0;width:fit-content;border-radius:var(--rio-global-corner-radius-large) 0 0 var(--rio-global-corner-radius-large)}.rio-drawer-top>.rio-drawer-content-outer{left:0;top:0;right:0;height:fit-content;border-radius:0 0 var(--rio-global-corner-radius-large) var(--rio-global-corner-radius-large)}.rio-drawer-bottom>.rio-drawer-content-outer{left:0;bottom:0;right:0;height:fit-content;border-radius:var(--rio-global-corner-radius-large) var(--rio-global-corner-radius-large) 0 0}.rio-drawer-no-transition{transition:none!important}.rio-drawer-no-transition>*{transition:none!important}.rio-popup{z-index:10003}.rio-popup-anchor>*,.rio-popup-content>*{position:relative!important}.rio-popup-content{position:fixed;width:min-content;height:min-content;background-color:var(--rio-local-bg);border-radius:var(--rio-global-corner-radius-medium);box-shadow:0 0 1rem var(--rio-global-shadow-color);transform:scale(0);opacity:0;transition:transform .2s linear,opacity .1s ease-in-out}.rio-popup-open>.rio-popup-content{transform:scale(1);opacity:1;transition:transform .2s cubic-bezier(.5,.5,.2,1.14),opacity .1s ease-in-out}.rio-image{pointer-events:auto;display:flex;justify-content:center;align-items:center}.rio-image img{width:100%;height:100%;object-fit:contain}.rio-image svg{max-width:3rem}.rio-card{pointer-events:auto;background-color:var(--rio-local-bg);box-shadow:0 0 0 var(--rio-global-shadow-color);transition:box-shadow .15s ease-out,background-color .1s ease-out}.rio-card-elevate-on-hover:hover{box-shadow:0 .15rem .3rem var(--rio-global-shadow-color)}.rio-card-colorize-on-hover:hover{background-color:var(--rio-local-bg-active)}.rio-card-ripple{overflow:hidden}.rio-switcher-bar{display:flex;align-items:center}.rio-switcher-bar>div{position:relative}.rio-switcher-bar>div>.rio-switcher-bar-options{position:relative!important}.rio-switcher-bar-options{pointer-events:auto;position:absolute;display:flex;align-items:stretch;justify-content:space-between}.rio-switcher-bar-option{display:flex;flex-direction:column;align-items:center;justify-content:space-between;cursor:pointer;border-radius:var(--rio-global-corner-radius-large);color:var(--rio-local-text-color);transition:background-color .1s ease-out}.rio-switcher-bar-option:hover{background-color:var(--rio-local-bg-active)}.rio-switcher-bar-marker>.rio-switcher-bar-options>.rio-switcher-bar-option{background-color:unset!important}.rio-switcher-bar-option>div{margin-left:auto;margin-right:auto;white-space:nowrap}.rio-switcher-bar-marker{pointer-events:none;background:var(--rio-local-bg);overflow:hidden;position:absolute;left:0;top:0;border-radius:var(--rio-global-corner-radius-large)}.rio-table{pointer-events:auto;display:grid}.rio-table>*{padding:.5rem .8rem}.rio-table .header{display:flex;cursor:pointer}.rio-table .header:after{content:"▴";display:inline-block;margin-left:.3rem;opacity:0}.rio-table .header[data-sort=ascending]:after{content:"▴";opacity:1}.rio-table .header[data-sort=descending]:after{content:"▾";opacity:1}.rio-list-view{pointer-events:none;display:flex;flex-direction:column;align-items:stretch}.rio-heading-list-item{pointer-events:none;box-sizing:border-box}.rio-listview-grouped{pointer-events:auto;background-color:var(--rio-local-bg-variant);transition:background-color .1s ease-out}.rio-listview-grouped+.rio-listview-grouped:after{content:"";position:absolute;top:0;left:0;right:0;height:1px;background-color:var(--rio-local-text-color);opacity:.2}.rio-list-item-ripple{overflow:hidden}.rio-list-item-ripple:hover{background:var(--rio-local-bg-active)}.rio-flow-container{display:flex;flex-wrap:wrap}.rio-flow-container>*{transition:left .2s ease-out,top .2s ease-out}.rio-connection-lost-popup{pointer-events:none;position:fixed;left:0;top:0;width:100vw;height:100vh;z-index:10004;background-color:transparent;transition:background-color 1s ease-in-out}.rio-connection-lost-popup.rio-connection-lost-popup-visible{display:flex;align-items:stretch;background-color:#00000080}.rio-connection-lost-popup>*{position:absolute;flex-grow:1;left:0;top:0;width:100%;height:100%;opacity:0;transform:translateY(-5rem);transition:opacity .3s ease-in-out,transform .3s cubic-bezier(.5,.5,.2,1.14)}.rio-connection-lost-popup.rio-connection-lost-popup-visible>*{opacity:1;transform:translateY(0)}.rio-traceback{pointer-events:auto;position:relative;left:50%;top:5rem;width:fit-content;max-width:50rem;padding:2.2rem;overflow:hidden;display:flex;flex-direction:column;align-items:stretch;gap:1.5rem;border-radius:var(--rio-global-corner-radius-large);box-shadow:0 .4rem 1rem var(--rio-global-shadow-color);transform:translate(-50%)}.rio-traceback-header{display:flex;align-items:center;gap:.6rem}.rio-traceback-header>svg{width:2.5rem;height:2.5rem;fill:var(--rio-global-danger-bg)}.rio-traceback-header>div{flex-grow:1;text-align:left;font-size:1.8rem;color:var(--rio-global-danger-bg)}.rio-traceback-traceback{pointer-events:auto;font-family:var(--rio-global-monospace-font),monospace;font-size:.9rem;white-space:pre-wrap;overflow-wrap:break-word;padding:.5rem 1rem;background-color:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-small)}.rio-traceback-footer{display:flex;flex-direction:column;gap:.5rem}.rio-traceback-footer-links{display:flex;flex-direction:row;gap:.5rem;justify-content:space-between}.rio-traceback-footer>a{flex:1}.rio-traceback-bold{font-weight:700}.rio-traceback-dim{opacity:.5}.rio-traceback-red{color:var(--rio-global-danger-bg)}.rio-traceback-yellow{color:var(--rio-global-warning-bg)}.rio-dev-tools-connector{pointer-events:auto;display:flex;flex-direction:column;align-items:center;justify-content:end;gap:.1rem;z-index:2;text-decoration:none}.rio-dev-tools-connector img{width:2.5rem;height:2.5rem;object-fit:contain;margin-bottom:.25rem}.rio-dev-tools-connector div{color:var(--rio-local-text-color);transition:color 1s ease-in-out}.rio-dev-tools-connector div:last-child{margin-bottom:1rem}.rio-dev-tools-connector:hover div{color:var(--rio-global-secondary-fg);transition:color .1s ease-in-out}.rio-dev-tools-connector:before{content:"";position:absolute;top:0;right:0;bottom:0;left:0;z-index:-1;background:linear-gradient(to top,var(--rio-global-secondary-bg),transparent);opacity:0;transition:opacity 1s ease-out}.rio-dev-tools-connector:hover:before{opacity:1;transition:opacity .1s ease-out}.rio-dev-tools-component-tree{overflow-x:hidden;overflow-y:auto}.rio-dev-tools-component-tree>*{position:absolute;width:100%;height:100%}.rio-dev-tools-component-tree-item{display:flex;flex-direction:column;gap:.2rem}@keyframes flash-text{0%{color:initial}20%{color:var(--rio-global-warning-bg)}to{color:initial}}.rio-dev-tools-component-tree-flash{animation:flash-text 3s linear}.rio-dev-tools-component-tree-item-header{pointer-events:auto;cursor:pointer;z-index:1;position:relative;padding:.3rem .6rem;display:flex;flex-direction:row;align-items:center;gap:.5rem}.rio-dev-tools-component-tree-item>.rio-dev-tools-component-tree-item-header>div:first-child{width:1rem;height:1rem;transition:transform .1s ease-in-out}.rio-dev-tools-component-tree-item[data-expanded=true]>.rio-dev-tools-component-tree-item-header>div:first-child{transform:rotate(90deg)}.rio-dev-tools-component-tree-item-header:after{pointer-events:none;content:"";display:block;z-index:-1;position:absolute;left:0;top:0;right:0;bottom:0;background:var(--rio-global-secondary-bg);border-radius:99999px;opacity:0;transition:opacity .1s ease-in-out}.rio-dev-tools-component-tree-item-header>div>svg{width:1rem;height:1rem}.rio-dev-tools-component-tree-item-header-weakly-selected{font-weight:700}.rio-dev-tools-component-tree-item-header-strongly-selected{font-weight:700;color:var(--rio-global-secondary-fg)}.rio-dev-tools-component-tree-item-header:hover:after{opacity:.4}.rio-dev-tools-component-tree-item-header-weakly-selected:after{opacity:.15}.rio-dev-tools-component-tree-item-header-strongly-selected:after{opacity:.6}.rio-dev-tools-component-tree-item-header-strongly-selected:hover:after{opacity:.8}.rio-dev-tools-component-tree-item-children{margin-left:.7rem;display:none;flex-direction:column;gap:.2rem}.rio-dev-tools-component-tree-item[data-has-children=true][data-expanded=true]>.rio-dev-tools-component-tree-item-children{display:flex}.rio-dev-tools-component-highlighter{pointer-events:none;position:fixed;z-index:10001;transition:left .3s ease-in-out,top .3s ease-in-out,width .3s ease-in-out,height .3s ease-in-out}@keyframes pulse{0%{left:-.3rem;top:-.3rem;right:-.3rem;bottom:-.3rem;border-width:.4rem}50%{left:-.7rem;top:-.7rem;right:-.7rem;bottom:-.7rem;border-width:.3rem}to{left:-.3rem;top:-.3rem;right:-.3rem;bottom:-.3rem;border-width:.4rem}}.rio-dev-tools-component-highlighter:after{content:"";position:absolute;display:block;border-radius:1rem;box-shadow:0 0 0 9999rem #0009;border-style:solid;border-color:var(--rio-global-secondary-bg);animation:pulse 1.4s infinite}.rio-dev-tools-background{position:relative;background:var(--rio-local-bg)}.rio-dev-tools-background:after{pointer-events:none;content:"";position:absolute;display:block;z-index:1;left:0;top:0;bottom:0;right:0;background-image:linear-gradient(-45deg,var(--rio-local-bg) 25%,var(--rio-global-secondary-bg) 25%,var(--rio-global-secondary-bg) 50%,var(--rio-local-bg) 50%,var(--rio-local-bg) 75%,var(--rio-global-secondary-bg) 75%,var(--rio-global-secondary-bg));background-size:3rem 3rem;opacity:.03}.rio-switcher{overflow:hidden}.rio-tooltip{pointer-events:none;position:relative}.rio-tooltip-anchor{pointer-events:auto;position:relative}.rio-tooltip-anchor>*,.rio-tooltip-label>*{position:relative!important}.rio-tooltip-label{position:absolute;width:max-content;padding:.5rem;border-radius:var(--rio-global-corner-radius-small);background:var(--rio-global-hud-bg);box-shadow:0 .1rem .2rem var(--rio-global-shadow-color);opacity:0;transition:opacity .15s ease-in-out}.rio-build-failed{pointer-events:auto;color:var(--rio-global-danger-fg);display:flex;flex-direction:column;align-items:stretch;background:var(--rio-global-danger-bg);border-radius:var(--rio-global-corner-radius-small);overflow:hidden;background-image:linear-gradient(-45deg,var(--rio-global-danger-bg-variant) 15%,transparent 15%,transparent 50%,var(--rio-global-danger-bg-variant) 50%,var(--rio-global-danger-bg-variant) 65%,transparent 65%);background-size:3rem 3rem;animation:barber-pole 1s linear infinite}.rio-build-failed-top,.rio-build-failed-bottom{flex-grow:1}.rio-build-failed-top{background:linear-gradient(to top,var(--rio-global-danger-bg),var(--rio-global-danger-bg) 30%,transparent)}.rio-build-failed-bottom{background:linear-gradient(to bottom,var(--rio-global-danger-bg),var(--rio-global-danger-bg) 30%,transparent)}.rio-build-failed-content{padding:1rem;display:flex;flex-direction:column;align-items:stretch;gap:1rem;background:var(--rio-global-danger-bg)}.rio-build-failed-header{align-self:center;display:flex;align-items:center;gap:.5rem}.rio-build-failed-icon{width:2rem;height:2rem}.rio-build-failed-summary{font-weight:700}.rio-build-failed-details{align-self:center}.rio-code-explorer{pointer-events:none;display:flex;align-items:center;justify-content:space-between}.rio-code-explorer-source-code{pointer-events:auto;display:block;cursor:text;white-space:pre;font-size:1rem;font-family:var(--rio-global-monospace-font),monospace;position:relative;width:min-content;background:var(--rio-local-bg-variant);border-radius:var(--rio-global-corner-radius-medium)}.rio-code-explorer-build-result{position:relative}.rio-code-explorer-build-result>*:not(.rio-code-explorer-highlighter){position:relative!important}.rio-code-explorer-highlighter{pointer-events:none;position:absolute;opacity:0;transition:opacity .3s ease-in-out,left .3s ease-in-out,top .3s ease-in-out,width .3s ease-in-out,height .3s ease-in-out}.rio-code-explorer-highlighter:after{content:"";z-index:10001;position:absolute;border-radius:1rem;border-style:solid;border-width:.2rem!important;border-color:var(--rio-global-secondary-bg);box-shadow:0 0 4rem 1rem var(--rio-global-secondary-bg);opacity:.4;animation:pulse 1.4s infinite}.rio-separator{position:relative;background-color:var(--rio-local-bg)}.rio-separator:after{content:"";position:absolute;left:0;top:0;right:0;bottom:0;background-color:var(--separator-color);opacity:var(--separator-opacity)}.rio-ripple-effect{pointer-events:none;position:absolute;background:var(--rio-ripple-color);border-radius:50%;transform:translate(-50%,-50%);transition:top var(--rio-ripple-duration),left var(--rio-ripple-duration),width var(--rio-ripple-duration),height var(--rio-ripple-duration),opacity var(--rio-ripple-duration)}
```

### Comparing `rio_ui-0.8.5/rio/frontend files/assets/index-a8d525bb.js` & `rio_ui-0.8.6/rio/frontend files/assets/index-8ca8e5f1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13231,15 +13231,16 @@
 }
 
 function vr(t, e) {
     let n = e[t] || {},
         i = Bu(t, n),
         r = t,
         s = i._margin_;
-    if (s === void 0 && console.error(`Got incomplete state for component ${t}`), s[0] !== 0 || s[1] !== 0 || s[2] !== 0 || s[3] !== 0) {
+    if (s === void 0) console.error(`Got incomplete state for component ${t}`);
+    else if (s[0] !== 0 || s[1] !== 0 || s[2] !== 0 || s[3] !== 0) {
         let a = t * -10;
         e[a] = {
             _type_: "Margin-builtin",
             _python_type_: "Margin (injected)",
             _key_: null,
             _margin_: [0, 0, 0, 0],
             _size_: [0, 0],
@@ -13249,15 +13250,16 @@
             margin_left: s[0],
             margin_top: s[1],
             margin_right: s[2],
             margin_bottom: s[3]
         }, r = a
     }
     let o = i._align_;
-    if (o === void 0 && console.error(`Got incomplete state for component ${t}`), o[0] !== null || o[1] !== null) {
+    if (o === void 0) console.error(`Got incomplete state for component ${t}`);
+    else if (o[0] !== null || o[1] !== null) {
         let a = t * -10 - 1;
         e[a] = {
             _type_: "Align-builtin",
             _python_type_: "Align (injected)",
             _key_: null,
             _margin_: [0, 0, 0, 0],
             _size_: [0, 0],
```

### Comparing `rio_ui-0.8.5/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/README.md` & `rio_ui-0.8.6/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/__init__.py` & `rio_ui-0.8.6/rio/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/core-classes.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/core-classes.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/debugging-setup.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/debugging-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/deployment.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/deployment.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-custom-events.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-custom-events.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-install.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-install.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/persistent-settings.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/persistent-settings.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/project-setup.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/project-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/run-project.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/run-project.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/howtos/theming.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/theming.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import *  # type:ignore
 
 import pandas as pd
 
+# list of cryptocurrencies we want to display in our dashboard
+CRYPTO_LIST: list[str] = ["bitcoin", "litecoin", "ethereum"]
+
 # example data for our bar chart in the balance card component
 BAR_CHART: pd.DataFrame = pd.DataFrame([4, 5, 6, 5, 4, 6, 7], columns=["data"])
 
 
 # example data for our crypto portfolio. Our portfolio consists of three coins:
 # bitcoin, litecoin, and ethereum. Each coin has a value, a ticker, a color, and a logo.
 MY_COINS: dict[str, Tuple[float, str, str, str]] = {
```

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,24 @@
+# <additional-imports>
 import dataclasses
 from pathlib import Path
 from typing import *  # type:ignore
 
-# <additional-imports>
 import numpy as np
 import pandas as pd
 from pycoingecko import CoinGeckoAPI
 
 import rio
 
 from .. import components as comps
 from .. import data_models
 
 # </additional-imports>
 
 
-DIR = Path(__file__).parent.parent
-ASSET_DIR = DIR / "assets"
-
-CRYPTO_LIST: list[str] = ["bitcoin", "litecoin", "ethereum"]
-
-FETCH_DATA_FROM_API = True  # Set to False to use local data
-
-
 # <component>
 class DashboardPage(rio.Component):
     """
     A component for displaying our cryptocurrency dashboard.
 
     The DashboardPage class is the main component of the dashboard application,
     designed to display a user's cryptocurrency balance and the historical data
@@ -38,47 +30,48 @@
 
     ## Attributes
 
     `coin_data`: the historical data of our portfolio consisting of Bitcoin,
         Litecoin, and Ethereum.
     """
 
+    fetch_data_from_api: bool = False
     coin_data: pd.DataFrame = dataclasses.field(
         default=pd.DataFrame(
             {
                 "date": np.zeros(5),
-                **{coin: np.zeros(5) for coin in CRYPTO_LIST},
+                **{coin: np.zeros(5) for coin in data_models.CRYPTO_LIST},
             }
         )
     )
 
     @rio.event.on_populate
     async def on_populate(self) -> None:
         """
         The method fetches the historical data of our cryptocurrencies from the
         CoinGecko API or reads the data from a local CSV file, depending on the
-        value of the FETCH_DATA_FROM_API flag.
+        value of the fetch_data_from_api flag.
 
         The @rio.event.on_populate decorator triggers our on_populate method
         after the component has been created or has been reconciled. This allows
         us to asynchronously fetch any data which depends on the component's
         state.
         """
-        if FETCH_DATA_FROM_API is True:
-            self.coin_data = self._fetch_coin_data(CRYPTO_LIST)
+        if self.fetch_data_from_api is True:
+            self.coin_data = self._fetch_coin_data(data_models.CRYPTO_LIST)
         else:
-            self.coin_data = self._read_csv(ASSET_DIR / "cryptos.csv")
+            self.coin_data = self._read_csv(self.session.assets / "cryptos.csv")
 
     def _read_csv(self, path: Path) -> pd.DataFrame:
         """
         Reads a csv file from the given path and returns a pandas DataFrame.
 
         ## Parameters
 
-        `path`: A string representing the path to the csv file.
+        `path`: A Path object representing the path to the csv file.
         """
         df = pd.read_csv(path)
         df["date"] = pd.to_datetime(df["date"])
         df.set_index("date", inplace=True)
         return df
 
     def _fetch_coin_data(
@@ -171,37 +164,35 @@
             margin_right=5,
         )
 
         grid.add(
             comps.BalanceCard(data=self.coin_data),
             row=0,
             column=0,
-            width=2,
         )
 
         # you can use a loop to add the CryptoCard components for each coin
-        for i, coin in enumerate(CRYPTO_LIST):
+        for i, coin in enumerate(data_models.CRYPTO_LIST):
             grid.add(
                 comps.CryptoCard(
                     data=self.coin_data,
                     coin=coin,
                     coin_amount=data_models.MY_COINS[coin][0],
                     coin_ticker=data_models.MY_COINS[coin][1],
                     color=data_models.MY_COINS[coin][2],
                     logo_url=data_models.MY_COINS[coin][3],
                 ),
                 row=i,
-                column=4,
+                column=1,
             )
 
         grid.add(
             comps.CryptoChart(data=self.coin_data, coin="bitcoin"),
             row=1,
             column=0,
-            width=2,
             height=2,
         )
 
         return grid
 
 
 # </component>
```

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/README.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/README.md` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/scripts/benchmark.py` & `rio_ui-0.8.6/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/scripts/build_frontend.py` & `rio_ui-0.8.6/scripts/build_frontend.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/scripts/build_material_icon_set.py` & `rio_ui-0.8.6/scripts/build_material_icon_set.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/scripts/code_coverage.py` & `rio_ui-0.8.6/scripts/code_coverage.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/scripts/publish_new_release.py` & `rio_ui-0.8.6/scripts/publish_new_release.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_attribute_bindings.py` & `rio_ui-0.8.6/tests/test_attribute_bindings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_custom_components.py` & `rio_ui-0.8.6/tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_docstring_code_blocks.py` & `rio_ui-0.8.6/tests/test_docstring_code_blocks.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_documentation.py` & `rio_ui-0.8.6/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_events.py` & `rio_ui-0.8.6/tests/test_events.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
         @rio.event.on_unmount
         def _on_unmount(self):
             nonlocal unmounted
             unmounted = True
 
         def build(self) -> rio.Component:
+            return NestedComponent()
+
+    class NestedComponent(rio.Component):
+        def build(self) -> rio.Component:
             return rio.Text("hi")
 
     def build():
         return ChildToggler(DemoComponent())
 
     async with rio.testing.TestClient(build) as test_client:
         root = test_client.get_component(ChildToggler)
@@ -43,14 +47,25 @@
         assert not unmounted
 
         root.toggle()
         await test_client.refresh()
         assert mounted
         assert not unmounted
 
+        # Make sure the newly mounted components were sent to the client
+        demo_component = test_client.get_component(DemoComponent)
+        nested_component = test_client.get_component(NestedComponent)
+        text_component = test_client.get_component(rio.Text)
+        assert test_client._last_updated_components == {
+            root,
+            demo_component,
+            nested_component,
+            text_component,
+        }
+
         root.toggle()
         await test_client.refresh()
         assert unmounted
 
 
 async def test_refresh_after_synchronous_mount_handler():
     class DemoComponent(rio.Component):
```

### Comparing `rio_ui-0.8.5/tests/test_project_templates.py` & `rio_ui-0.8.6/tests/test_project_templates.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_reconciliation.py` & `rio_ui-0.8.6/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_refresh.py` & `rio_ui-0.8.6/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_session.py` & `rio_ui-0.8.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_testing_tools.py` & `rio_ui-0.8.6/tests/test_testing_tools.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_user_settings.py` & `rio_ui-0.8.6/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/test_zzz_guardrails.py` & `rio_ui-0.8.6/tests/test_zzz_guardrails.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/tests/utils.py` & `rio_ui-0.8.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/LICENSE.txt` & `rio_ui-0.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/README.md` & `rio_ui-0.8.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   <img src="https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square" alt="Version"/>
   <!--
   <img src="https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square" alt="Discord"/>
   -->
   <img src="https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square" alt="Python Version"/>
   <img src="https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square" alt="License"/>
   <img src="https://img.shields.io/github/stars/rio-labs/rio?style=flat-square" alt="GitHub Stars"/>
+  <img src="https://img.shields.io/pypi/dm/rio-ui?color=%2311e8e3e&style=flat-square" alt="Downloads"/>
 </p>
 
 ![Image Generation Example](https://github.com/rio-labs/rio/assets/41641225/44279406-0c2d-47e2-98b5-4582722054b2)
 
 ## Features 🧩
 
 - Modern, **declarative UI** framework
@@ -59,15 +60,15 @@
         return rio.Column(
             rio.Button('Click me', on_press=self._on_press),
             rio.Text(f'You clicked the button {self.clicks} time(s)'),
         )
 
 # Create an App and tell it to display a ButtonClicker when it starts
 app = rio.App(build=ButtonClicker)
-app.run_in_browser()
+app.run_in_browser()  # Or `app.run_in_window()` to run as local app!
 ```
 
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
@@ -102,13 +103,14 @@
 **Every project thrives with a helping hand**, and that's especially true for Rio. **There are lots of ways to jump in**, like adding new features, fixing bugs, or just sharing your ideas.
 Check out our [Contributing Guide](https://github.com/rio-labs/rio/blob/dev/CONTRIBUTING.md) when submitting a Pull Request to the project.
 Rio keeps getting better with new features rolling out every week. **Star ⭐ and 👀 watch this repo to stay in the loop!**
 
 ## Community Support 🫶
 
 **Join the Rio adventure and be part of an awesome fellowship! Here is how to get in touch:**
+
 - [Discord](https://discord.gg/7ejXaPwhyH) (Level up your Rio skills! **Join our Discord server** to chat with other developers and discuss how to contribute.)
 - [GitHub](https://github.com/rio-labs/rio) (**Spot a bug?** Issues are the perfect place to let us know. Feeling super-helpful? Try fixing an existing issue and submit a PR!)
 - [Community Forum](https://github.com/rio-labs/rio/discussions) (**Join our community forum on Github** for asking questions and discussions)
 - [Feature Requests](https://github.com/rio-labs/rio/discussions/categories/feature-requests) (Cleanest way to **request a feature** on GitHub)
 
 For general help using Rio, please refer to the [official Rio documentation](https://rio.dev/docs).
```

### Comparing `rio_ui-0.8.5/pyproject.toml` & `rio_ui-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.5/PKG-INFO` & `rio_ui-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.8.5
+Version: 0.8.6
 Summary: Build modern Websites and Apps just with Python
 Project-URL: homepage, https://rio.dev
 Project-URL: repository, https://github.com/rio-labs/rio
 Project-URL: documentation, https://rio.dev/docs
 Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>, Paul Pinterits <rawing7@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
@@ -274,14 +274,15 @@
   <img src="https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square" alt="Version"/>
   <!--
   <img src="https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square" alt="Discord"/>
   -->
   <img src="https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square" alt="Python Version"/>
   <img src="https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square" alt="License"/>
   <img src="https://img.shields.io/github/stars/rio-labs/rio?style=flat-square" alt="GitHub Stars"/>
+  <img src="https://img.shields.io/pypi/dm/rio-ui?color=%2311e8e3e&style=flat-square" alt="Downloads"/>
 </p>
 
 ![Image Generation Example](https://github.com/rio-labs/rio/assets/41641225/44279406-0c2d-47e2-98b5-4582722054b2)
 
 ## Features 🧩
 
 - Modern, **declarative UI** framework
@@ -314,15 +315,15 @@
         return rio.Column(
             rio.Button('Click me', on_press=self._on_press),
             rio.Text(f'You clicked the button {self.clicks} time(s)'),
         )
 
 # Create an App and tell it to display a ButtonClicker when it starts
 app = rio.App(build=ButtonClicker)
-app.run_in_browser()
+app.run_in_browser()  # Or `app.run_in_window()` to run as local app!
 ```
 
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
@@ -357,13 +358,14 @@
 **Every project thrives with a helping hand**, and that's especially true for Rio. **There are lots of ways to jump in**, like adding new features, fixing bugs, or just sharing your ideas.
 Check out our [Contributing Guide](https://github.com/rio-labs/rio/blob/dev/CONTRIBUTING.md) when submitting a Pull Request to the project.
 Rio keeps getting better with new features rolling out every week. **Star ⭐ and 👀 watch this repo to stay in the loop!**
 
 ## Community Support 🫶
 
 **Join the Rio adventure and be part of an awesome fellowship! Here is how to get in touch:**
+
 - [Discord](https://discord.gg/7ejXaPwhyH) (Level up your Rio skills! **Join our Discord server** to chat with other developers and discuss how to contribute.)
 - [GitHub](https://github.com/rio-labs/rio) (**Spot a bug?** Issues are the perfect place to let us know. Feeling super-helpful? Try fixing an existing issue and submit a PR!)
 - [Community Forum](https://github.com/rio-labs/rio/discussions) (**Join our community forum on Github** for asking questions and discussions)
 - [Feature Requests](https://github.com/rio-labs/rio/discussions/categories/feature-requests) (Cleanest way to **request a feature** on GitHub)
 
 For general help using Rio, please refer to the [official Rio documentation](https://rio.dev/docs).
```

