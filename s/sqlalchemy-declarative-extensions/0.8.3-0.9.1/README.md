# Comparing `tmp/sqlalchemy-declarative-extensions-0.8.3.tar.gz` & `tmp/sqlalchemy-declarative-extensions-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-declarative-extensions-0.8.3.tar", max compression
+gzip compressed data, was "sqlalchemy-declarative-extensions-0.9.1.tar", max compression
```

## Comparing `sqlalchemy-declarative-extensions-0.8.3.tar` & `sqlalchemy-declarative-extensions-0.9.1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0      191 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/LICENSE
--rw-r--r--   0        0        0    11624 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/README.md
--rw-r--r--   0        0        0     3348 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     1350 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/__init__.py
--rw-r--r--   0        0        0      129 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/__init__.py
--rw-r--r--   0        0        0     1054 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/base.py
--rw-r--r--   0        0        0     1338 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/function.py
--rw-r--r--   0        0        0     1916 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/grant.py
--rw-r--r--   0        0        0     1894 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/role.py
--rw-r--r--   0        0        0     2102 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/row.py
--rw-r--r--   0        0        0     1551 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/schema.py
--rw-r--r--   0        0        0     1480 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/trigger.py
--rw-r--r--   0        0        0     1510 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/view.py
--rw-r--r--   0        0        0     8347 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/api.py
--rw-r--r--   0        0        0     8191 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/audit.py
--rw-r--r--   0        0        0      770 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/__init__.py
--rw-r--r--   0        0        0      775 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/from_string.py
--rw-r--r--   0        0        0        0 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/mysql/__init__.py
--rw-r--r--   0        0        0      716 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py
--rw-r--r--   0        0        0      853 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py
--rw-r--r--   0        0        0     1104 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py
--rw-r--r--   0        0        0     4503 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py
--rw-r--r--   0        0        0     1403 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py
--rw-r--r--   0        0        0    11857 2024-05-13 22:19:02.807083 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py
--rw-r--r--   0        0        0     5557 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py
--rw-r--r--   0        0        0     5944 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py
--rw-r--r--   0        0        0     8148 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py
--rw-r--r--   0        0        0     7384 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py
--rw-r--r--   0        0        0     4941 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py
--rw-r--r--   0        0        0     2801 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/query.py
--rw-r--r--   0        0        0        0 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/snowflake/__init__.py
--rw-r--r--   0        0        0      868 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py
--rw-r--r--   0        0        0        0 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/__init__.py
--rw-r--r--   0        0        0     1321 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py
--rw-r--r--   0        0        0      483 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py
--rw-r--r--   0        0        0      189 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/function/__init__.py
--rw-r--r--   0        0        0     3079 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/function/base.py
--rw-r--r--   0        0        0     3071 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/function/compare.py
--rw-r--r--   0        0        0      529 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/function/ddl.py
--rw-r--r--   0        0        0       93 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/grant/__init__.py
--rw-r--r--   0        0        0     2308 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/grant/base.py
--rw-r--r--   0        0        0     4488 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/grant/compare.py
--rw-r--r--   0        0        0      643 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/grant/ddl.py
--rw-r--r--   0        0        0        0 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/py.typed
--rw-r--r--   0        0        0       91 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/__init__.py
--rw-r--r--   0        0        0     1092 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/base.py
--rw-r--r--   0        0        0     3861 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/compare.py
--rw-r--r--   0        0        0      707 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/ddl.py
--rw-r--r--   0        0        0     1088 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/generic.py
--rw-r--r--   0        0        0     2615 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/topological_sort.py
--rw-r--r--   0        0        0      196 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/row/__init__.py
--rw-r--r--   0        0        0     2973 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/row/base.py
--rw-r--r--   0        0        0    10595 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/row/compare.py
--rw-r--r--   0        0        0      471 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/row/query.py
--rw-r--r--   0        0        0      194 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/schema/__init__.py
--rw-r--r--   0        0        0     1691 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/schema/base.py
--rw-r--r--   0        0        0     1649 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/schema/compare.py
--rw-r--r--   0        0        0      568 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/schema/ddl.py
--rw-r--r--   0        0        0      528 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/sql.py
--rw-r--r--   0        0        0     2712 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/sqlalchemy.py
--rw-r--r--   0        0        0      182 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/trigger/__init__.py
--rw-r--r--   0        0        0     2176 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/trigger/base.py
--rw-r--r--   0        0        0     2334 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/trigger/compare.py
--rw-r--r--   0        0        0      541 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/trigger/ddl.py
--rw-r--r--   0        0        0      103 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/typing.py
--rw-r--r--   0        0        0      215 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/view/__init__.py
--rw-r--r--   0        0        0    17066 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/view/base.py
--rw-r--r--   0        0        0     3378 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/view/compare.py
--rw-r--r--   0        0        0      580 2024-05-13 22:19:02.811082 sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/view/ddl.py
--rw-r--r--   0        0        0    13506 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.8.3/setup.py
--rw-r--r--   0        0        0    12693 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      191 2024-05-31 13:12:32.685033 sqlalchemy-declarative-extensions-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2024-05-31 13:12:32.685033 sqlalchemy-declarative-extensions-0.9.1/LICENSE
+-rw-r--r--   0        0        0    11624 2024-05-31 13:12:32.685033 sqlalchemy-declarative-extensions-0.9.1/README.md
+-rw-r--r--   0        0        0     3348 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1350 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/__init__.py
+-rw-r--r--   0        0        0      129 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/__init__.py
+-rw-r--r--   0        0        0     1054 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/base.py
+-rw-r--r--   0        0        0     1338 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/function.py
+-rw-r--r--   0        0        0     1916 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/grant.py
+-rw-r--r--   0        0        0     1295 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/role.py
+-rw-r--r--   0        0        0     2102 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/row.py
+-rw-r--r--   0        0        0     1551 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/schema.py
+-rw-r--r--   0        0        0     1480 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/trigger.py
+-rw-r--r--   0        0        0     1510 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/view.py
+-rw-r--r--   0        0        0     8347 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/api.py
+-rw-r--r--   0        0        0     8191 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/audit.py
+-rw-r--r--   0        0        0      808 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/__init__.py
+-rw-r--r--   0        0        0      775 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/from_string.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/mysql/__init__.py
+-rw-r--r--   0        0        0      716 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py
+-rw-r--r--   0        0        0      853 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py
+-rw-r--r--   0        0        0     1336 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py
+-rw-r--r--   0        0        0     4503 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py
+-rw-r--r--   0        0        0     2410 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py
+-rw-r--r--   0        0        0    11857 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py
+-rw-r--r--   0        0        0     5557 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py
+-rw-r--r--   0        0        0     6244 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py
+-rw-r--r--   0        0        0     8316 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py
+-rw-r--r--   0        0        0     7464 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py
+-rw-r--r--   0        0        0     4941 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py
+-rw-r--r--   0        0        0     4049 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/view.py
+-rw-r--r--   0        0        0     2963 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/query.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/snowflake/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/__init__.py
+-rw-r--r--   0        0        0     1321 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py
+-rw-r--r--   0        0        0      483 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py
+-rw-r--r--   0        0        0      189 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/function/__init__.py
+-rw-r--r--   0        0        0     2959 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/function/base.py
+-rw-r--r--   0        0        0     3071 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/function/compare.py
+-rw-r--r--   0        0        0      529 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/function/ddl.py
+-rw-r--r--   0        0        0       93 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/grant/__init__.py
+-rw-r--r--   0        0        0     2308 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/grant/base.py
+-rw-r--r--   0        0        0     4488 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/grant/compare.py
+-rw-r--r--   0        0        0      643 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/grant/ddl.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/py.typed
+-rw-r--r--   0        0        0       91 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/__init__.py
+-rw-r--r--   0        0        0     1092 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/base.py
+-rw-r--r--   0        0        0     3917 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/compare.py
+-rw-r--r--   0        0        0      707 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/ddl.py
+-rw-r--r--   0        0        0     1922 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/generic.py
+-rw-r--r--   0        0        0     2644 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/topological_sort.py
+-rw-r--r--   0        0        0      196 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/row/__init__.py
+-rw-r--r--   0        0        0     2973 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/row/base.py
+-rw-r--r--   0        0        0    10595 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/row/compare.py
+-rw-r--r--   0        0        0      471 2024-05-31 13:12:32.689033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/row/query.py
+-rw-r--r--   0        0        0      194 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/schema/__init__.py
+-rw-r--r--   0        0        0     1691 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/schema/base.py
+-rw-r--r--   0        0        0     1649 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/schema/compare.py
+-rw-r--r--   0        0        0      568 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/schema/ddl.py
+-rw-r--r--   0        0        0      528 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/sql.py
+-rw-r--r--   0        0        0     2788 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/sqlalchemy.py
+-rw-r--r--   0        0        0      182 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/trigger/__init__.py
+-rw-r--r--   0        0        0     2176 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/trigger/base.py
+-rw-r--r--   0        0        0     2334 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/trigger/compare.py
+-rw-r--r--   0        0        0      541 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/trigger/ddl.py
+-rw-r--r--   0        0        0      103 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/typing.py
+-rw-r--r--   0        0        0      215 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/view/__init__.py
+-rw-r--r--   0        0        0    17502 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/view/base.py
+-rw-r--r--   0        0        0     3577 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/view/compare.py
+-rw-r--r--   0        0        0      580 2024-05-31 13:12:32.693033 sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/view/ddl.py
+-rw-r--r--   0        0        0    13506 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.9.1/setup.py
+-rw-r--r--   0        0        0    12693 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.9.1/PKG-INFO
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/LICENSE` & `sqlalchemy-declarative-extensions-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/README.md` & `sqlalchemy-declarative-extensions-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/pyproject.toml` & `sqlalchemy-declarative-extensions-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-declarative-extensions"
-version = "0.8.3"
+version = "0.9.1"
 authors = ["Dan Cardin <ddcardin@gmail.com>"]
 
 description = "Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic."
 license = "Apache-2.0"
 repository = "https://github.com/dancardin/sqlalchemy-declarative-extensions"
 readme = 'README.md'
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/__init__.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/function.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/function.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/grant.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/grant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/row.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/row.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/schema.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/trigger.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/trigger.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/alembic/view.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/alembic/view.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/api.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/api.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/audit.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/audit.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/__init__.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,29 +9,31 @@
     get_grants,
     get_objects,
     get_role_cls,
     get_roles,
     get_schemas,
     get_triggers,
     get_view,
