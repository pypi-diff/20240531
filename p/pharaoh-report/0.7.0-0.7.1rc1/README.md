# Comparing `tmp/pharaoh_report-0.7.0.tar.gz` & `tmp/pharaoh_report-0.7.1rc1.tar.gz`

## Comparing `pharaoh_report-0.7.0.tar` & `pharaoh_report-0.7.1rc1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/__main__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/api.py
--rw-r--r--   0        0        0    12260 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/cli.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/errors.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/log.py
--rw-r--r--   0        0        0    45028 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/project.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/sphinx_app.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/version.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/__init__.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/api.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/context.py
--rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/finder.py
--rw-r--r--   0        0        0    15818 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/generation.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/matlab_engine.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/resource.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/util.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/.gitignore
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/__init__.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_bokeh.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_holoviews.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_matplotlib.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_pandas.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_panel.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_plotly.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/bokeh_embed.html
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/api.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/contextvar.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/plugin_manager.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/spec.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/__init__.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/default_settings.yaml
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/plugin.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/error.rst.jinja2
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/iframe.rst.jinja2
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/image.rst.jinja2
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/include_wrapper.rst.jinja2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/markdown.rst.jinja2
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/raw_html.rst.jinja2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/raw_rst.rst.jinja2
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/raw_txt.rst.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/default_context.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/index.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/asset_scripts/default_assets.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/debug.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/index.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-archive.cmd
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-build.cmd
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-generate-assets.cmd
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh.cmd.jinja2
--rw-r--r--   0        0        0    12674 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/footer.html
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/user_templates/placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/__init__.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/find.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/render.py
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/scaffolder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/__init__.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/env_filters.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/env_globals.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/env_tests.py
--rw-r--r--   0        0        0    16068 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/template_env.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/__init__.py
--rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_ext.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/contextlib_chdir.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/json_encoder.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/mergedeep.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/oc_resolvers.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/README.md
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/__main__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/api.py
+-rw-r--r--   0        0        0    12260 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/cli.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/errors.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/log.py
+-rw-r--r--   0        0        0    45005 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/project.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/sphinx_app.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/version.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/__init__.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/api.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/context.py
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/finder.py
+-rw-r--r--   0        0        0    15818 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/generation.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/matlab_engine.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/resource.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/util.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/.gitignore
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/__init__.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_bokeh.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_holoviews.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_matplotlib.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_pandas.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_panel.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_plotly.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/bokeh_embed.html
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/api.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/contextvar.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/plugin_manager.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/spec.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/__init__.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/default_settings.yaml
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/plugin.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/error.rst.jinja2
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/iframe.rst.jinja2
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/image.rst.jinja2
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/include_wrapper.rst.jinja2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/markdown.rst.jinja2
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/raw_html.rst.jinja2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/raw_rst.rst.jinja2
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/raw_txt.rst.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/empty/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/empty/default_context.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/empty/index.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/empty/asset_scripts/default_assets.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/debug.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/index.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-archive.cmd
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-build.cmd
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-generate-assets.cmd
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh.cmd.jinja2
+-rw-r--r--   0        0        0    12674 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/footer.html
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/user_templates/placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/first_level/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/first_level/find.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/first_level/render.py
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/first_level/scaffolder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/__init__.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/env_filters.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/env_globals.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/env_tests.py
+-rw-r--r--   0        0        0    16068 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/template_env.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/sphinx_ext/__init__.py
+-rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/sphinx_ext/asset_ext.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/util/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/util/contextlib_chdir.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/util/json_encoder.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/util/mergedeep.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/src/pharaoh/util/oc_resolvers.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/LICENSE.txt
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/README.md
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 pharaoh_report-0.7.1rc1/PKG-INFO
```

### Comparing `pharaoh_report-0.7.0/pharaoh/cli.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/cli.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/log.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/log.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/project.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         ret = omegaconf.OmegaConf.to_container(merged_settings, resolve=resolve) if to_container else merged_settings
         try:
             paths = key.split(".")
             for path in paths:
                 ret = ret[path]
 
             return ret
