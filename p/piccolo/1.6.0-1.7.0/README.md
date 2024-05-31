# Comparing `tmp/piccolo-1.6.0.tar.gz` & `tmp/piccolo-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piccolo-1.6.0.tar", last modified: Thu May 30 00:16:59 2024, max compression
+gzip compressed data, was "piccolo-1.7.0.tar", last modified: Fri May 31 11:53:59 2024, max compression
```

## Comparing `piccolo-1.6.0.tar` & `piccolo-1.7.0.tar`

### file list

```diff
@@ -1,462 +1,462 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.843379 piccolo-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-30 00:16:23.000000 piccolo-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-30 00:16:59.843379 piccolo-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-30 00:16:23.000000 piccolo-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.775379 piccolo-1.6.0/piccolo/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.775379 piccolo-1.6.0/piccolo/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.775379 piccolo-1.6.0/piccolo/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/new.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/app/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/templates/tables.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.763378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_esmerald_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_lilya_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    35096 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    26266 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/backwards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/forwards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/templates/migration.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/playground/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/playground/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/project/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/schema/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/schema/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/tester/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/columns/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    81069 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/columns/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/m2m.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/columns/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/math.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/conf/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.803379 piccolo-1.6.0/piccolo/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/cockroach.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.803379 piccolo-1.6.0/piccolo/query/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.803379 piccolo-1.6.0/piccolo/query/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.807379 piccolo-1.6.0/piccolo/query/methods/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/drop_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/table_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    21982 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/querystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    49457 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/table_reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.807379 piccolo-1.6.0/piccolo/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/testing/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/testing/random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/piccolo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/piccolo/utils/graphlib/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/graphlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/graphlib/_graphlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/sql_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/piccolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 00:16:23.000000 piccolo-1.6.0/profiling/run_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-30 00:16:23.000000 piccolo-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 00:16:59.843379 piccolo-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-30 00:16:23.000000 piccolo-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/commands/test_show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/asgi/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/commands/test_dump_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/commands/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/meta/commands/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/auto/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46131 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/integration/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_forwards_backwards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/test_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/project/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/sql_shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.823379 piccolo-1.6.0/tests/columns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/columns/m2m/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/test_m2m_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_bigint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_bytea.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_db_column_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_double_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_jsonb.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_primary_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_reserved_column_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_smallint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_varchar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/conf/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/conf/test_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_extra_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_nested_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_version_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/mega/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/music/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/tables_detailed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.831379 piccolo-1.6.0/tests/query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.831379 piccolo-1.6.0/tests/query/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/mixins/test_columns_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/mixins/test_order_by_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_await.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_camelcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_querystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.835379 piccolo-1.6.0/tests/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/tests/table/instance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_get_related.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_get_related_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_all_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_create_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_create_table_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_drop_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_join_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    40390 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_table_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/testing/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/testing/test_random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26623 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_sql_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_table_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.859614 piccolo-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-31 11:53:34.000000 piccolo-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-31 11:53:59.859614 piccolo-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-31 11:53:34.000000 piccolo-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.799613 piccolo-1.7.0/piccolo/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.799613 piccolo-1.7.0/piccolo/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.803613 piccolo-1.7.0/piccolo/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.803613 piccolo-1.7.0/piccolo/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/app/commands/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/app/commands/show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.803613 piccolo-1.7.0/piccolo/apps/app/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/app/commands/templates/tables.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/app/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.803613 piccolo-1.7.0/piccolo/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.803613 piccolo-1.7.0/piccolo/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.787613 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/_esmerald_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/_lilya_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/main.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/asgi/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/fixtures/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/fixtures/commands/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/fixtures/commands/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/fixtures/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.807613 piccolo-1.7.0/piccolo/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/meta/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/meta/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35096 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26266 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/auto/serialisation_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/backwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/forwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/migrations/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/commands/templates/migration.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/migrations/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/playground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/playground/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/playground/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/playground/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/playground/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.811613 piccolo-1.7.0/piccolo/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/project/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/project/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/project/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/schema/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/schema/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/schema/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/schema/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/schema/commands/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/schema/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/schema/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/sql_shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/sql_shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/tester/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/tester/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/tester/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/tester/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.815613 piccolo-1.7.0/piccolo/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.819613 piccolo-1.7.0/piccolo/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/commands/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/commands/change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.819613 piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/apps/user/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.819613 piccolo-1.7.0/piccolo/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81685 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.819613 piccolo-1.7.0/piccolo/columns/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/defaults/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/m2m.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.823613 piccolo-1.7.0/piccolo/columns/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/operators/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/operators/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/operators/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/columns/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.823613 piccolo-1.7.0/piccolo/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/conf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.823613 piccolo-1.7.0/piccolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/engine/cockroach.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/engine/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/engine/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25033 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/engine/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.823613 piccolo-1.7.0/piccolo/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.823613 piccolo-1.7.0/piccolo/query/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/functions/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/functions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/functions/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.827613 piccolo-1.7.0/piccolo/query/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/drop_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/methods/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21982 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/query/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49457 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/table_reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.827613 piccolo-1.7.0/piccolo/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/testing/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/testing/random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/piccolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/piccolo/utils/graphlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/graphlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/graphlib/_graphlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-31 11:53:34.000000 piccolo-1.7.0/piccolo/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.855614 piccolo-1.7.0/piccolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-31 11:53:59.000000 piccolo-1.7.0/piccolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-31 11:53:59.000000 piccolo-1.7.0/piccolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:53:59.000000 piccolo-1.7.0/piccolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 11:53:59.000000 piccolo-1.7.0/piccolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 11:53:59.000000 piccolo-1.7.0/piccolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 11:53:59.000000 piccolo-1.7.0/piccolo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-31 11:53:34.000000 piccolo-1.7.0/profiling/run_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-31 11:53:34.000000 piccolo-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:53:59.859614 piccolo-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-31 11:53:34.000000 piccolo-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/app/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/app/commands/test_show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/asgi/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/fixtures/commands/test_dump_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/fixtures/commands/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/meta/commands/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.831613 piccolo-1.7.0/tests/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/migrations/auto/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46131 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/integration/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/test_diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/test_migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/test_schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/test_schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/auto/test_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/test_forwards_backwards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/migrations/commands/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/test_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/migrations/test_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/project/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.835613 piccolo-1.7.0/tests/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.839613 piccolo-1.7.0/tests/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/sql_shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.839613 piccolo-1.7.0/tests/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.839613 piccolo-1.7.0/tests/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.839613 piccolo-1.7.0/tests/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/user/commands/test_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/user/commands/test_change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/user/commands/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/user/commands/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/apps/user/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.843613 piccolo-1.7.0/tests/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.843613 piccolo-1.7.0/tests/columns/m2m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/m2m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/m2m/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/m2m/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/m2m/test_m2m_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_bytea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_db_column_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_double_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_jsonb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_primary_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_reserved_column_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_smallint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/columns/test_varchar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.843613 piccolo-1.7.0/tests/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/conf/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/conf/test_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.843613 piccolo-1.7.0/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/engine/test_extra_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/engine/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/engine/test_nested_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/engine/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/engine/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/engine/test_version_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.843613 piccolo-1.7.0/tests/example_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.847613 piccolo-1.7.0/tests/example_apps/mega/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/mega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/mega/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.847613 piccolo-1.7.0/tests/example_apps/mega/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/mega/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/mega/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.847613 piccolo-1.7.0/tests/example_apps/music/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/music/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/music/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/example_apps/music/tables_detailed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.847613 piccolo-1.7.0/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.847613 piccolo-1.7.0/tests/query/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/mixins/test_columns_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/mixins/test_order_by_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/test_camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/test_querystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/query/test_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.851614 piccolo-1.7.0/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.855614 piccolo-1.7.0/tests/table/instance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/test_get_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/test_get_related_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/test_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/instance/test_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_all_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_create_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_create_table_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_drop_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_join_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40390 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/table/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.855614 piccolo-1.7.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/testing/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/testing/test_random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:59.855614 piccolo-1.7.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26623 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_table_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 11:53:34.000000 piccolo-1.7.0/tests/utils/test_warnings.py
```

### Comparing `piccolo-1.6.0/LICENSE` & `piccolo-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/PKG-INFO` & `piccolo-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 1.6.0
+Version: 1.7.0
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
```

### Comparing `piccolo-1.6.0/README.md` & `piccolo-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/app/commands/new.py` & `piccolo-1.7.0/piccolo/apps/app/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja` & `piccolo-1.7.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/new.py` & `piccolo-1.7.0/piccolo/apps/asgi/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/main.css` & `piccolo-1.7.0/piccolo/apps/asgi/commands/templates/app/static/main.css`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/fixtures/commands/dump.py` & `piccolo-1.7.0/piccolo/apps/fixtures/commands/dump.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/fixtures/commands/load.py` & `piccolo-1.7.0/piccolo/apps/fixtures/commands/load.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/fixtures/commands/shared.py` & `piccolo-1.7.0/piccolo/apps/fixtures/commands/shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/auto/diffable_table.py` & `piccolo-1.7.0/piccolo/apps/migrations/auto/diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/auto/migration_manager.py` & `piccolo-1.7.0/piccolo/apps/migrations/auto/migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/auto/operations.py` & `piccolo-1.7.0/piccolo/apps/migrations/auto/operations.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/auto/schema_differ.py` & `piccolo-1.7.0/piccolo/apps/migrations/auto/schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/auto/schema_snapshot.py` & `piccolo-1.7.0/piccolo/apps/migrations/auto/schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation.py` & `piccolo-1.7.0/piccolo/apps/migrations/auto/serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation_legacy.py` & `piccolo-1.7.0/piccolo/apps/migrations/auto/serialisation_legacy.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/commands/backwards.py` & `piccolo-1.7.0/piccolo/apps/migrations/commands/backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/commands/base.py` & `piccolo-1.7.0/piccolo/apps/migrations/commands/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/commands/check.py` & `piccolo-1.7.0/piccolo/apps/migrations/commands/check.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/commands/clean.py` & `piccolo-1.7.0/piccolo/apps/migrations/commands/clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/commands/forwards.py` & `piccolo-1.7.0/piccolo/apps/migrations/commands/forwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/commands/new.py` & `piccolo-1.7.0/piccolo/apps/migrations/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/commands/templates/migration.py.jinja` & `piccolo-1.7.0/piccolo/apps/migrations/commands/templates/migration.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/piccolo_app.py` & `piccolo-1.7.0/piccolo/apps/migrations/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/migrations/tables.py` & `piccolo-1.7.0/piccolo/apps/migrations/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/playground/commands/run.py` & `piccolo-1.7.0/piccolo/apps/playground/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/project/commands/new.py` & `piccolo-1.7.0/piccolo/apps/project/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/schema/commands/generate.py` & `piccolo-1.7.0/piccolo/apps/schema/commands/generate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/schema/commands/graph.py` & `piccolo-1.7.0/piccolo/apps/schema/commands/graph.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja` & `piccolo-1.7.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/shell/commands/run.py` & `piccolo-1.7.0/piccolo/apps/shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/sql_shell/commands/run.py` & `piccolo-1.7.0/piccolo/apps/sql_shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/tester/commands/run.py` & `piccolo-1.7.0/piccolo/apps/tester/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/commands/change_password.py` & `piccolo-1.7.0/piccolo/apps/user/commands/change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/commands/change_permissions.py` & `piccolo-1.7.0/piccolo/apps/user/commands/change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/commands/create.py` & `piccolo-1.7.0/piccolo/apps/user/commands/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/commands/list.py` & `piccolo-1.7.0/piccolo/apps/user/commands/list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/piccolo_app.py` & `piccolo-1.7.0/piccolo/apps/user/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py` & `piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py` & `piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py` & `piccolo-1.7.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/apps/user/tables.py` & `piccolo-1.7.0/piccolo/apps/user/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/__init__.py` & `piccolo-1.7.0/piccolo/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/base.py` & `piccolo-1.7.0/piccolo/columns/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/choices.py` & `piccolo-1.7.0/piccolo/columns/choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/column_types.py` & `piccolo-1.7.0/piccolo/columns/column_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -2528,15 +2528,22 @@
 
     @property
     def column_type(self):
         engine_type = self._meta.engine_type
         if engine_type in ("postgres", "cockroach"):
             return f"{self.base_column.column_type}[]"
         elif engine_type == "sqlite":
-            return "ARRAY"
+            inner_column = self._get_inner_column()
+            return (
+                f"ARRAY_{inner_column.column_type}"
+                if isinstance(
+                    inner_column, (Date, Timestamp, Timestamptz, Time)
+                )
+                else "ARRAY"
+            )
         raise Exception("Unrecognized engine type")
 
     def _setup_base_column(self, table_class: t.Type[Table]):
         """
         Called from the ``Table.__init_subclass__`` - makes sure
         that the ``base_column`` has a reference to the parent table.
         """
@@ -2560,30 +2567,44 @@
 
         """
         if isinstance(self.base_column, Array):
             return self.base_column._get_dimensions(start=start + 1)
         else:
             return start + 1
 
+    def _get_inner_column(self) -> Column:
+        """
+        A helper function to get the innermost ``Column`` for the array. For
+        example::
+
+            >>> Array(Varchar())._get_inner_column()
+            Varchar
+
+            >>> Array(Array(Varchar()))._get_inner_column()
+            Varchar
+
+        """
+        if isinstance(self.base_column, Array):
+            return self.base_column._get_inner_column()
+        else:
+            return self.base_column
+
     def _get_inner_value_type(self) -> t.Type:
         """
         A helper function to get the innermost value type for the array. For
         example::
 
             >>> Array(Varchar())._get_inner_value_type()
             str
 
             >>> Array(Array(Varchar()))._get_inner_value_type()
             str
 
         """
-        if isinstance(self.base_column, Array):
-            return self.base_column._get_inner_value_type()
-        else:
-            return self.base_column.value_type
+        return self._get_inner_column().value_type
 
     def __getitem__(self, value: int) -> Array:
         """
         Allows queries which retrieve an item from the array. The index starts
         with 0 for the first value. If you were to write the SQL by hand, the
         first index would be 1 instead (see `Postgres array docs <https://www.postgresql.org/docs/current/arrays.html>`_).