+    get_view_cls,
     get_views,
 )
 
 __all__ = [
     "check_schema_exists",
     "check_table_exists",
     "get_current_schema",
     "get_default_grants",
     "get_function_cls",
+    "get_functions",
     "get_grants",
     "get_objects",
     "get_role_cls",
     "get_roles",
     "get_schemas",
     "get_triggers",
     "get_view",
+    "get_view_cls",
     "get_views",
-    "get_functions",
     "mysql",
     "postgresql",
     "sqlite",
 ]
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/from_string.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/from_string.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,31 +17,39 @@
 from sqlalchemy_declarative_extensions.dialects.postgresql.role import Role
 from sqlalchemy_declarative_extensions.dialects.postgresql.trigger import (
     Trigger,
     TriggerEvents,
     TriggerForEach,
     TriggerTimes,
 )
+from sqlalchemy_declarative_extensions.dialects.postgresql.view import (
+    MaterializedOptions,
+    View,
+)
+from sqlalchemy_declarative_extensions.view.base import ViewIndex
 
 __all__ = [
     "DefaultGrant",
     "DefaultGrant",
     "DefaultGrantStatement",
     "DefaultGrantStatement",
     "DefaultGrantTypes",
     "Function",
     "FunctionGrants",
     "Grant",
     "Grant",
     "GrantStatement",
     "GrantStatement",
     "GrantTypes",
+    "MaterializedOptions",
     "Role",
     "SchemaGrants",
     "SequenceGrants",
     "TableGrants",
     "Trigger",
     "TriggerEvents",
     "TriggerForEach",
     "TriggerTimes",
     "TypeGrants",
+    "View",
+    "ViewIndex",
 ]
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 from typing import Container, List, cast
 
 from sqlalchemy import Index, UniqueConstraint
 from sqlalchemy.engine import Connection
 
+from sqlalchemy_declarative_extensions.dialects.postgresql import View, ViewIndex
 from sqlalchemy_declarative_extensions.dialects.postgresql.acl import (
     parse_acl,
     parse_default_acl,
 )
-from sqlalchemy_declarative_extensions.dialects.postgresql.function import Function
+from sqlalchemy_declarative_extensions.dialects.postgresql.function import (
+    Function,
+    FunctionSecurity,
+)
 from sqlalchemy_declarative_extensions.dialects.postgresql.role import Role
 from sqlalchemy_declarative_extensions.dialects.postgresql.schema import (
     default_acl_query,
     functions_query,
     object_acl_query,
     objects_query,
     roles_query,
@@ -25,16 +29,18 @@
 )
 from sqlalchemy_declarative_extensions.dialects.postgresql.trigger import (
     Trigger,
     TriggerEvents,
     TriggerForEach,
     TriggerTimes,
 )