-        except omegaconf.errors.ConfigKeyError:
+        except KeyError:
             if default is DEFAULT_MISSING:
                 msg = f"No setting key called {key!r}!"
                 raise LookupError(msg) from None
             return default
 
     def save_settings(self, include_env: bool = False):
         """
```

### Comparing `pharaoh_report-0.7.0/pharaoh/sphinx_app.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/sphinx_app.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/api.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/api.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/context.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/context.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/finder.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/finder.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/generation.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/generation.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/matlab_engine.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/matlab_engine.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/resource.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/resource.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/util.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/util.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/__init__.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_bokeh.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_bokeh.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_holoviews.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_holoviews.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_matplotlib.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_matplotlib.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_pandas.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_pandas.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_panel.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_panel.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_plotly.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/_plotly.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/assetlib/patches/bokeh_embed.html` & `pharaoh_report-0.7.1rc1/src/pharaoh/assetlib/patches/bokeh_embed.html`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/contextvar.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/contextvar.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/plugin_manager.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/spec.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/spec.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/template.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/template.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/default_settings.yaml` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/plugin.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html` & `pharaoh_report-0.7.1rc1/src/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/first_level/find.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/first_level/find.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/first_level/render.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/first_level/render.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/first_level/scaffolder.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/first_level/scaffolder.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/second_level/env_filters.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/env_filters.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/second_level/env_globals.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/env_globals.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/second_level/template_env.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/template_env.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/second_level/util.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/util.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_ext.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/sphinx_ext/asset_ext.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+import pharaoh
 from pharaoh.templating.second_level.template_env import PharaohTemplateEnv
 
 if TYPE_CHECKING:
     from pharaoh.sphinx_app import PharaohSphinx
 
 
 def setup(app: PharaohSphinx):
@@ -16,7 +17,13 @@
     app.add_config_value("pharaoh_jinja_globals", None, "env")
 
     app.pharaoh_te = PharaohTemplateEnv()
     app.connect("config-inited", app.pharaoh_te.sphinx_config_inited_hook)
     app.connect("builder-inited", app.pharaoh_te.sphinx_builder_inited_hook)
     app.connect("source-read", app.pharaoh_te.sphinx_source_read_hook)
     app.connect("include-read", app.pharaoh_te.sphinx_include_read_hook)
+
+    return {
+        "parallel_read_safe": True,
+        "parallel_write_safe": True,
+        "version": pharaoh.__version__,
+    }
```

### Comparing `pharaoh_report-0.7.0/pharaoh/util/contextlib_chdir.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/util/contextlib_chdir.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/util/json_encoder.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/util/json_encoder.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/util/mergedeep.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/util/mergedeep.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pharaoh/util/oc_resolvers.py` & `pharaoh_report-0.7.1rc1/src/pharaoh/util/oc_resolvers.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/LICENSE.txt` & `pharaoh_report-0.7.1rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/README.md` & `pharaoh_report-0.7.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.7.0/pyproject.toml` & `pharaoh_report-0.7.1rc1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [build-system]
+# See https://pypi.org/project/hatchling/
+requires = ["hatchling", "hatch-vcs>=0.3"]
 build-backend = "hatchling.build"
-requires = [
-    "hatch-vcs>=0.3",
-    "hatchling>=1.18",
-]
+
 
 [project]
 name = "pharaoh-report"
 dynamic = ["version"]
 description = """Pharaoh is a Sphinx-based Python framework
 for generating reports in various formats by combining the
 power of configurable Jinja templates and Python scripts