```

### Comparing `piccolo-1.6.0/piccolo/columns/combination.py` & `piccolo-1.7.0/piccolo/columns/combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/defaults/base.py` & `piccolo-1.7.0/piccolo/columns/defaults/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/defaults/date.py` & `piccolo-1.7.0/piccolo/columns/defaults/date.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/defaults/interval.py` & `piccolo-1.7.0/piccolo/columns/defaults/interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/defaults/time.py` & `piccolo-1.7.0/piccolo/columns/defaults/time.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/defaults/timestamp.py` & `piccolo-1.7.0/piccolo/columns/defaults/timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/defaults/timestamptz.py` & `piccolo-1.7.0/piccolo/columns/defaults/timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/m2m.py` & `piccolo-1.7.0/piccolo/columns/m2m.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/operators/comparison.py` & `piccolo-1.7.0/piccolo/columns/operators/comparison.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/readable.py` & `piccolo-1.7.0/piccolo/columns/readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/columns/reference.py` & `piccolo-1.7.0/piccolo/columns/reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/conf/apps.py` & `piccolo-1.7.0/piccolo/conf/apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/custom_types.py` & `piccolo-1.7.0/piccolo/custom_types.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/engine/base.py` & `piccolo-1.7.0/piccolo/engine/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/engine/cockroach.py` & `piccolo-1.7.0/piccolo/engine/cockroach.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/engine/postgres.py` & `piccolo-1.7.0/piccolo/engine/postgres.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/engine/sqlite.py` & `piccolo-1.7.0/piccolo/engine/sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import enum
 import os
 import sqlite3
 import typing as t
 import uuid
 from dataclasses import dataclass
 from decimal import Decimal