+from sqlalchemy_declarative_extensions.dialects.postgresql.view import (
+    MaterializedOptions,
+)
 from sqlalchemy_declarative_extensions.sql import qualify_name
-from sqlalchemy_declarative_extensions.view.base import View, ViewIndex
 
 
 def get_schemas_postgresql(connection: Connection):
     from sqlalchemy_declarative_extensions.schema.base import Schema
 
     return {
         Schema(schema) for schema, *_ in connection.execute(schemas_query).fetchall()
@@ -132,15 +138,15 @@
             )
             for raw in connection.dialect.get_indexes(connection, v.name, schema=schema)
         ]
         view = View(
             v.name,
             v.definition,
             schema=schema,
-            materialized=v.materialized,
+            materialized=MaterializedOptions() if v.materialized else False,
             constraints=indexes or None,
         )
         views.append(view)
     return views
 
 
 def get_view_postgresql(connection: Connection, name: str, schema: str = "public"):
@@ -158,14 +164,17 @@
     for f in connection.execute(functions_query).fetchall():
         function = Function(
             name=f.name,
             definition=f.source,
             returns=f.return_type,
             language=f.language,
             schema=f.schema if f.schema != "public" else None,
+            security=FunctionSecurity.definer
+            if f.security_definer
+            else FunctionSecurity.invoker,
         )
         functions.append(function)
     return functions
 
 
 def get_triggers_postgresql(connection: Connection):
     triggers = []
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,20 @@
             valid_until=r.rolvaliduntil,
             in_roles=sorted(r.memberof) if r.memberof else None,
         )
 
     @classmethod
     def from_unknown_role(cls, r: generic.Role | Role) -> Role:
         if not isinstance(r, Role):
-            return Role(r.name, in_roles=sorted(r.in_roles) if r.in_roles else None)
+            return Role(
+                r.name,
+                in_roles=sorted(r.in_roles, key=generic.by_name)
+                if r.in_roles
+                else None,
+            )
 
         return r
 
     @property
     def options(self):
         for f in fields(self):
             if f.name == "name":
@@ -77,29 +82,29 @@
             yield f.name, value
 
     def __repr__(self):
         cls_name = self.__class__.__name__
         options = ", ".join([f"{key}={value!r}" for key, value in self.options])
         return f'{cls_name}("{self.name}", {options})'
 
-    def to_sql_create(self) -> str:
+    def to_sql_create(self) -> list[str]:
         segments = ["CREATE ROLE", self.name]
 
         options = postgres_render_role_options(self)
         if options:
             segments.append("WITH")
         segments.extend(options)
 
         if self.in_roles is not None:
-            in_roles = ", ".join(self.in_roles)
+            in_roles = ", ".join(generic.role_names(self.in_roles))
             segment = f"IN ROLE {in_roles}"
             segments.append(segment)
 
         command = " ".join(segments)
-        return command + ";"
+        return [command + ";"]
 
     def to_sql_update(self, to_role: Role) -> list[str]:
         role_name = to_role.name
         diff = RoleDiff.diff(self, to_role)
 
         result = []
 
@@ -191,16 +196,16 @@
             createrole=createrole,
             inherit=inherit,
             login=login,
             replication=replication,
             bypass_rls=bypass_rls,
             connection_limit=connection_limit,
             valid_until=valid_until,
-            add_roles=add_roles,
-            remove_roles=remove_roles,
+            add_roles=generic.role_names(add_roles),
+            remove_roles=generic.role_names(remove_roles),
         )
 
 
 def conditional_option(option, condition):
     if not condition:
         return f"NO{option}"
     return option
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "pg_proc",
     column("oid"),
     column("proname"),
     column("prosrc"),
     column("pronamespace"),
     column("prolang"),
     column("prorettype"),
+    column("prosecdef"),
 )
 
 pg_language = table(
     "pg_language",
     column("oid"),
     column("lanname"),
 )
@@ -254,14 +255,15 @@
 functions_query = (
     select(
         pg_proc.c.proname.label("name"),
         pg_namespace.c.nspname.label("schema"),
         pg_language.c.lanname.label("language"),
         pg_type.c.typname.label("return_type"),
         pg_proc.c.prosrc.label("source"),
+        pg_proc.c.prosecdef.label("security_definer"),
     )
     .select_from(
         pg_proc.join(pg_namespace, pg_proc.c.pronamespace == pg_namespace.c.oid)
         .join(pg_language, pg_proc.c.prolang == pg_language.c.oid)
         .join(pg_type, pg_proc.c.prorettype == pg_type.c.oid)
     )
     .where(pg_namespace.c.nspname.notin_(["pg_catalog", "information_schema"]))
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/query.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 )
 from sqlalchemy_declarative_extensions.dialects.sqlite.query import (
     check_schema_exists_sqlite,
     get_schemas_sqlite,
     get_views_sqlite,
 )
 from sqlalchemy_declarative_extensions.sqlalchemy import dialect_dispatch, select
+from sqlalchemy_declarative_extensions.view import View
 
 get_schemas = dialect_dispatch(
     postgresql=get_schemas_postgresql,
     sqlite=get_schemas_sqlite,
     snowflake=get_schemas_snowflake,
 )
 
@@ -70,14 +71,19 @@
 
 get_views = dialect_dispatch(
     postgresql=get_views_postgresql,
     sqlite=get_views_sqlite,
     mysql=get_views_mysql,
 )
 
+get_view_cls = dialect_dispatch(
+    postgresql=lambda _: postgresql.View,
+    default=lambda _: View,
+)
+
 get_view = dialect_dispatch(
     postgresql=get_view_postgresql,
 )
 
 get_functions = dialect_dispatch(
     postgresql=get_functions_postgresql,
 )
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/function/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/function/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,36 +27,31 @@
     def qualified_name(self):
         return qualify_name(self.schema, self.name)
 
     def normalize(self) -> Function:
         raise NotImplementedError()  # pragma: no cover
 
     def to_sql_create(self, replace=False):
-        components = ["CREATE"]
-
-        if replace:
-            components.append("OR REPLACE")
-
-        components.append("FUNCTION")
-        components.append(self.qualified_name + "()")
-
-        if self.returns:
-            components.append(f"RETURNS {self.returns}")
-
-        components.append(f"LANGUAGE {self.language}")
-        components.append(f"AS $${self.definition}$$")
-
-        return " ".join(components) + ";"
+        raise NotImplementedError()
 
     def to_sql_update(self):
         return self.to_sql_create(replace=True)
 
     def to_sql_drop(self):
         return f"DROP FUNCTION {self.qualified_name}();"
 
