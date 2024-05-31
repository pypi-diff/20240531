# Comparing `tmp/flask_template_cli-0.1.1.tar.gz` & `tmp/flask_template_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_template_cli-0.1.1.tar", last modified: Mon May 27 06:39:16 2024, max compression
+gzip compressed data, was "flask_template_cli-0.2.0.tar", last modified: Fri May 31 06:03:16 2024, max compression
```

## Comparing `flask_template_cli-0.1.1.tar` & `flask_template_cli-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:39:16.371343 flask_template_cli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-27 06:39:16.371343 flask_template_cli-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:39:16.367344 flask_template_cli-0.1.1/flask_template_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:39:16.367344 flask_template_cli-0.1.1/flask_template_cli/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/templates/init_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/templates/models_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/templates/req_txt_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/templates/routes_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/flask_template_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:39:16.367344 flask_template_cli-0.1.1/flask_template_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-27 06:39:16.000000 flask_template_cli-0.1.1/flask_template_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-27 06:39:16.000000 flask_template_cli-0.1.1/flask_template_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:39:16.000000 flask_template_cli-0.1.1/flask_template_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 06:39:16.000000 flask_template_cli-0.1.1/flask_template_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 06:39:16.000000 flask_template_cli-0.1.1/flask_template_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 06:39:16.000000 flask_template_cli-0.1.1/flask_template_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 06:39:16.371343 flask_template_cli-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:39:16.367344 flask_template_cli-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-27 06:39:09.000000 flask_template_cli-0.1.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:03:16.771392 flask_template_cli-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-31 06:03:16.771392 flask_template_cli-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:03:16.767392 flask_template_cli-0.2.0/flask_template_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:03:16.771392 flask_template_cli-0.2.0/flask_template_cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/templates/auth_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/templates/init_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/templates/models_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/templates/req_txt_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/templates/routes_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/flask_template_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:03:16.771392 flask_template_cli-0.2.0/flask_template_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-31 06:03:16.000000 flask_template_cli-0.2.0/flask_template_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-31 06:03:16.000000 flask_template_cli-0.2.0/flask_template_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:03:16.000000 flask_template_cli-0.2.0/flask_template_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 06:03:16.000000 flask_template_cli-0.2.0/flask_template_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 06:03:16.000000 flask_template_cli-0.2.0/flask_template_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 06:03:16.000000 flask_template_cli-0.2.0/flask_template_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-31 06:03:16.771392 flask_template_cli-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:03:16.771392 flask_template_cli-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-31 06:03:05.000000 flask_template_cli-0.2.0/tests/test_cli.py
```

### Comparing `flask_template_cli-0.1.1/flask_template_cli/templates/init_gen.py` & `flask_template_cli-0.2.0/flask_template_cli/templates/init_gen.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 """
 Generate the __init__.py file for the package
 """
+
 import os
 from typing import TextIO
 
 
 def init_gen(project):
     file_location = os.path.join(project.name, "app/__init__.py")
     with open(file_location, "w") as f:
         f.write(f"from flask import Flask\n\n")
 