@@ -46,15 +45,15 @@
 dependencies = [
     "attrs",
     "click", # CLI
     "omegaconf", # yaml R/W
     "natsort", # sorting paths naturally
     "pyyaml!=5.3.0",
     "pluggy",
-    "nbconvert", # used to programmatically execute asset notebooks",
+    "nbconvert", # used to programmatically execute asset notebooks,
     "mistletoe", # Markdown to HTML
     # Sphinx, theme & extensions
     "sphinx >=7.2.5, <8.0",
     "sphinxcontrib-jquery",
     "sphinx-design",
     "sphinx-rtd-theme",
     #    "sphinx-toolbox",
@@ -99,75 +98,123 @@
 docs = [
     "sphinx<8",
     "sphinx-rtd-theme",
     "sphinx-design",
     "sphinxcontrib-jquery",
     "sphinx-jinja",
     "sphinx-copybutton",
-    "numpy<2.0",
 ]
 dev = [
-    "tox",
-    "gitpython",
-    "setuptools_scm",
     "pytest",
     "pytest-sugar",
     "pytest-cov",
     "pytest-mock",
     "pytest-timeout",
     "pytest-xdist",
     "pytest-randomly",
-    "diff-cover>=7.7",
-    "pharaoh-report[all-plotting]",
+    "mypy",
+    "pharaoh-report[all-plotting,docs]",
 ]
 
 [project.scripts]
 pharaoh = "pharaoh.cli:cli"
 
 [tool.hatch]
 build.dev-mode-dirs = ["src"]
-build.targets.sdist.packages = ["src/pharaoh"]
+build.targets.sdist.packages = ["src"]
 build.targets.wheel.packages = ["src/pharaoh"]
 build.hooks.vcs.version-file = "src/pharaoh/version.py"
 version.source = "vcs"
 
+# https://hatch.pypa.io/latest/config/environment/overview/
+[tool.hatch.envs.default]
+installer = "uv"
+python = "3.11"  # Specifies the Python version for the default development environment
+features = ["dev"]
+
+[tool.hatch.envs.default.env-vars]
+
+[tool.hatch.envs.default.scripts]
+# Runs all tests
+test = [
+    "bash -c 'mkdir -p .tmp'",
+    "pytest --basetemp=.tmp/pytest --timeout=120 -n={env:PYTEST_XDIST_AUTO_NUM_WORKERS:auto} {args}",
+]
+
+# Runs all tests including coverage and junit xml output
+cov = [
+    "bash -c 'mkdir -p .tmp'",
+    """pytest \
+        --basetemp=.tmp/pytest \
+        {args: \
+        --junitxml .tmp/junit.{env_name}.xml \
+        --cov \
+        --cov-context test \
+        --cov-config pyproject.toml \
+        --cov-report term-missing:skip-covered \
+        --cov-report html:.tmp/htmlcov \
+        --cov-report xml:.tmp/coverage.{env_name}.xml \
+        --no-cov-on-fail \
+        --timeout=120 \
+        -n={env:PYTEST_XDIST_AUTO_NUM_WORKERS:auto} \
+    }""",
+]
+
+# Installs the current package in editable mode.
+# This script may be used to quickly install missing entry points or dependencies
+# that are not tracked by Hatch.
+dev = [
+    "hatch build",
+    "{env:HATCH_UV} pip install -e .",
+]
 
-[tool.pytest.ini_options]
-# timeout = 30
-python_files = ["test_*.py"]
-python_classes = ["Test*"]
-python_functions = ["test_*"]
-addopts = "--tb=auto -ra --showlocals -vv"
-testpaths = [
-    "tests/unit",
-    "tests/integration",
+# Cleans files that are ignored by Git
+clean = [
+    "git clean -ffX .tmp",  # Temporary files from testing
+    "git clean -fX .coverage*",
+    "git clean -fX dist",  # Built documentation and distributions (wheels etc)
+    "git clean -fX src/*/version.py",
 ]
 
-[tool.coverage.run]
-branch = true
-parallel = true
+# Builds documentation with upcoming changelog and runs link checks
+docs = [
+    "hatch build",
+    "python docs/cli/generate_cli_command_docs.py",
+    "sphinx-build -E -W -b html docs dist/docs",
+    "- sphinx-build -b linkcheck docs dist/docs",
+]
 
-[tool.coverage.html]
-directory = "dist/coverage"
+# Runs mypy
+type = "hatch run ci:mypy --install-types --non-interactive src {args}"
 
-[tool.coverage.report]
-show_missing = true
-# fail_under = 90
-precision = 2
-exclude_lines = [
-    "pragma: no cover",
-    "pragma: nocover",
-    "def __repr__",
-    "def __str__",
-    "if self.debug:",
-    "if settings.DEBUG",
-    "raise AssertionError",
+# Runs ruff without auto-fixes
+style = "ruff check {args:.}"
+
+# Runs pre-commit (includes ruff with auto-fixes and other stuff) on all files
+fix = [
+    "pre-commit install",
+    "pre-commit run {args:--all-files}",
 ]
 
 
+[tool.hatch.envs.all]
+dev-mode = false  # for matrix tests we want the packages to be installed non-editable
+
+# https://hatch.pypa.io/latest/config/environment/advanced/#matrix
+[[tool.hatch.envs.all.matrix]]
+python = ["3.9", "3.10", "3.11", "3.12"]
+
+# An environment for CI only to speed up env creation for certain jobs
+[tool.hatch.envs.ci]
+skip-install = true
+
+
+########
+# Ruff #
+########
 [tool.ruff]
 # https://docs.astral.sh/ruff/settings
 target-version = "py39"
 line-length = 120
 fix = false  # Allow autofix for all enabled rules (when `--fix`) is provided.
 show-fixes = true
 unsafe-fixes = true
@@ -195,39 +242,91 @@
     "PLC",  # Pylint - conventions
     "RUF",  # Ruff-specific rules
 ]
 ignore = [
     "PLW2901",  # Pylint - warnings: redefined-loop-name
     "E501", # https://docs.astral.sh/ruff/faq/#is-the-ruff-linter-compatible-with-black
 ]
-exclude = []
-
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+exclude = [
+    "tests/templates/*"
+]
 
 [tool.ruff.lint.isort]
 known-first-party = ["pharaoh", "test"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "api.py" = ["F401"]
 
 [tool.ruff.lint.flake8-tidy-imports]
-# Whether to ban all relative imports ("all"),
-# or only those imports that extend into the parent module or beyond ("parents").
 ban-relative-imports = "parents"
 
 
+############
+# Coverage #
+############
+# https://coverage.readthedocs.io/en/latest/config.html#
+[tool.coverage.run]
+source_pkgs = ["pharaoh"]
+branch = true
+parallel = true
+relative_files = true
+
+[tool.coverage.paths]
+ifx_pharaoh = ["src/pharaoh", "*site-packages/pharaoh"]
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    "pragma: nocover",
+    "def __repr__",
+    "def __str__",
+    "raise AssertionError",
+    "no cov",
+    "if __name__ == \"__main__\":",
+    "if TYPE_CHECKING:",
+]
+
+
+##########
+# PyTest #
+##########
+# https://docs.pytest.org/en/stable/reference/customize.html#pyproject-toml
+[tool.pytest.ini_options]
+# timeout = 30
+python_files = ["test_*.py"]
+python_classes = ["Test*"]
+python_functions = ["test_*"]
+addopts = "--tb=auto -ra --showlocals -vv"
+testpaths = [
+    "tests/unit",
+    "tests/integration",
+]
+
+
+########
+# MYPY #
+########
+# https://justincaustin.com/blog/mypy-tips-and-tricks/
 [tool.mypy]
-python_version = "3.11"
-show_error_codes = true
+# disallow_any_generics = true
+# disallow_incomplete_defs = true
+# disallow_untyped_calls = true
+# disallow_untyped_decorators = true
+# disallow_untyped_defs = true
+follow_imports = "normal"
 ignore_missing_imports = true
-allow_untyped_defs = true
-allow_incomplete_defs = true
-allow_untyped_calls = true
+no_implicit_reexport = true
+show_error_codes = true
+show_error_context = true
+strict_equality = true
+strict_optional = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unused_ignores = true
 disable_error_code = [
     "import-untyped",
     "no-redef",
     "union-attr",
     "attr-defined",
 ]
```

### Comparing `pharaoh_report-0.7.0/PKG-INFO` & `pharaoh_report-0.7.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pharaoh-report
-Version: 0.7.0
+Version: 0.7.1rc1
 Summary: Pharaoh is a Sphinx-based Python framework for generating reports in various formats by combining the power of configurable Jinja templates and Python scripts for asset generation.
 Project-URL: Documentation, https://infineon.github.io/pharaoh-dev/
 Project-URL: Homepage, https://infineon.github.io/pharaoh-dev/
 Project-URL: Release Notes, https://infineon.github.io/pharaoh-dev/changelog.html
 Project-URL: Source, https://github.com/Infineon/pharaoh-dev
 Project-URL: Tracker, https://github.com/Infineon/pharaoh-dev/issues
 Author: Johannes Loibl
@@ -56,37 +56,39 @@
 Provides-Extra: bokeh
 Requires-Dist: bokeh<3.3.0,>=3.0.0; (python_version >= '3.9') and extra == 'bokeh'
 Requires-Dist: bokeh<3.3.0,>=3.1.0; (python_version >= '3.11') and extra == 'bokeh'
 Requires-Dist: selenium>=4.11; extra == 'bokeh'
 Provides-Extra: dev
 Requires-Dist: bokeh<3.3.0,>=3.0.0; (python_version >= '3.9') and extra == 'dev'
 Requires-Dist: bokeh<3.3.0,>=3.1.0; (python_version >= '3.11') and extra == 'dev'
-Requires-Dist: diff-cover>=7.7; extra == 'dev'
-Requires-Dist: gitpython; extra == 'dev'
 Requires-Dist: holoviews; extra == 'dev'
 Requires-Dist: holoviews>=1.16; (python_version >= '3.11') and extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: jupyter-contrib-nbextensions; extra == 'dev'
 Requires-Dist: kaleido; (platform_system == 'Linux') and extra == 'dev'
 Requires-Dist: kaleido==0.1.0.post1; (platform_system == 'Windows') and extra == 'dev'
 Requires-Dist: matplotlib; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pandas>=1.5; extra == 'dev'
 Requires-Dist: plotly; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest-randomly; extra == 'dev'
 Requires-Dist: pytest-sugar; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
 Requires-Dist: selenium>=4.11; extra == 'dev'
-Requires-Dist: setuptools-scm; extra == 'dev'
-Requires-Dist: tox; extra == 'dev'
+Requires-Dist: sphinx-copybutton; extra == 'dev'
+Requires-Dist: sphinx-design; extra == 'dev'
+Requires-Dist: sphinx-jinja; extra == 'dev'
+Requires-Dist: sphinx-rtd-theme; extra == 'dev'
+Requires-Dist: sphinx<8; extra == 'dev'
+Requires-Dist: sphinxcontrib-jquery; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: numpy<2.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Requires-Dist: sphinx-jinja; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Requires-Dist: sphinx<8; extra == 'docs'
 Requires-Dist: sphinxcontrib-jquery; extra == 'docs'
 Provides-Extra: holoviews
```