+    def with_name(self, name: str):
+        return replace(self, name=name)
+
+    def with_language(self, language: str):
+        return replace(self, language=language)
+
+    def with_return_type(self, return_type: str):
+        return replace(self, returns=return_type)
+
 
 @dataclass
 class Functions:
     """The collection of functions and associated options comparisons.
 
     Note: `ignore` option accepts a sequence of strings. Each string is individually
         interpreted as a "glob". This means a string like "foo.*" would ignore all views
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/function/compare.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/function/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/function/ddl.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/function/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/grant/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/grant/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/grant/compare.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/grant/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/grant/ddl.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/grant/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/compare.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,65 +67,66 @@
         op = cls(Role(role_name))
         return operations.invoke(op)
 
     def reverse(self):
         return CreateRoleOp(self.role)
 
     def to_sql(self):
-        return self.role.to_sql_drop()
+        return [self.role.to_sql_drop()]
 
 
 Operation = Union[CreateRoleOp, UpdateRoleOp, DropRoleOp]
 
 
 def compare_roles(connection: Connection, roles: Roles) -> list[Operation]:
     result: list[Operation] = []
     if not roles:
         return result
 
-    roles_by_name = {r.name: r for r in roles.roles}
+    roles_by_name = {r.name: r for r in roles.roles if not r.external}
     expected_role_names = set(roles_by_name)
 
     existing_roles = get_roles(connection)
     existing_roles_by_name = {r.name: r for r in existing_roles}
     existing_role_names = set(existing_roles_by_name)
 
     new_role_names = expected_role_names - existing_role_names
     removed_role_names = existing_role_names - expected_role_names
 
     role_cls = get_role_cls(connection)
 
     for role in topological_sort(roles.roles):
         role_name = role.name
 
-        if role_name in roles.ignore_roles:
+        if role_name in roles.ignore_roles or role.external:
             continue
 
         role_created = role_name in new_role_names
 
+        # An input role might be defined as a more general `Role` while
+        # the `existing_role` will always be a concrete dialect-specific version.
+        concrete_defined_role = role_cls.from_unknown_role(role).normalize()
+
         if role_created:
-            result.append(CreateRoleOp(role))
+            result.append(CreateRoleOp(concrete_defined_role))
         else:
-            existing_role = existing_roles_by_name[role_name]
+            existing_role = existing_roles_by_name[role_name].normalize()
             role_cls = type(existing_role)
 
-            # An input role might be defined as a more general `Role` while
-            # the `existing_role` will always be a concrete dialect-specific version.
-            concrete_defined_role = role_cls.from_unknown_role(role)
-
             role_updated = existing_role != concrete_defined_role
             if role_updated:
                 existing_role = existing_roles_by_name[role_name]
                 result.append(
                     UpdateRoleOp(
                         from_role=existing_role,
-                        to_role=role_cls.from_unknown_role(role),
+                        to_role=concrete_defined_role,
                     )
                 )
 
     if not roles.ignore_unspecified:
         for removed_role in removed_role_names:
             if removed_role in roles.ignore_roles:
                 continue
+
             result.append(DropRoleOp(role_cls(removed_role)))
 
     return result
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/ddl.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/role/topological_sort.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/role/topological_sort.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Iterable, Set
 
-from sqlalchemy_declarative_extensions.role.generic import Role
+from sqlalchemy_declarative_extensions.role.generic import Role, role_names
 
 
 def topological_sort(roles: Iterable[Role]):
     """Sort roles in an order that guarantees success based on role dependence.
 
     Uses Kahn's algorithm.
     """
@@ -63,18 +63,18 @@
     return result
 
 
 def generate_role_dependency_map(role_name_map: Dict[str, Role]) -> Dict[str, Set[str]]:
     result: Dict[str, Set[str]] = {}
     valid_role_names = set(role_name_map)
     for name, role in role_name_map.items():
-        in_roles = set(role.in_roles or [])
+        in_roles = set(role_names(role.in_roles or []))
 
         if not in_roles.issubset(valid_role_names):
             missing_roles = ", ".join(sorted(in_roles - valid_role_names))
             raise ValueError(
                 "The following roles are specified as dependencies of other "
                 "top-level roles, but are missing in the list of top-level "
                 f"roles: {missing_roles}."
             )
-        result[name] = in_roles
+        result[name] = set(in_roles)
     return result
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/row/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/row/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/row/compare.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/row/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/schema/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/schema/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/schema/compare.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/schema/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/schema/ddl.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/schema/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/sql.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/sql.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/sqlalchemy.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/sqlalchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 
 
 def dialect_dispatch(
     postgresql: Callable[Concatenate[Connection, P], T] | None = None,
     sqlite: Callable[Concatenate[Connection, P], T] | None = None,
     mysql: Callable[Concatenate[Connection, P], T] | None = None,
     snowflake: Callable[Concatenate[Connection, P], T] | None = None,
+    default: Callable[Concatenate[Connection, P], T] | None = None,
 ) -> Callable[Concatenate[Connection, P], T]:
     dispatchers = {
         "postgresql": postgresql,
         "sqlite": sqlite,
         "mysql": mysql,
         "snowflake": snowflake,
     }
 
     def dispatch(connection: Connection, *args: P.args, **kwargs: P.kwargs) -> T:
         dialect_name = connection.dialect.name
-        if dialect_name == "pmrsqlite":
+        if "sqlite" in dialect_name:
             dialect_name = "sqlite"
 
-        dispatcher = dispatchers.get(dialect_name)
+        dispatcher = dispatchers.get(dialect_name) or default
         if dispatcher is None:  # pragma: no cover
             raise NotImplementedError(
                 f"'{dialect_name}' is not yet supported for this operation."
             )
 
         return dispatcher(connection, *args, **kwargs)
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/trigger/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/trigger/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/trigger/compare.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/trigger/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/trigger/ddl.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/trigger/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/view/base.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/view/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 from __future__ import annotations
 
+import inspect
 import uuid
+import warnings
 from dataclasses import dataclass, field, replace
-from typing import Any, Callable, Iterable, List, Optional, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, List, Optional, TypeVar, cast
 
 from sqlalchemy import Index, MetaData, UniqueConstraint, text
 from sqlalchemy.engine import Connection, Dialect
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.compiler import IdentifierPreparer
 from sqlalchemy.sql.elements import conv
 from sqlalchemy.sql.naming import ConventionDict
 from sqlalchemy.sql.schema import DEFAULT_NAMING_CONVENTION
+from typing_extensions import Self
 
 from sqlalchemy_declarative_extensions.sql import qualify_name
 from sqlalchemy_declarative_extensions.sqlalchemy import (
     HasMetaData,
     create_mapper,
     escape_params,
 )
 
+if TYPE_CHECKING:
+    from sqlalchemy_declarative_extensions.dialects.postgresql import (
+        MaterializedOptions,
+    )
+
 T = TypeVar("T")
+ViewType = TypeVar("ViewType", "View", "DeclarativeView")
 
 
-def view(base, materialized: bool = False, register_as_model=False) -> Callable[[T], T]:
+def view(
+    base,
+    *,
+    register_as_model=False,
+    materialized: bool | dict | MaterializedOptions = False,
+) -> Callable[[T], T]:
     """Decorate a class or declarative base model in order to register a View.
 
     Given some object with the attributes: `__tablename__`, (optionally for schema) `__table_args__`,
     and `__view__`, registers a View object.
 