-        if project.need_database:
-            if project.db_type == "SQL":
-                f.write("from flask_sqlalchemy import SQLAlchemy\n\n")
-            elif project.db_type == "NoSQL":
-                f.write("from flask_mongoengine import MongoEngine\n\n")
+        # if project.need_database:
+        #     if project.db_type == "SQL":
+        #         f.write("from flask_sqlalchemy import SQLAlchemy\n\n")
+        #     elif project.db_type == "NoSQL":
+        #         f.write("from flask_mongoengine import MongoEngine\n\n")
 
         f.write(f"""
 def create_app(): 
-    app = Flask(__name__)\n""")
+    app = Flask(__name__)\n\n""")
 
         if project.need_database:
             f.write(f"\tfrom .models import db\n")
-            f.write(f"\tdb.init_app(app)\n")
+            f.write(f"\tdb.init_app(app)\n\n")
 
-        # f.write(f"\tfrom .routes import my_routes\n")
-        # f.write(f"\tapp.register_blueprint(my_routes)\n")
         _routes_import(project, f)
 
+        _auth_import(project, f)
+
         f.write(f"\treturn app\n")
         f.write(f"\n")
 
 
 def _routes_import(project, f: TextIO):
     if project.project_type == "api":
         f.write(f"\tfrom .routes import api\n")
         f.write(f"\tapi.init_app(app)\n")
     else:
         f.write(f"\tfrom .routes import my_routes\n")
-        f.write(f"\tapp.register_blueprint(my_routes)\n")
+        f.write(f"\tapp.register_blueprint(my_routes)\n\n")
+
+
+def _auth_import(project, f: TextIO):
+    if project.need_auth:
+        f.write(f"\tfrom .routes import auth\n")
+        f.write(f"\tapp.register_blueprint(auth)\n\n")
+
+        if project.auth_type == "cookie":
+            f.write(f"\tfrom .routes import login_manager\n")
+            f.write(f"\tlogin_manager.init_app(app)\n\n")
+
+        elif project.auth_type == "token":
+            f.write(f"\tfrom .routes import jwt\n")
+            f.write(f"\tjwt.init_app(app)\n\n")
```

### Comparing `flask_template_cli-0.1.1/flask_template_cli/templates/models_gen.py` & `flask_template_cli-0.2.0/flask_template_cli/templates/models_gen.py`

 * *Files identical despite different names*

### Comparing `flask_template_cli-0.1.1/flask_template_cli/templates/req_txt_gen.py` & `flask_template_cli-0.2.0/flask_template_cli/templates/req_txt_gen.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 """
 
 
 def req_txt_gen(project):
     file_location = f"{project.name}/requirements.txt"
 
     with open(file_location, "w") as file:
-        file.write("flask\n")
+        project.add_requirements("flask")
 
         if project.project_type == "api":
             # Add flask-restful if project type is API
-            file.write("flask-restful\n")
+            project.add_requirements("flask-restful")
 
         if project.need_database:
             # Add database requirements
-            file.writelines(_database_requirements(project))
+            _database_requirements(project)
+
+        # Write requirements to file
+        file.write("\n".join(project.requirements))
 
 
 def _database_requirements(project):
-    db_req = []
     if project.need_database:
         if project.db_type == "SQL":
-            db_req.append("sqlalchemy\n")
+            project.add_requirements("sqlalchemy")
             if project.db_engine == "Postgres":
                 # Add psycopg2-binary if database engine is Postgres
-                db_req.append("psycopg2-binary\n")
+                project.add_requirements("psycopg2-binary")
             elif project.db_engine == "MySQL":
                 # Add mysql-connector-python if database engine is MySQL
-                db_req.append("mysql-connector-python\n")
+                project.add_requirements("mysql-connector-python")
         elif project.db_type == "NoSQL":
             # Add mongoengine if database type is NoSQL and engine is MongoDB
-            db_req.append("mongoengine") if project.db_engine == "MongoDB" else []
-        return db_req
-    return []
+            project.add_requirements("mongoengine") if project.db_engine == "MongoDB" else None
```

### Comparing `flask_template_cli-0.1.1/flask_template_cli/templates/routes_gen.py` & `flask_template_cli-0.2.0/flask_template_cli/templates/routes_gen.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,25 @@
     if project.project_type == "full_stack":
         _full_stack_routes_gen(project)
     else:
         _api_routes_gen(project)
 
 
 def _full_stack_routes_gen(project):
-    file_location = os.path.join(project.name, "app/routes/routes.py")
+    init_file_location = os.path.join(project.name, "app/routes/__init__.py")
+
+    with open(init_file_location, "w") as f:
+        f.write(f"from .routes import my_routes\n\n")
+        if project.need_auth:
+            f.write(f"from .auth import auth\n\n")
+            _auth_config(project)
+
+    resource_file_location = os.path.join(project.name, "app/routes/routes.py")
 
