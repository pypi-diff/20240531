# Comparing `tmp/django_db_views-0.1.7.dev1.tar.gz` & `tmp/django_db_views-0.1.8.tar.gz`

## Comparing `django_db_views-0.1.7.dev1.tar` & `django_db_views-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/CHANGELOG.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/__init__.py
--rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/autodetector.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/context_manager.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/db_view.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/migration_functions.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/operations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/management/commands/__init__.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/management/commands/makeviewmigrations.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/LICENSE
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/README.md
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/pyproject.toml
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/PKG-INFO
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 django_db_views-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/__init__.py
+-rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/autodetector.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/context_manager.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/db_view.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/migration_functions.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/operations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/management/commands/__init__.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 django_db_views-0.1.8/django_db_views/management/commands/makeviewmigrations.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_db_views-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_db_views-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 django_db_views-0.1.8/README.md
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 django_db_views-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 django_db_views-0.1.8/PKG-INFO
```

### Comparing `django_db_views-0.1.7.dev1/CHANGELOG.md` & `django_db_views-0.1.8/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 Changelogs starts from version 0.1.3
 
 ## Unreleased
 
 ## Released
 
+### [0.1.8]
+- Sqlmigrate command shows sql definitions of a view models
+
 ### [0.1.7]
 - Support for reading ViewRunPython operations from SeparateDatabaseAndState operations
 
 ### [0.1.6]
 - Adjusted tests to django 4.2
 
 ### [0.1.5]
```

### Comparing `django_db_views-0.1.7.dev1/django_db_views/autodetector.py` & `django_db_views-0.1.8/django_db_views/autodetector.py`

 * *Files identical despite different names*

### Comparing `django_db_views-0.1.7.dev1/django_db_views/db_view.py` & `django_db_views-0.1.8/django_db_views/db_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 
 DBViewsRegistry = {}
 
 
 class DBViewModelBase(ModelBase):
     def __new__(cls, *args, **kwargs):
         new_class = super().__new__(cls, *args, **kwargs)
-        assert new_class._meta.managed is False, "For DB View managed must be se to false"
+        assert (
+            new_class._meta.managed is False
+        ), "For DB View managed must be se to false"
         DBViewsRegistry[new_class._meta.db_table] = new_class
         return new_class
 
 
 class DBView(models.Model, metaclass=DBViewModelBase):
     """
-        Children should define:
-            view_definition - define the view, can be callable or attribute (string)
-            view definition can be per db engine.
+    Children should define:
+        view_definition - define the view, can be callable or attribute (string)
+        view definition can be per db engine.
     """
+
     view_definition: Union[Callable, str, dict]
 
     class Meta:
         managed = False
         abstract = True
 
 
@@ -36,10 +39,12 @@
     def refresh(cls, using=None, concurrently=False):
         """
         concurrently option requires an index and postgres db
         """
         using = using or DEFAULT_DB_ALIAS
         with connections[using].cursor() as cursor:
             if concurrently:
-                cursor.execute("REFRESH MATERIALIZED VIEW CONCURRENTLY %s;" % cls._meta.db_table)
+                cursor.execute(
+                    "REFRESH MATERIALIZED VIEW CONCURRENTLY %s;" % cls._meta.db_table
+                )
             else:
                 cursor.execute("REFRESH MATERIALIZED VIEW %s;" % cls._meta.db_table)
```

### Comparing `django_db_views-0.1.7.dev1/django_db_views/migration_functions.py` & `django_db_views-0.1.8/django_db_views/migration_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,26 +12,41 @@
         self.view_definition = view_definition
         self.table_name = table_name
 
 
 class ForwardViewMigrationBase(ViewMigration):
     def __call__(self, apps, schema_editor):
         if self.view_definition:
-            if self.view_engine is None or self.view_engine == schema_editor.connection.settings_dict['ENGINE']:
+            if (
+                self.view_engine is None
+                or self.view_engine == schema_editor.connection.settings_dict["ENGINE"]
+            ):
                 schema_editor.execute(self.DROP_COMMAND_TEMPLATE % self.table_name)
-                schema_editor.execute(self.CREATE_COMMAND_TEMPLATE % (self.table_name, self.view_definition))
+                schema_editor.execute(
+                    self.CREATE_COMMAND_TEMPLATE
+                    % (self.table_name, self.view_definition)
+                )
 
 
 class BackwardViewMigrationBase(ViewMigration):
     def __call__(self, apps, schema_editor):
-        if self.view_engine is None or self.view_engine == schema_editor.connection.settings_dict['ENGINE']:
+        if (
+            self.view_engine is None
+            or self.view_engine == schema_editor.connection.settings_dict["ENGINE"]
+        ):
             schema_editor.execute(self.DROP_COMMAND_TEMPLATE % self.table_name)
         if self.view_definition:
-            if self.view_engine is None or self.view_engine == schema_editor.connection.settings_dict['ENGINE']:
-                schema_editor.execute(self.CREATE_COMMAND_TEMPLATE % (self.table_name, self.view_definition))
+            if (
+                self.view_engine is None
+                or self.view_engine == schema_editor.connection.settings_dict["ENGINE"]
+            ):
+                schema_editor.execute(
+                    self.CREATE_COMMAND_TEMPLATE
+                    % (self.table_name, self.view_definition)
+                )
 
 
 @deconstructible
 class ForwardViewMigration(ForwardViewMigrationBase):
     DROP_COMMAND_TEMPLATE = "DROP VIEW IF EXISTS %s;"
     CREATE_COMMAND_TEMPLATE = "CREATE VIEW %s as %s;"
 
@@ -58,15 +73,18 @@
     DROP_COMMAND_TEMPLATE: str
 
     def __init__(self, table_name: str, engine=None):
         self.table_name = table_name
         self.view_engine = engine
 
     def __call__(self, apps, schema_editor):
-        if self.view_engine is None or self.view_engine == schema_editor.connection.settings_dict['ENGINE']:
+        if (
+            self.view_engine is None
+            or self.view_engine == schema_editor.connection.settings_dict["ENGINE"]
+        ):
             schema_editor.execute(self.DROP_COMMAND_TEMPLATE % self.table_name)
 
 
 @deconstructible
 class DropMaterializedView(DropViewMigration):
     DROP_COMMAND_TEMPLATE = "DROP MATERIALIZED VIEW IF EXISTS %s;"
```

### Comparing `django_db_views-0.1.7.dev1/django_db_views/operations.py` & `django_db_views-0.1.8/django_db_views/operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 from django.db.migrations import operations
 from django.db.migrations.state import ModelState
 
 from django_db_views.context_manager import VIEW_MIGRATION_CONTEXT
 from django_db_views.db_view import DBView, DBMaterializedView