-    The `__view__` attribute can be either a raw string query, or a SQLAlchemy object
-    capable of being compiled (namely :func:`~sqlalchemy.sql.expression.text` or :func:`~sqlalchemy.sql.expression.select`).
+    The `__view__` attribute can be either a raw string query, a SQLAlchemy object
+    capable of being compiled (namely :func:`~sqlalchemy.sql.expression.text` or
+    :func:`~sqlalchemy.sql.expression.select`), or a no-argument function which returns
+    either of the two.
 
     This intentionally allows one to register a Model definition as a view,
     and have it register in the same way you might otherwise manually define it.
     This can be useful, to enable querying that view in native SQLAlchemy ORM-style,
     as though it were a table.
 
     Arguments:
         base: A declarative base object
-        materialized: Whether the view should be a materialized view
         register_as_model: Whether the view should be registered as a SQLAlchemy mapped object.
             Note this only works if the view defines mappable models columns (minimally a primary
             key), like a proper modeled table
+        materialized: Whether a view should be materialized or not. Accepts a `bool` for default
+            options, a dialect-specific `MaterializedOptions` variant, or a dict describing that
+            dialect-specific variant.
 
     >>> try:
     ...     from sqlalchemy.orm import declarative_base
     ... except ImportError:
     ...     from sqlalchemy_declarative_extensions.sqlalchemy import declarative_base
     >>> from sqlalchemy import Column, types
     >>> from sqlalchemy_declarative_extensions import view
@@ -60,27 +78,15 @@
     ...     id = Column(types.Integer, primary_key=True)
     """
     metadata = getattr(base, "metadata", None)
     if metadata is None:  # pragma: no cover
         raise ValueError("Model must have a 'metadata' attribute.")
 
     def decorator(cls):
-        name = cls.__tablename__
-        table_args = getattr(cls, "__table_args__", None)
-        view_def = cls.__view__
-
-        schema = find_schema(table_args)
-        constraints = find_constraints(table_args)
-        instance = View(
-            name,
-            view_def,
-            schema=schema,
-            materialized=materialized,
-            constraints=constraints,
-        )
+        instance = DeclarativeView(cls, materialized)
 
         register_view(base, instance)
 
         if register_as_model:
             return instrument_sqlalchemy(base, cls)
         return cls
 
@@ -88,15 +94,15 @@
 
 
 def instrument_sqlalchemy(base: T, cls) -> T:
     temp_metadata = MetaData(naming_convention=base.metadata.naming_convention)  # type: ignore
     return create_mapper(cls, temp_metadata)
 
 
-def register_view(base_or_metadata: HasMetaData | MetaData, view: View):
+def register_view(base_or_metadata: HasMetaData | MetaData, view: ViewType):
     """Register a view onto the given declarative base or `Metadata`.
 
     This can be used instead of the [view](view) decorator, if you are constructing
     `View` objects directly. In this way, you can imperitively register views next
     to their corresponding table definitions, rather than at the root declarative
     base, like many of the other object types are documented to do.
     """
@@ -107,14 +113,63 @@
 
     if not metadata.info.get("views"):
         metadata.info["views"] = Views()
     metadata.info["views"].append(view)
 
 
 @dataclass
+class DeclarativeView:
+    cls: type
+    materialized: bool | dict | MaterializedOptions
+
+    @property
+    def name(self):
+        return self.cls.__tablename__
+
+    @property
+    def table_args(self):
+        return getattr(self.cls, "__table_args__", None)
+
+    @property
+    def view_def(self):
+        if inspect.isfunction(self.cls.__view__):
+            return self.cls.__view__()
+
+        return self.cls.__view__
+
+    @property
+    def schema(self):
+        table_args = self.table_args
+        if isinstance(table_args, dict):
+            return table_args.get("schema")
+
+        if isinstance(table_args, Iterable):
+            for table_arg in table_args:
+                if isinstance(table_arg, dict):
+                    return table_arg.get("schema")
+
+        return None
+
+    @property
+    def constraints(self):
+        table_args = self.table_args
+        if isinstance(table_args, dict):
+            return None
+
+        if isinstance(table_args, Iterable):
+            return [
+                arg
+                for arg in table_args
+                if isinstance(arg, (UniqueConstraint, ViewIndex, Index))
+            ]
+
+        return None
+
+
+@dataclass
 class View:
     """Definition of a view.
 
     **Note** the `materialized` field will always be false for databases
     which don't support it, and may generate invalid SQL if declared when
     unsupported.
 