-    with open(file_location, "w") as f:
+    with open(resource_file_location, "w") as f:
         f.write(f"from flask import Blueprint\n\n")
         f.write(f"my_routes = Blueprint('my_routes', __name__)\n\n")
         f.write(f"""
     @my_routes.route('/')
     def index():  
         return "Hello World"
 
@@ -28,14 +36,17 @@
 
 def _api_routes_gen(project):
     init_file_location = os.path.join(project.name, "app/routes/__init__.py")
 
     with open(init_file_location, "w") as f:
         f.write(f"from flask_restful import Api \n\n\n")
         f.write(f"api = Api(prefix='/api/v1')\n\n")
+        if project.need_auth:
+            f.write(f"from .auth import auth\n\n")
+            _auth_config(project)
 
     resource_file_location = os.path.join(project.name, "app/routes/resources.py")
     with open(resource_file_location, "w") as f:
         f.write(f"from flask_restful import Resource\n\n")
         f.write(f"from . import api\n\n")
         f.write(f"""
 class HelloWorld(Resource):
@@ -43,7 +54,23 @@
         return {{'hello': 'world'}}
             
             """)
 
         f.write(f"\n")
 
         f.write(f"api.add_resource(HelloWorld, '/')\n\n")
+
+
+def _auth_config(project):
+    if project.auth_type == "cookie":
+        return """
+from flask_login import LoginManager
+login_manager = LoginManager()
+            """
+
+    elif project.auth_type == "token":
+        return """
+        
+from flask_jwt_extended import JWTManager
+jwt = JWTManager()
+        
+        """
```

### Comparing `flask_template_cli-0.1.1/flask_template_cli/types.py` & `flask_template_cli-0.2.0/flask_template_cli/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 class Project:
     def __init__(self):
         self._name = None
         self._project_type = None
         self._need_database = False
         self._db_type = None
         self._db_engine = None
+        self._requirements = []
+        self._need_auth = False
+        self._auth_type = None
 
     @property
     def name(self):
         return self._name
 
     @property
     def project_type(self):
@@ -22,14 +25,26 @@
     def db_engine(self):
         return self._db_engine
 
     @property
     def db_type(self):
         return self._db_type
 
+    @property
+    def requirements(self):
+        return self._requirements
+
+    @property
+    def auth_type(self):
+        return self._auth_type
+
+    @property
+    def need_auth(self):
+        return self._need_auth
+
     @name.setter
     def name(self, value):
         self._name = value
 
     @project_type.setter
     def project_type(self, value):
         self._project_type = value
@@ -41,7 +56,18 @@
     @db_engine.setter
     def db_engine(self, value):
         self._db_engine = value
 
     @db_type.setter
     def db_type(self, value):
         self._db_type = value
+
+    @need_auth.setter
+    def need_auth(self, value):
+        self._need_auth = value
+
+    @auth_type.setter
+    def auth_type(self, value):
+        self._auth_type = value
+
+    def add_requirements(self, value):
+        self._requirements.append(value)
```

### Comparing `flask_template_cli-0.1.1/flask_template_cli.egg-info/SOURCES.txt` & `flask_template_cli-0.2.0/flask_template_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,13 @@
 flask_template_cli.egg-info/PKG-INFO
 flask_template_cli.egg-info/SOURCES.txt
 flask_template_cli.egg-info/dependency_links.txt
 flask_template_cli.egg-info/entry_points.txt
 flask_template_cli.egg-info/requires.txt
 flask_template_cli.egg-info/top_level.txt
 flask_template_cli/templates/__init__.py
+flask_template_cli/templates/auth_gen.py
 flask_template_cli/templates/init_gen.py
 flask_template_cli/templates/models_gen.py
 flask_template_cli/templates/req_txt_gen.py
 flask_template_cli/templates/routes_gen.py
 tests/test_cli.py
```

### Comparing `flask_template_cli-0.1.1/setup.cfg` & `flask_template_cli-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flask_template_cli
-version = 0.1.1
+version = 0.2.0
 url = https://github.com/saipraveenkondapalli/flask_template_cli
 author = Sai Praveen Kondapalli
 author_email = saipraveenkondapalli@gmail.com
 description = Description of my package
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `flask_template_cli-0.1.1/tests/test_cli.py` & `flask_template_cli-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