-from django_db_views.migration_functions import ForwardMaterializedViewMigration, ForwardViewMigration
+from django_db_views.migration_functions import (
+    ForwardMaterializedViewMigration,
+    ForwardViewMigration,
+)
 
 
 def get_table_engine_name_hash(table_name, engine):
     return f"{table_name}_{engine}".lower()
 
 
 class DBViewModelState(ModelState):
     def __init__(
-            self, *args,
-            # Not required cus migrate also load state using clone method that do not provide required by us fields.
-            view_engine: str = None,
-            view_definition: str = None,
-            table_name: str = None,
-            base_class=None,
-            **kwargs
+        self,
+        *args,
+        # Not required cus migrate also load state using clone method that do not provide required by us fields.
+        view_engine: str = None,
+        view_definition: str = None,
+        table_name: str = None,
+        base_class=None,
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if VIEW_MIGRATION_CONTEXT["is_view_migration"]:
             self.view_engine = view_engine
             self.view_definition = view_definition
             self.base_class = base_class
             self.table_name = table_name
 
 
 class ViewRunPython(operations.RunPython):
+    reduces_to_sql = True
 
     def state_forwards(self, app_label, state):
         if VIEW_MIGRATION_CONTEXT["is_view_migration"]:
             if isinstance(self.code, ForwardMaterializedViewMigration):
                 model = DBMaterializedView
             elif isinstance(self.code, ForwardViewMigration):
                 model = DBView
             else:
                 raise NotImplementedError
             state.add_model(
                 DBViewModelState(
                     app_label,
                     # Hash table_name_engine_name to add state model per migration, which are added per engine.
-                    get_table_engine_name_hash(self.code.table_name, self.code.view_engine),
+                    get_table_engine_name_hash(
+                        self.code.table_name, self.code.view_engine
+                    ),
                     list(),
                     dict(),
                     # we do not use django bases (they initialize model using that, and broke ViewRegistry),
                     # instead of that we pass bass class in separate argument.
                     tuple(),
                     list(),
                     view_engine=self.code.view_engine,
                     view_definition=self.code.view_definition,
                     base_class=model,
-                    table_name=self.code.table_name
+                    table_name=self.code.table_name,
                 )
             )
 
+    def describe(self):
+        return "View migration operation"
 
-class ViewDropRunPython(operations.RunPython):
 
+class ViewDropRunPython(operations.RunPython):
     def state_forwards(self, app_label, state):
         if VIEW_MIGRATION_CONTEXT["is_view_migration"]:
-            state.remove_model(app_label, get_table_engine_name_hash(self.code.table_name, self.code.view_engine))
+            state.remove_model(
+                app_label,
+                get_table_engine_name_hash(self.code.table_name, self.code.view_engine),
+            )
```

### Comparing `django_db_views-0.1.7.dev1/django_db_views/management/commands/makeviewmigrations.py` & `django_db_views-0.1.8/django_db_views/management/commands/makeviewmigrations.py`

 * *Files identical despite different names*

### Comparing `django_db_views-0.1.7.dev1/LICENSE` & `django_db_views-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_db_views-0.1.7.dev1/README.md` & `django_db_views-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django_db_views-0.1.7.dev1/pyproject.toml` & `django_db_views-0.1.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-db-views"
-version = "0.1.7.dev1"
+version = "0.1.8"
 description = """
     Handle database views.
     Allow to create migrations for database views.
     View migrations using django code.
     They can be reversed.
     Changes in model view definition are detected automatically.
     Support almost all options as regular makemigrations command
@@ -33,24 +33,38 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 py_modules = ["six"]
 dependencies = [
-  "django"
+    "six",
+    "django>=2.2"
 ]
 
 [project.urls]
 Homepage = "https://github.com/BezBartek/django-db-views"
 Documentation = "https://github.com/BezBartek/django-db-views/blob/master/README.md"
 Repository = "https://github.com/BezBartek/django-db-views"
 Issues = "https://github.com/BezBartek/django-db-views/issues"
 Changelog = "https://github.com/BezBartek/django-db-views/blob/master/CHANGELOG.md"
 
+[project.optional-dependencies]
+dev = [
+    "pre-commit==3.6.0",
+]
+tests = [
+    "psycopg2==2.9.3",
+    "pytest-django==4.5.2",
+    "django-environ==0.9.0",
+    "mysqlclient==2.2.1",
+    "pytest-mock==3.8.2",
+    "tox==3.25.1",
+    "build==1.2.1",
+]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
@@ -58,7 +72,32 @@
     '/CHANGELOG.md',
     '/LICENSE',
     '/django_db_views'
 ]
 
 [tool.pytest.ini_options]
 addopts = "--migrations --create-db"
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+isolated_build = True
+requires = tox-conda
+envlist = py39-dj{22,32,40,41}, py310-dj{22,32,40,41,42,50}, py311-dj{22,32,40,41,42,50}
+
+[testenv]
+conda_channels=
+    conda-forge
+conda_install_args=
+    --override-channels
+setenv =
+    PYTHONDONTWRITEBYTECODE=1
+conda_deps =
+    psycopg2
+    pytest-django
+    mysqlclient
+    pytest-mock
+deps =
+    django-environ==0.9.0
+
+commands = pytest tests/
+"""
```

### Comparing `django_db_views-0.1.7.dev1/PKG-INFO` & `django_db_views-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-db-views
-Version: 0.1.7.dev1
+Version: 0.1.8
 Summary:     Handle database views.     Allow to create migrations for database views.     View migrations using django code.     They can be reversed.     Changes in model view definition are detected automatically.     Support almost all options as regular makemigrations command
 Project-URL: Homepage, https://github.com/BezBartek/django-db-views
 Project-URL: Documentation, https://github.com/BezBartek/django-db-views/blob/master/README.md
 Project-URL: Repository, https://github.com/BezBartek/django-db-views
 Project-URL: Issues, https://github.com/BezBartek/django-db-views/issues
 Project-URL: Changelog, https://github.com/BezBartek/django-db-views/blob/master/CHANGELOG.md
 Author: Mariusz Okulanis
@@ -15,15 +15,26 @@
 Keywords: database perspective,database table function,database views,django,django materialized views,view migrations,views
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: django
+Requires-Dist: django>=2.2
+Requires-Dist: six
+Provides-Extra: dev
+Requires-Dist: pre-commit==3.6.0; extra == 'dev'
+Provides-Extra: tests
+Requires-Dist: build==1.2.1; extra == 'tests'
+Requires-Dist: django-environ==0.9.0; extra == 'tests'
+Requires-Dist: mysqlclient==2.2.1; extra == 'tests'
+Requires-Dist: psycopg2==2.9.3; extra == 'tests'
+Requires-Dist: pytest-django==4.5.2; extra == 'tests'
+Requires-Dist: pytest-mock==3.8.2; extra == 'tests'
+Requires-Dist: tox==3.25.1; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # django-db-views
 
 
 [![License](https://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)  
 [![PyPi](https://badge.fury.io/py/django-db-views.svg)](https://pypi.org/project/django-db-views/)
```