@@ -122,38 +177,30 @@
     base/metadata `Views` object, called with `register_view`, or produced by
     a `view` decorator.
     """
 
     name: str
     definition: str | Select
     schema: str | None = None
-    materialized: bool = False
+    materialized: bool | dict | MaterializedOptions = False
     constraints: list[Index | UniqueConstraint | ViewIndex] | None = field(default=None)
 
     @classmethod
     def coerce_from_unknown(cls, unknown: Any) -> View:
         if isinstance(unknown, View):
-            return unknown
+            if unknown.materialized or unknown.constraints:
+                warnings.warn(
+                    "`materialized` and `constraints` have been relocated to dialect-specific MaterializedView variants.",
+                    DeprecationWarning,
+                )
 
-        try:
-            import alembic_utils  # noqa
-        except ImportError:  # pragma: no cover
-            pass
-        else:
-            from alembic_utils.pg_materialized_view import PGMaterializedView
-            from alembic_utils.pg_view import PGView
+            return unknown
 
-            if isinstance(unknown, (PGView, PGMaterializedView)):
-                materialized = isinstance(unknown, PGMaterializedView)
-                return cls(
-                    name=unknown.signature,
-                    definition=unknown.definition,
-                    schema=unknown.schema,
-                    materialized=materialized,
-                )
+        if isinstance(unknown, DeclarativeView):
+            return cls(unknown.name, unknown.view_def, unknown.schema)
 
         raise NotImplementedError(
             f"Unsupported view source object {unknown}"
         )  # pragma: no cover
 
     @property
     def qualified_name(self):
@@ -238,39 +285,34 @@
                 query = constraint.drop(self)
 
             result.append(query)
         return result
 
     def normalize(
         self, conn: Connection, metadata: MetaData, using_connection: bool = True
-    ) -> View:
+    ) -> Self:
         constraints = None
         if self.constraints:
             constraints = [
                 ViewIndex.from_unknown(c, self, conn.dialect, metadata)
                 for c in self.constraints
             ]
 
         return replace(
             self,
             definition=self.render_definition(conn, using_connection=using_connection),
             constraints=constraints,
         )
 
     def to_sql_create(self, dialect: Dialect) -> list[str]:
-        definition = self.compile_definition(dialect)
+        assert self.materialized is False
 
-        components = ["CREATE"]
-        if self.materialized:
-            components.append("MATERIALIZED")
+        definition = self.compile_definition(dialect)
 
-        components.append("VIEW")
-        components.append(self.qualified_name)
-        components.append("AS")
-        components.append(definition)
+        components = ["CREATE", "VIEW", self.qualified_name, "AS", definition]
         statement = " ".join(components)
 
         result = [statement]
         result.extend(self.render_constraints(create=True))
 
         return result
 
@@ -308,83 +350,14 @@
         result.extend(self.render_constraints(create=False))
         result.append(statement)
 
         return result
 
 
 @dataclass
-class Views:
-    """The collection of views and associated options comparisons.
-
-    Note: `Views` supports views being specified from certain alternative sources, such
-    as `alembic_utils`'s `PGView` and `PGMaterializedView`. In order for that to work,
-    one needs to either call `View.coerce_from_unknown(alembic_utils_view)` directly, or
-    use `Views().are(...)` (which internally calls `coerce_from_unknown`).
-
-    Note: `ignore` option accepts a list of strings. Each string is individually
-        interpreted as a "glob". This means a string like "foo.*" would ignore all views
-        contained within the schema "foo".
-    """
-
-    views: list[View] = field(default_factory=list)
-
-    ignore_unspecified: bool = False
-
-    ignore: Iterable[str] = field(default_factory=set)
-    ignore_views: Iterable[str] = field(default_factory=set)
-
-    @classmethod
-    def coerce_from_unknown(
-        cls, unknown: None | Iterable[View] | Views
-    ) -> Views | None:
-        if isinstance(unknown, Views):
-            return unknown
-
-        if isinstance(unknown, Iterable):
-            return cls().are(*unknown)
-
-        return None
-
-    def append(self, view: View):
-        self.views.append(view)
-
-    def __iter__(self):
-        yield from self.views
-
-    def are(self, *views: View):
-        return replace(self, views=[View.coerce_from_unknown(v) for v in views])
-
-
-def find_schema(table_args=None):
-    if isinstance(table_args, dict):
-        return table_args.get("schema")
-
-    if isinstance(table_args, Iterable):
-        for table_arg in table_args:
-            if isinstance(table_arg, dict):
-                return table_arg.get("schema")
-
-    return None
-
-
-def find_constraints(table_args=None):
-    if isinstance(table_args, dict):
-        return None
-
-    if isinstance(table_args, Iterable):
-        return [
-            arg
-            for arg in table_args
-            if isinstance(arg, (UniqueConstraint, ViewIndex, Index))
-        ]
-
-    return None
-
-
-@dataclass
 class ViewIndex:
     columns: list[str]
     name: str | None = None
     unique: bool = False
 
     @classmethod
     def from_unknown(
@@ -505,7 +478,50 @@
 @dataclass
 class _ColumnNamingAdapter:
     name: str
 
     @property
     def _ddl_label(self):
         return self.name
+
+
+@dataclass
+class Views:
+    """The collection of views and associated options comparisons.
+
+    Note: `Views` supports views being specified from certain alternative sources, such
+    as `alembic_utils`'s `PGView` and `PGMaterializedView`. In order for that to work,
+    one needs to either call `View.coerce_from_unknown(alembic_utils_view)` directly, or
+    use `Views().are(...)` (which internally calls `coerce_from_unknown`).
+
+    Note: `ignore` option accepts a list of strings. Each string is individually
+        interpreted as a "glob". This means a string like "foo.*" would ignore all views
+        contained within the schema "foo".
+    """
+
+    views: list[View | DeclarativeView] = field(default_factory=list)
+
+    ignore_unspecified: bool = False
+
+    ignore: Iterable[str] = field(default_factory=set)
+    ignore_views: Iterable[str] = field(default_factory=set)
+
+    @classmethod
+    def coerce_from_unknown(
+        cls, unknown: None | Iterable[View] | Views
+    ) -> Views | None:
+        if isinstance(unknown, Views):
+            return unknown
+
+        if isinstance(unknown, Iterable):
+            return cls().are(*unknown)
+
+        return None
+
+    def append(self, view: View | DeclarativeView):
+        self.views.append(view)
+
+    def __iter__(self):
+        yield from self.views
+
+    def are(self, *views: View):
+        return replace(self, views=list(views))
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/view/compare.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/view/compare.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass, replace
 from fnmatch import fnmatch
 from typing import Union
 
 from sqlalchemy import MetaData
 from sqlalchemy.engine import Connection, Dialect
 
-from sqlalchemy_declarative_extensions.dialects import get_views
+from sqlalchemy_declarative_extensions.dialects import get_view_cls, get_views
 from sqlalchemy_declarative_extensions.view.base import View, Views
 
 
 @dataclass
 class CreateViewOp:
     view: View
 
@@ -59,25 +59,30 @@
         warnings.warn(
             "`ignore_views` is deprecated, use `ignore` instead", DeprecationWarning
         )
         views = replace(views, ignore=list(views.ignore_views) + list(views.ignore))
 
     result: list[Operation] = []
 
-    views_by_name = {r.qualified_name: r for r in views.views}
+    view_cls = get_view_cls(connection)
+    concrete_defined_views: list[View] = [
+        view_cls.coerce_from_unknown(view) for view in views.views
+    ]
+
+    views_by_name = {r.qualified_name: r for r in concrete_defined_views}
     expected_view_names = set(views_by_name)
 
     existing_views = get_views(connection)
     existing_views_by_name = {r.qualified_name: r for r in existing_views}
     existing_view_names = set(existing_views_by_name)
 
     new_view_names = expected_view_names - existing_view_names
     removed_view_names = existing_view_names - expected_view_names
 
-    for view in views:
+    for view in concrete_defined_views:
         view_name = view.qualified_name
 
         ignore_matches = any(
             fnmatch(view_name, view_pattern) for view_pattern in views.ignore
         )
         if ignore_matches:
             continue
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/src/sqlalchemy_declarative_extensions/view/ddl.py` & `sqlalchemy-declarative-extensions-0.9.1/src/sqlalchemy_declarative_extensions/view/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.3/setup.py` & `sqlalchemy-declarative-extensions-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ['sqlalchemy>=1.3']
 
 extras_require = \
 {'alembic': ['alembic>=1.0'], 'parse': ['sqlglot']}
 
 setup_kwargs = {
     'name': 'sqlalchemy-declarative-extensions',
-    'version': '0.8.3',
+    'version': '0.9.1',
     'description': 'Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic.',
     'long_description': '# SQLAlchemy Declarative Extensions\n\n[![Actions Status](https://github.com/dancardin/sqlalchemy-declarative-extensions/workflows/test/badge.svg)](https://github.com/dancardin/sqlalchemy-declarative-extensions/actions)\n[![Coverage Status](https://coveralls.io/repos/github/DanCardin/sqlalchemy-declarative-extensions/badge.svg?branch=main)](https://coveralls.io/github/DanCardin/sqlalchemy-declarative-extensions?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/sqlalchemy-declarative-extensions/badge/?version=latest)](https://sqlalchemy-declarative-extensions.readthedocs.io/en/latest/?badge=latest)\n\nSee the full documentation\n[here](https://sqlalchemy-declarative-extensions.readthedocs.io/en/latest/).\n\nAdds extensions to SQLAlchemy (and/or Alembic) which allows declaratively\nstating the existence of additional kinds of objects about your database not\nnatively supported by SQLAlchemy/Alembic.\n\nThis includes:\n\n- Schemas\n- Views\n- Roles\n- Privileges (Grants/Default Grants)\n- Functions\n- Triggers\n- Rows (i.e. data)\n- "audit tables" (i.e. triggers which record data changes to some source table)\n\nThe primary function(s) of this library include:\n\n- Registering onto the SQLAlchemy event system such that `metadata.create_all`\n  creates these objects.\n- (Optionally) Registers into Alembic such that\n  `alembic revision --autogenerate` automatically creates/updates/deletes\n  declared objects.\n\n## Kitchen Sink Example (using all available features)\n\n```python\nfrom sqlalchemy import Column, types, select\nfrom sqlalchemy.orm import as_declarative\nfrom sqlalchemy_declarative_extensions import (\n    declarative_database, Schemas, Roles, Row, View, view,\n)\nfrom sqlalchemy_declarative_extensions.dialects.postgresql import (\n    DefaultGrant, Function, Trigger, Role\n)\nfrom sqlalchemy_declarative_extensions.audit import audit\n\n\n@declarative_database\n@as_declarative\nclass Base:\n    # Note: each object type also has a plural version (i.e. Schemas/Roles/etc) where you can specify\n    # collection-level options like `ignore_unspecified`).\n    #\n    # If you dont set any collection-level options, you can instead use raw list/iterable as the collection.\n    schemas = Schemas().are("example")\n    roles = Roles(ignore_unspecified=True).are(\n        Role("read", login=False),\n        Role(\n            "app",\n            in_roles=[\'read\']\n        ),\n    )\n    grants = [\n        DefaultGrant.on_tables_in_schema("public", \'example\').grant("select", to="read"),\n        DefaultGrant.on_sequences_in_schema("public").grant("usage", to="read"),\n        Grant.new("usage", to="read").on_schemas("example")\n    ]\n    rows = [\n        Row(\'foo\', id=1),\n    ]\n    views = [\n        View("low_foo", "select * from foo where i < 10"),\n    ]\n    functions = [\n        Function(\n            "fancy_function",\n            """\n            BEGIN\n            INSERT INTO foo (id) select NEW.id + 1;\n            RETURN NULL;\n            END\n            """,\n            language="plpgsql",\n            returns="trigger",\n        ),\n    ]\n    triggers = [\n        Trigger.after("insert", on="foo", execute="fancy_function")\n        .named("on_insert_foo")\n        .when("pg_trigger_depth() < 1")\n        .for_each_row(),\n    ]\n\n\n@audit()\nclass Foo(Base):\n    __tablename__ = \'foo\'\n\n    id = Column(types.Integer(), primary_key=True)\n\n\naudit_table = Foo.__audit_table__\n\n\n@view(Base)\nclass HighFoo:\n    __tablename__ = "high_foo"\n    __view__ = select(Foo.__table__).where(Foo.__table__.c.id >= 10)\n```\n\nNote, there is also support for declaring objects directly through the\n`MetaData` for users not using sqlalchemy\'s declarative API.\n\n## Event Registration\n\nBy default, the above example does not automatically do anything. Depending on\nthe context, you can use one of two registration hooks:\n`register_sqlalchemy_events` or `register_alembic_events`.\n\n### `register_sqlalchemy_events`\n\nThis registers events in SQLAlchemy\'s event system such that a\n`metadata.create_all(...)` call will create the declared database objects.\n\n```python\nfrom sqlalchemy_declarative_extensions import register_sqlalchemy_events\n\nmetadata = Base.metadata  # Given the example above.\nregister_sqlalchemy_events(metadata)\n# Which is equivalent to...\nregister_sqlalchemy_events(metadata, schemas=False, roles=False, grants=False, rows=False)\n```\n\nAll object types are opt in, and should be explicitly included in order to get\nregistered.\n\nPractically, this is to avoid issues with testing. In **most** cases the\n`metadata.create_all` call will be run in tests, a context where it\'s more\nlikely that you dont **need** grants or grants, and where parallel test\nexecution could lead to issues with role or schema creation, depending on your\nsetup.\n\n### `register_alembic_events`\n\nThis registers comparators in Alembic\'s registration system such that an\n`alembic revision --autogenerate` command will diff the existing database state\nagainst the declared database objects, and issue statements to\ncreate/update/delete objects in order to match the declared state.\n\n```python\n# alembic\'s `env.py`\nfrom sqlalchemy_declarative_extensions import register_alembic_events\n\nregister_alembic_events()\n# Which is equivalent to...\nregister_sqlalchemy_events(schemas=True, roles=True, grants=True, rows=True)\n```\n\nAll object types are opt out but can be excluded.\n\nIn contrast to `register_sqlalchemy_events`, it\'s much more likely that you\'re\ndeclaring most of these object types in order to have alembic track them\n\n## Database support\n\nIn principle, this library **can** absolutely support any database supported by\nSQLAlchemy, and capable of being introspected enough to support detection of\ndifferent kinds of objects.\n\nAs you can see below, in reality the existence of implementations are going to\nbe purely driven by actual usage. The current maintainer(s) primarily use\nPostgreSQL and as such individual features for other databases will either\nsuffer or lack implementation.\n\n|               | Postgres | MySQL | SQLite | Snowflake |\n| ------------- | -------- | ----- | ------ | --------- |\n| Schema        | ✓        | N/A   | ✓      | ✓         |\n| View          | ✓        | ✓     | ✓      |           |\n| Role          | ✓        |       | N/A    |           |\n| Grant         | ✓        |       | N/A    |           |\n| Default Grant | ✓        |       | N/A    |           |\n| Function      | ✓        | *     |        |           |\n| Trigger       | ✓        | *     |        |           |\n| Row (data)    | ✓        | ✓     | ✓      | ✓         |\n| "Audit Table" | ✓        |       |        |           |\n\n**note** "Row" is implemented with pure SQLAlchemy concepts, so should work for\nany dialect that you can use SQLAlchemy to connect to.\n\nThe astrisks above note pending or provisional support through basic test cases.\nThe level of expertise in each dialects\' particular behaviors is not uniform,\nand deciding on the correct behavior for those dialects will require users to\nsubmit issues/fixes!\n\nSupporting a new dialect **can** be as simple as providing the\ndialect-dispatched implementations for detecting existing objects of the given\ntype. Very much the intent is that once a given object type is supported at all,\nthe comparison infrastructure for that type should make it straightforward to\nsupport other dialects. At the end of the day, this library is primarily\nproducing SQL statements, so in theory any dialect supporting a given object\ntype should be able to be supported.\n\nIn such cases (like Grants/Roles) that different dialects support wildly\ndifferent options/syntax, there are also patterns for defining dialect-specific\nobjects, to mediate any additional differences.\n\n## Alembic-utils\n\n[Alembic Utils](https://github.com/olirice/alembic_utils) is the primary library\nagainst which this library can be compared. At time of writing, **most** (but\nnot all) object types supported by alembic-utils are supported by this library.\nOne might begin to question when to use which library.\n\nBelow is a list of points on which the two libraries diverge. But note that you\n**can** certainly use both in tandem! It doesn\'t need to be one or the other,\nand certainly for any object types which do not overlap, you might **need** to\nuse both.\n\n- Database Support\n\n  - Alembic Utils seems to explicitly only support PostgreSQL.\n\n  - This library is designed to support any dialect (in theory). Certainly\n    PostgreSQL is **best** supported, but there does exist support for specific\n    kinds of objects to varying levels of support for SQLite and MySQL, so far.\n\n- Architecture\n\n  - Alembic Utils is directly tied to Alembic and does not support SQLAlchemy\'s\n    `MetaData.create_all`. It\'s also the responsibility of the user to\n    discover/register objects in alembic.\n\n  - This library **depends** only on SQLAlchemy, although it also supports\n    alembic. Support for `MetaData.create_all` can be important for creating all\n    object types in tests. It also is designed such that objects are registered\n    on the `MetaData` itself, so there is no need for any specific discovery\n    phase.\n\n- Scope\n\n  - Alembic Utils declares specific, individual objects. I.e. you instantiate\n    one specific `PGGrantTable` or `PGView` instance and Alembic know knows you\n    want that object to be created. It cannot drop objects it is not already\n    aware of.\n\n  - This library declares ths objects the system as a whole expects to exist.\n    Similar to Alembic\'s behavior on tables, it will (by default) detect any\n    **undeclared** objects that should not exist and drop them. That means, you\n    can rely on this object to ensure the state of your migrations matches the\n    state of your database exactly.\n\n- Migration history\n\n  - Alembic Utils imports and references its own objects in your migrations\n    history. This can be unfortunate, in that it deeply ties your migrations\n    history to alembic-utils.\n\n    (In fact, this can be a sticking point, trying to convert **away** from\n    `alembic_utils`, because it will attempt to drop all the (e.g `PGView`)\n    instances previously created when we replaced it with this library.)\n\n  - This library, by contrast, prefers to emit the raw SQL of the operation into\n    your migration. That means you know the exact commands that will execute in\n    your migration, which can be helpful in debugging failure. It also means, if\n    at any point you decide to stop use of the library (or pause a given type of\n    object, due to a bug), you can! This library\'s behaviors are primarily very\n    much `--autogenerate`-time only.\n\n- Abstraction Level\n\n  - Alembic Utils appears to define a very "literal" interface (for example,\n    `PGView` accepts the whole view definition as a raw literal string).\n\n  - This library tries to, as much as possible, provide a more abstracted\n    interface that enables more compatibility with SQLAlchemy (For example\n    `View` accepts SQLAlchemy objects which can be coerced into a `SELECT`). It\n    also tends towards "builder" interfaces which progressively produce a object\n    (Take a look at the `DefaultGrant` above, for an example of where that\'s\n    helpful).\n\nA separate note on conversion/compatibility. Where possible, this library tries\nto support alembic-utils native objects as stand-ins for the objects defined in\nthis library. For example, `alembic_utils.pg_view.PGView` can be declared\ninstead of a `sqlalchemy_declarative_extensions.View`, and we will internally\ncoerce it into the appropriate type. Hopefully this eases any transitional\ncosts, or issues using one or the other library.\n',
     'author': 'Dan Cardin',
     'author_email': 'ddcardin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dancardin/sqlalchemy-declarative-extensions',
```

### Comparing `sqlalchemy-declarative-extensions-0.8.3/PKG-INFO` & `sqlalchemy-declarative-extensions-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-declarative-extensions
-Version: 0.8.3
+Version: 0.9.1
 Summary: Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic.
 Home-page: https://github.com/dancardin/sqlalchemy-declarative-extensions
 License: Apache-2.0
 Keywords: alembic,declarative,grant,mysql,postgresql,role,schema,sqlalchemy,view
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.8,<4
```