+from functools import partial, wraps
 
 from piccolo.engine.base import Batch, Engine, validate_savepoint_name
 from piccolo.engine.exceptions import TransactionError
 from piccolo.query.base import DDL, Query
 from piccolo.querystring import QueryString
 from piccolo.utils.encoding import dump_json, load_json
 from piccolo.utils.lazy_loader import LazyLoader
@@ -31,36 +32,36 @@
 # We need to register some adapters so sqlite returns types which are more
 # consistent with the Postgres engine.
 
 
 # In
 
 
-def convert_numeric_in(value):
+def convert_numeric_in(value: Decimal) -> float:
     """
     Convert any Decimal values into floats.
     """
     return float(value)
 
 
-def convert_uuid_in(value) -> str:
+def convert_uuid_in(value: uuid.UUID) -> str:
     """
     Converts the UUID value being passed into sqlite.
     """
     return str(value)
 
 
 def convert_time_in(value: datetime.time) -> str:
     """
     Converts the time value being passed into sqlite.
     """
     return value.isoformat()
 
 
-def convert_date_in(value: datetime.date):
+def convert_date_in(value: datetime.date) -> str:
     """
     Converts the date value being passed into sqlite.
     """
     return value.isoformat()
 
 
 def convert_datetime_in(value: datetime.datetime) -> str:
@@ -70,130 +71,243 @@
     timezone aware datetimes in UTC.
     """
     if value.tzinfo is not None:
         value = value.astimezone(datetime.timezone.utc)
     return str(value)
 
 
-def convert_timedelta_in(value: datetime.timedelta):
+def convert_timedelta_in(value: datetime.timedelta) -> float:
     """
     Converts the timedelta value being passed into sqlite.
     """
     return value.total_seconds()
 
 
-def convert_array_in(value: list):
+def convert_array_in(value: list) -> str:
     """
-    Converts a list value into a string.
+    Converts a list value into a string (it handles nested lists, and type like
+    dateime/ time / date which aren't usually JSON serialisable.).
+
     """
-    if value and type(value[0]) not in [str, int, float, list]:
-        raise ValueError("Can only serialise str, int, float, and list.")
 
-    return dump_json(value)
+    def serialise(data: list):
+        output = []
+
+        for item in data:
+            if isinstance(item, list):
+                output.append(serialise(item))
+            elif isinstance(
+                item, (datetime.datetime, datetime.time, datetime.date)
+            ):
+                if adapter := ADAPTERS.get(type(item)):
+                    output.append(adapter(item))
+                else:
+                    raise ValueError("The adapter wasn't found.")
+            elif item is None or isinstance(item, (str, int, float, list)):
+                # We can safely JSON serialise these.
+                output.append(item)
+            else:
+                raise ValueError("We can't currently serialise this value.")
+
+        return output
+
+    return dump_json(serialise(value))
+
+
+###############################################################################
+
+# Register adapters
+
+ADAPTERS: t.Dict[t.Type, t.Callable[[t.Any], t.Any]] = {
+    Decimal: convert_numeric_in,
+    uuid.UUID: convert_uuid_in,
+    datetime.time: convert_time_in,
+    datetime.date: convert_date_in,
+    datetime.datetime: convert_datetime_in,
+    datetime.timedelta: convert_timedelta_in,
+    list: convert_array_in,
+}
 
+for value_type, adapter in ADAPTERS.items():
+    sqlite3.register_adapter(value_type, adapter)
+
+###############################################################################
 
 # Out
 
 
-def convert_numeric_out(value: bytes) -> Decimal:
+def decode_to_string(converter: t.Callable[[str], t.Any]):
+    """
+    This means we can use our converters with string and bytes. They are
+    passed bytes when used directly via SQLite, and are passed strings when
+    used by the array converters.
+    """
+
+    @wraps(converter)
+    def wrapper(value: t.Union[str, bytes]) -> t.Any:
+        if isinstance(value, bytes):
+            return converter(value.decode("utf8"))
+        elif isinstance(value, str):
+            return converter(value)
+        else:
+            raise ValueError("Unsupported type")
+
+    return wrapper
+
+
+@decode_to_string
+def convert_numeric_out(value: str) -> Decimal:
     """
     Convert float values into Decimals.
     """
-    return Decimal(value.decode("ascii"))
+    return Decimal(value)
 
 
-def convert_int_out(value: bytes) -> int:
+@decode_to_string
+def convert_int_out(value: str) -> int:
     """
     Make sure Integer values are actually of type int.
     """
     return int(float(value))
 
 
-def convert_uuid_out(value: bytes) -> uuid.UUID:
+@decode_to_string
+def convert_uuid_out(value: str) -> uuid.UUID:
     """
     If the value is a uuid, convert it to a UUID instance.
     """
-    return uuid.UUID(value.decode("utf8"))
+    return uuid.UUID(value)
 
 
-def convert_date_out(value: bytes) -> datetime.date:
-    return datetime.date.fromisoformat(value.decode("utf8"))
+@decode_to_string
+def convert_date_out(value: str) -> datetime.date:
+    return datetime.date.fromisoformat(value)
 
 
-def convert_time_out(value: bytes) -> datetime.time:
+@decode_to_string
+def convert_time_out(value: str) -> datetime.time:
     """
     If the value is a time, convert it to a UUID instance.
     """
-    return datetime.time.fromisoformat(value.decode("utf8"))
+    return datetime.time.fromisoformat(value)
 
 
-def convert_seconds_out(value: bytes) -> datetime.timedelta:
+@decode_to_string
+def convert_seconds_out(value: str) -> datetime.timedelta:
     """
     If the value is from a seconds column, convert it to a timedelta instance.
     """
-    return datetime.timedelta(seconds=float(value.decode("utf8")))
+    return datetime.timedelta(seconds=float(value))
 
 
-def convert_boolean_out(value: bytes) -> bool:
+@decode_to_string
+def convert_boolean_out(value: str) -> bool:
     """
     If the value is from a boolean column, convert it to a bool value.
     """
-    _value = value.decode("utf8")
-    return _value == "1"
+    return value == "1"
 
 
-def convert_timestamp_out(value: bytes) -> datetime.datetime:
+@decode_to_string
+def convert_timestamp_out(value: str) -> datetime.datetime:
     """
     If the value is from a timestamp column, convert it to a datetime value.
     """
-    return datetime.datetime.fromisoformat(value.decode("utf8"))
+    return datetime.datetime.fromisoformat(value)
 
 
-def convert_timestamptz_out(value: bytes) -> datetime.datetime:
+@decode_to_string
+def convert_timestamptz_out(value: str) -> datetime.datetime:
     """
     If the value is from a timestamptz column, convert it to a datetime value,
     with a timezone of UTC.
     """
-    _value = datetime.datetime.fromisoformat(value.decode("utf8"))
-    _value = _value.replace(tzinfo=datetime.timezone.utc)
-    return _value
+    return datetime.datetime.fromisoformat(value).replace(
+        tzinfo=datetime.timezone.utc
+    )
 
 
-def convert_array_out(value: bytes) -> t.List:
+@decode_to_string
+def convert_array_out(value: str) -> t.List:
     """
     If the value if from an array column, deserialise the string back into a
     list.
     """
-    return load_json(value.decode("utf8"))
+    return load_json(value)
 
 
-def convert_M2M_out(value: bytes) -> t.List:
-    _value = value.decode("utf8")
-    return _value.split(",")
-
-
-sqlite3.register_converter("Numeric", convert_numeric_out)
-sqlite3.register_converter("Integer", convert_int_out)
-sqlite3.register_converter("UUID", convert_uuid_out)
-sqlite3.register_converter("Date", convert_date_out)
-sqlite3.register_converter("Time", convert_time_out)
-sqlite3.register_converter("Seconds", convert_seconds_out)
-sqlite3.register_converter("Boolean", convert_boolean_out)
-sqlite3.register_converter("Timestamp", convert_timestamp_out)
-sqlite3.register_converter("Timestamptz", convert_timestamptz_out)
-sqlite3.register_converter("Array", convert_array_out)
-sqlite3.register_converter("M2M", convert_M2M_out)
-
-sqlite3.register_adapter(Decimal, convert_numeric_in)
-sqlite3.register_adapter(uuid.UUID, convert_uuid_in)
-sqlite3.register_adapter(datetime.time, convert_time_in)
-sqlite3.register_adapter(datetime.date, convert_date_in)
-sqlite3.register_adapter(datetime.datetime, convert_datetime_in)
-sqlite3.register_adapter(datetime.timedelta, convert_timedelta_in)
-sqlite3.register_adapter(list, convert_array_in)
+def convert_complex_array_out(value: bytes, converter: t.Callable):
+    """
+    This is used to handle arrays of things like timestamps, which we can't
+    just load from JSON without doing additional work to convert the elements
+    back into Python objects.
+    """
+    parsed = load_json(value.decode("utf8"))
+
+    def convert_list(list_value: t.List):
+        output = []
+
+        for value in list_value:
+            if isinstance(value, list):
+                # For nested arrays
+                output.append(convert_list(value))
+            elif isinstance(value, str):
+                output.append(converter(value))
+            else:
+                output.append(value)
+
+        return output
+
+    if isinstance(parsed, list):
+        return convert_list(parsed)
+    else:
+        return parsed
+
+
+@decode_to_string
+def convert_M2M_out(value: str) -> t.List:
+    return value.split(",")
+
+
+###############################################################################
+# Register the basic converters
+
+CONVERTERS = {
+    "NUMERIC": convert_numeric_out,
+    "INTEGER": convert_int_out,
+    "UUID": convert_uuid_out,
+    "DATE": convert_date_out,
+    "TIME": convert_time_out,
+    "SECONDS": convert_seconds_out,
+    "BOOLEAN": convert_boolean_out,
+    "TIMESTAMP": convert_timestamp_out,
+    "TIMESTAMPTZ": convert_timestamptz_out,
+    "M2M": convert_M2M_out,
+}
+
+for column_name, converter in CONVERTERS.items():
+    sqlite3.register_converter(column_name, converter)
+
+###############################################################################
+# Register the array converters
+
+# The ARRAY column type handles values which can be easily serialised to and
+# from JSON.
+sqlite3.register_converter("ARRAY", convert_array_out)
+
+# We have special column types for arrays of timestamps etc, as simply loading
+# the JSON isn't sufficient.
+for column_name in ("TIMESTAMP", "TIMESTAMPTZ", "DATE", "TIME"):
+    sqlite3.register_converter(
+        f"ARRAY_{column_name}",
+        partial(
+            convert_complex_array_out,
+            converter=CONVERTERS[column_name],
+        ),
+    )
 
 ###############################################################################
 
 
 @dataclass
 class AsyncBatch(Batch):
     connection: Connection
```

### Comparing `piccolo-1.6.0/piccolo/main.py` & `piccolo-1.7.0/piccolo/main.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/__init__.py` & `piccolo-1.7.0/piccolo/query/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/base.py` & `piccolo-1.7.0/piccolo/query/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/functions/aggregate.py` & `piccolo-1.7.0/piccolo/query/functions/aggregate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/functions/string.py` & `piccolo-1.7.0/piccolo/query/functions/string.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/__init__.py` & `piccolo-1.7.0/piccolo/query/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/alter.py` & `piccolo-1.7.0/piccolo/query/methods/alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/count.py` & `piccolo-1.7.0/piccolo/query/methods/count.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/create.py` & `piccolo-1.7.0/piccolo/query/methods/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/create_index.py` & `piccolo-1.7.0/piccolo/query/methods/create_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/delete.py` & `piccolo-1.7.0/piccolo/query/methods/delete.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/drop_index.py` & `piccolo-1.7.0/piccolo/query/methods/drop_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/exists.py` & `piccolo-1.7.0/piccolo/query/methods/exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/indexes.py` & `piccolo-1.7.0/piccolo/query/methods/indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/insert.py` & `piccolo-1.7.0/piccolo/query/methods/insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/objects.py` & `piccolo-1.7.0/piccolo/query/methods/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/raw.py` & `piccolo-1.7.0/piccolo/query/methods/raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/refresh.py` & `piccolo-1.7.0/piccolo/query/methods/refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/select.py` & `piccolo-1.7.0/piccolo/query/methods/select.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/table_exists.py` & `piccolo-1.7.0/piccolo/query/methods/table_exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/methods/update.py` & `piccolo-1.7.0/piccolo/query/methods/update.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/mixins.py` & `piccolo-1.7.0/piccolo/query/mixins.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/query/proxy.py` & `piccolo-1.7.0/piccolo/query/proxy.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/querystring.py` & `piccolo-1.7.0/piccolo/querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/schema.py` & `piccolo-1.7.0/piccolo/schema.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/table.py` & `piccolo-1.7.0/piccolo/table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/table_reflection.py` & `piccolo-1.7.0/piccolo/table_reflection.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/testing/model_builder.py` & `piccolo-1.7.0/piccolo/testing/model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/testing/random_builder.py` & `piccolo-1.7.0/piccolo/testing/random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/dictionary.py` & `piccolo-1.7.0/piccolo/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/encoding.py` & `piccolo-1.7.0/piccolo/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/graphlib/_graphlib.py` & `piccolo-1.7.0/piccolo/utils/graphlib/_graphlib.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/lazy_loader.py` & `piccolo-1.7.0/piccolo/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/list.py` & `piccolo-1.7.0/piccolo/utils/list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/objects.py` & `piccolo-1.7.0/piccolo/utils/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/printing.py` & `piccolo-1.7.0/piccolo/utils/printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/pydantic.py` & `piccolo-1.7.0/piccolo/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/repr.py` & `piccolo-1.7.0/piccolo/utils/repr.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/sql_values.py` & `piccolo-1.7.0/piccolo/utils/sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/sync.py` & `piccolo-1.7.0/piccolo/utils/sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo/utils/warnings.py` & `piccolo-1.7.0/piccolo/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/piccolo.egg-info/PKG-INFO` & `piccolo-1.7.0/piccolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 1.6.0
+Version: 1.7.0
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
```

### Comparing `piccolo-1.6.0/piccolo.egg-info/SOURCES.txt` & `piccolo-1.7.0/piccolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/profiling/run_profile.py` & `piccolo-1.7.0/profiling/run_profile.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/pyproject.toml` & `piccolo-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/setup.py` & `piccolo-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/app/commands/test_new.py` & `piccolo-1.7.0/tests/apps/app/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/app/commands/test_show_all.py` & `piccolo-1.7.0/tests/apps/app/commands/test_show_all.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/asgi/commands/test_new.py` & `piccolo-1.7.0/tests/apps/asgi/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/fixtures/commands/test_dump_load.py` & `piccolo-1.7.0/tests/apps/fixtures/commands/test_dump_load.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/fixtures/commands/test_shared.py` & `piccolo-1.7.0/tests/apps/fixtures/commands/test_shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/auto/integration/test_migrations.py` & `piccolo-1.7.0/tests/apps/migrations/auto/integration/test_migrations.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/auto/test_diffable_table.py` & `piccolo-1.7.0/tests/apps/migrations/auto/test_diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/auto/test_migration_manager.py` & `piccolo-1.7.0/tests/apps/migrations/auto/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/auto/test_schema_differ.py` & `piccolo-1.7.0/tests/apps/migrations/auto/test_schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/auto/test_schema_snapshot.py` & `piccolo-1.7.0/tests/apps/migrations/auto/test_schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/auto/test_serialisation.py` & `piccolo-1.7.0/tests/apps/migrations/auto/test_serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/commands/test_base.py` & `piccolo-1.7.0/tests/apps/migrations/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/commands/test_check.py` & `piccolo-1.7.0/tests/apps/migrations/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/commands/test_clean.py` & `piccolo-1.7.0/tests/apps/migrations/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/commands/test_forwards_backwards.py` & `piccolo-1.7.0/tests/apps/migrations/commands/test_forwards_backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py` & `piccolo-1.7.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/migrations/commands/test_new.py` & `piccolo-1.7.0/tests/apps/migrations/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/shell/commands/test_run.py` & `piccolo-1.7.0/tests/apps/shell/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/user/commands/test_change_password.py` & `piccolo-1.7.0/tests/apps/user/commands/test_change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/user/commands/test_change_permissions.py` & `piccolo-1.7.0/tests/apps/user/commands/test_change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/user/commands/test_create.py` & `piccolo-1.7.0/tests/apps/user/commands/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/user/commands/test_list.py` & `piccolo-1.7.0/tests/apps/user/commands/test_list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/apps/user/test_tables.py` & `piccolo-1.7.0/tests/apps/user/test_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/m2m/base.py` & `piccolo-1.7.0/tests/columns/m2m/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/m2m/test_m2m.py` & `piccolo-1.7.0/tests/columns/m2m/test_m2m.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_base.py` & `piccolo-1.7.0/tests/columns/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_bigint.py` & `piccolo-1.7.0/tests/columns/test_bigint.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_boolean.py` & `piccolo-1.7.0/tests/columns/test_boolean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_bytea.py` & `piccolo-1.7.0/tests/columns/test_bytea.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_choices.py` & `piccolo-1.7.0/tests/columns/test_choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_combination.py` & `piccolo-1.7.0/tests/columns/test_combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_date.py` & `piccolo-1.7.0/tests/columns/test_date.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_db_column_name.py` & `piccolo-1.7.0/tests/columns/test_db_column_name.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_defaults.py` & `piccolo-1.7.0/tests/columns/test_defaults.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_double_precision.py` & `piccolo-1.7.0/tests/columns/test_double_precision.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_interval.py` & `piccolo-1.7.0/tests/columns/test_interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_json.py` & `piccolo-1.7.0/tests/columns/test_json.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_jsonb.py` & `piccolo-1.7.0/tests/columns/test_jsonb.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_numeric.py` & `piccolo-1.7.0/tests/columns/test_numeric.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_primary_key.py` & `piccolo-1.7.0/tests/columns/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_readable.py` & `piccolo-1.7.0/tests/columns/test_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_real.py` & `piccolo-1.7.0/tests/columns/test_real.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_reference.py` & `piccolo-1.7.0/tests/columns/test_reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_reserved_column_names.py` & `piccolo-1.7.0/tests/columns/test_reserved_column_names.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_smallint.py` & `piccolo-1.7.0/tests/columns/test_smallint.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_time.py` & `piccolo-1.7.0/tests/columns/test_time.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_timestamp.py` & `piccolo-1.7.0/tests/columns/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_timestamptz.py` & `piccolo-1.7.0/tests/columns/test_timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/columns/test_varchar.py` & `piccolo-1.7.0/tests/columns/test_varchar.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/conf/test_apps.py` & `piccolo-1.7.0/tests/conf/test_apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/engine/test_extra_nodes.py` & `piccolo-1.7.0/tests/engine/test_extra_nodes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/engine/test_logging.py` & `piccolo-1.7.0/tests/engine/test_logging.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/engine/test_nested_transaction.py` & `piccolo-1.7.0/tests/engine/test_nested_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/engine/test_pool.py` & `piccolo-1.7.0/tests/engine/test_pool.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/engine/test_transaction.py` & `piccolo-1.7.0/tests/engine/test_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/engine/test_version_parsing.py` & `piccolo-1.7.0/tests/engine/test_version_parsing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py` & `piccolo-1.7.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/example_apps/mega/tables.py` & `piccolo-1.7.0/tests/example_apps/mega/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/example_apps/music/tables.py` & `piccolo-1.7.0/tests/example_apps/music/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/example_apps/music/tables_detailed.py` & `piccolo-1.7.0/tests/example_apps/music/tables_detailed.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/query/mixins/test_columns_delegate.py` & `piccolo-1.7.0/tests/query/mixins/test_columns_delegate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/query/test_camelcase.py` & `piccolo-1.7.0/tests/query/test_camelcase.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/query/test_freeze.py` & `piccolo-1.7.0/tests/query/test_freeze.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/query/test_functions.py` & `piccolo-1.7.0/tests/query/test_functions.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/query/test_gather.py` & `piccolo-1.7.0/tests/query/test_gather.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/query/test_querystring.py` & `piccolo-1.7.0/tests/query/test_querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/query/test_slots.py` & `piccolo-1.7.0/tests/query/test_slots.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/instance/test_create.py` & `piccolo-1.7.0/tests/table/instance/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/instance/test_get_related.py` & `piccolo-1.7.0/tests/table/instance/test_get_related.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/instance/test_get_related_readable.py` & `piccolo-1.7.0/tests/table/instance/test_get_related_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/instance/test_instantiate.py` & `piccolo-1.7.0/tests/table/instance/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/instance/test_remove.py` & `piccolo-1.7.0/tests/table/instance/test_remove.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/instance/test_save.py` & `piccolo-1.7.0/tests/table/instance/test_save.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/instance/test_to_dict.py` & `piccolo-1.7.0/tests/table/instance/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_all_columns.py` & `piccolo-1.7.0/tests/table/test_all_columns.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_alter.py` & `piccolo-1.7.0/tests/table/test_alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_batch.py` & `piccolo-1.7.0/tests/table/test_batch.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_callback.py` & `piccolo-1.7.0/tests/table/test_callback.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_constructor.py` & `piccolo-1.7.0/tests/table/test_constructor.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_count.py` & `piccolo-1.7.0/tests/table/test_count.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_create.py` & `piccolo-1.7.0/tests/table/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_create_db_tables.py` & `piccolo-1.7.0/tests/table/test_create_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_create_table_class.py` & `piccolo-1.7.0/tests/table/test_create_table_class.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_delete.py` & `piccolo-1.7.0/tests/table/test_delete.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_drop_db_tables.py` & `piccolo-1.7.0/tests/table/test_drop_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_from_dict.py` & `piccolo-1.7.0/tests/table/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_indexes.py` & `piccolo-1.7.0/tests/table/test_indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_inheritance.py` & `piccolo-1.7.0/tests/table/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_insert.py` & `piccolo-1.7.0/tests/table/test_insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_join.py` & `piccolo-1.7.0/tests/table/test_join.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_join_on.py` & `piccolo-1.7.0/tests/table/test_join_on.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_metaclass.py` & `piccolo-1.7.0/tests/table/test_metaclass.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_objects.py` & `piccolo-1.7.0/tests/table/test_objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_output.py` & `piccolo-1.7.0/tests/table/test_output.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_raw.py` & `piccolo-1.7.0/tests/table/test_raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_refresh.py` & `piccolo-1.7.0/tests/table/test_refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_select.py` & `piccolo-1.7.0/tests/table/test_select.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_str.py` & `piccolo-1.7.0/tests/table/test_str.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_table_exists.py` & `piccolo-1.7.0/tests/table/test_table_exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/table/test_update.py` & `piccolo-1.7.0/tests/table/test_update.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/test_schema.py` & `piccolo-1.7.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/testing/test_model_builder.py` & `piccolo-1.7.0/tests/testing/test_model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/testing/test_random_builder.py` & `piccolo-1.7.0/tests/testing/test_random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_dictionary.py` & `piccolo-1.7.0/tests/utils/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_lazy_loader.py` & `piccolo-1.7.0/tests/utils/test_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_list.py` & `piccolo-1.7.0/tests/utils/test_list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_naming.py` & `piccolo-1.7.0/tests/utils/test_naming.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_printing.py` & `piccolo-1.7.0/tests/utils/test_printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_pydantic.py` & `piccolo-1.7.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_sql_values.py` & `piccolo-1.7.0/tests/utils/test_sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_sync.py` & `piccolo-1.7.0/tests/utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.6.0/tests/utils/test_table_reflection.py` & `piccolo-1.7.0/tests/utils/test_table_reflection.py`

 * *Files identical despite different names*

