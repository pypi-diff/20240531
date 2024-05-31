# Comparing `tmp/SerialDBPy-0.1.3.9.tar.gz` & `tmp/SerialDBPy-0.1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerialDBPy-0.1.3.9.tar", last modified: Fri May 31 04:23:06 2024, max compression
+gzip compressed data, was "SerialDBPy-0.1.4.0.tar", last modified: Fri May 31 17:29:15 2024, max compression
```

## Comparing `SerialDBPy-0.1.3.9.tar` & `SerialDBPy-0.1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:23:06.438355 SerialDBPy-0.1.3.9/
--rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.3.9/LICENSE
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 04:23:06.438355 SerialDBPy-0.1.3.9/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)     3853 2024-05-31 03:40:11.000000 SerialDBPy-0.1.3.9/README.md
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:23:06.438355 SerialDBPy-0.1.3.9/SerialDBPy/
--rw-rw-r--   0 swim      (1000) swim      (1000)       37 2024-05-31 04:22:42.000000 SerialDBPy-0.1.3.9/SerialDBPy/__init__.py
--rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 04:22:30.000000 SerialDBPy-0.1.3.9/SerialDBPy/query.py
--rw-rw-r--   0 swim      (1000) swim      (1000)    18356 2024-05-31 04:22:28.000000 SerialDBPy-0.1.3.9/SerialDBPy/serialization.py
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:23:06.438355 SerialDBPy-0.1.3.9/SerialDBPy.egg-info/
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 04:23:06.000000 SerialDBPy-0.1.3.9/SerialDBPy.egg-info/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)      243 2024-05-31 04:23:06.000000 SerialDBPy-0.1.3.9/SerialDBPy.egg-info/SOURCES.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 04:23:06.000000 SerialDBPy-0.1.3.9/SerialDBPy.egg-info/dependency_links.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       11 2024-05-31 04:23:06.000000 SerialDBPy-0.1.3.9/SerialDBPy.egg-info/top_level.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 04:23:06.438355 SerialDBPy-0.1.3.9/setup.cfg
--rw-rw-r--   0 swim      (1000) swim      (1000)      611 2024-05-31 04:22:53.000000 SerialDBPy-0.1.3.9/setup.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 17:29:15.187737 SerialDBPy-0.1.4.0/
+-rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.4.0/LICENSE
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 17:29:15.187737 SerialDBPy-0.1.4.0/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)     3853 2024-05-31 03:40:11.000000 SerialDBPy-0.1.4.0/README.md
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 17:29:15.187737 SerialDBPy-0.1.4.0/SerialDBPy.egg-info/
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 17:29:15.000000 SerialDBPy-0.1.4.0/SerialDBPy.egg-info/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)      252 2024-05-31 17:29:15.000000 SerialDBPy-0.1.4.0/SerialDBPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 17:29:15.000000 SerialDBPy-0.1.4.0/SerialDBPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)       14 2024-05-31 17:29:15.000000 SerialDBPy-0.1.4.0/SerialDBPy.egg-info/top_level.txt
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 17:29:15.187737 SerialDBPy-0.1.4.0/Serialization/
+-rw-rw-r--   0 swim      (1000) swim      (1000)       91 2024-05-31 17:26:33.000000 SerialDBPy-0.1.4.0/Serialization/__init__.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 04:22:30.000000 SerialDBPy-0.1.4.0/Serialization/query.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)    18412 2024-05-31 17:24:41.000000 SerialDBPy-0.1.4.0/Serialization/serialization.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 17:29:15.187737 SerialDBPy-0.1.4.0/setup.cfg
+-rw-rw-r--   0 swim      (1000) swim      (1000)      611 2024-05-31 17:29:00.000000 SerialDBPy-0.1.4.0/setup.py
```

### Comparing `SerialDBPy-0.1.3.9/LICENSE` & `SerialDBPy-0.1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.9/PKG-INFO` & `SerialDBPy-0.1.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.9
+Version: 0.1.4.0
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.9.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.0.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.9/README.md` & `SerialDBPy-0.1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.9/SerialDBPy/query.py` & `SerialDBPy-0.1.4.0/Serialization/query.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.9/SerialDBPy/serialization.py` & `SerialDBPy-0.1.4.0/Serialization/serialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional
 from query import iQuery    
 
 import os
 import uuid
 
-class SerialDBPy(object):
+class Serializable(object):
 
     """
     ** TO DO: for person in [array of Person( input=query result )] Maybe we call this function load()
     ** TO DO: allow variables that shouldnt be included in the map, possibly by putting a _ in front of the name EXAMPLE: self._current = None
 
     1) This object allows any class object to become deserializable into the database, or serialized from the db
     2) How do I use this?
-        - Simply add SerialDBPy as an interited class; call [YOUR_INSTANCE].deserialize_to_db()
+        - Simply add Serializable as an interited class; call [YOUR_INSTANCE].deserialize_to_db()
     
     To-Do: Add __slots__ use; SQL Sanitizer
 
 
 
     INFORMATION:
         Table-related actions should always be @classmethods, unless functionality would be significantly hindered
@@ -52,44 +52,44 @@
         ):
 
         self.default_middleware = middleware_name
         self.default_server = server_name
 
     def _get_vars(self):
 
-        server = getattr(self,'resource_server',SerialDBPy.default_server)
+        server = getattr(self,'resource_server',Serializable.default_server)
         db = getattr(self,'resource_db',None)
         table = getattr(self,'resource_table',None)
         map = getattr(self,'resource_map',{})
-        keys = [ key for key in map if key in SerialDBPy.key_types ]
+        keys = [ key for key in map if key in Serializable.key_types ]
 
         _mapsize = len( map.keys() )
 
         if map is None or _mapsize == 0:
 
             # Let's do default mapping if no map is available
             map = { key:key for key,val in self.__dict__.items() }
 
         elif _mapsize == len( keys ) and len( keys ) > 0:
 
             # if map only contains valid key types
             
             _keys = { key:map.get( key,None ) for key in keys }
 
-            if not SerialDBPy.IGNORE_UNDERSCORE_VARS:
+            if not Serializable.IGNORE_UNDERSCORE_VARS:
 
                 map = { key:key for key,val in self.__dict__.items() }
                 map = { **_keys,**map }
 
-            elif SerialDBPy.IGNORE_UNDERSCORE_VARS and not SerialDBPy.OVERRIDE_UNDERSCORE_WITH_PROPERTY:
+            elif Serializable.IGNORE_UNDERSCORE_VARS and not Serializable.OVERRIDE_UNDERSCORE_WITH_PROPERTY:
 
                 map = { key:key for key,val in self.__dict__.items() if key[0] != '_' }
                 map = { **_keys,**map }                
             
-            elif SerialDBPy.IGNORE_UNDERSCORE_VARS and SerialDBPy.OVERRIDE_UNDERSCORE_WITH_PROPERTY:
+            elif Serializable.IGNORE_UNDERSCORE_VARS and Serializable.OVERRIDE_UNDERSCORE_WITH_PROPERTY:
                 
                 map = { key:key for key,val in self.__dict__.items() if key[0] != '_' }
                 replaced_underscores = { key[1:]:key[1:] for key,val in self.__dict__.items() if key[0] == '_' }
                 map = { **_keys,**map,**replaced_underscores }
 
         return server,db,table,map
     
@@ -156,15 +156,15 @@
         Function that returns keys' col name, var name
         """
 
         server,db,table,map = self._get_vars()
 
         keys = {}
 
-        for key in SerialDBPy.key_types: # key = <pk> or <ck> or <fk> etc...
+        for key in Serializable.key_types: # key = <pk> or <ck> or <fk> etc...
 
             column_name = map.get( key,None ) # Column Name
             var_name = map.get( column_name,None ) # Python Object's Name
 
             if isinstance( column_name,str ):
 
                 keys[key] = var_name # sets col name = var name
@@ -179,15 +179,15 @@
     @property
     @_valid_mapping
     def _key_clauses( self ):
 
         server,db,table,map = self._get_vars()
 
         keys = self._keys()
-        clauses = [ f'{val} = \'{ getattr( self,map[val],None ) }\'' for key,val in keys.items() if key in SerialDBPy.key_types ]
+        clauses = [ f'{val} = \'{ getattr( self,map[val],None ) }\'' for key,val in keys.items() if key in Serializable.key_types ]
 
         return f' WHERE { " AND ".join( clauses ) }'
 
     @_valid_mapping
     def get_from_json( 
         self, 
         data:dict, 
@@ -269,15 +269,15 @@
         
         return output
     
     @classmethod
     @_valid_mapping
     def get_all_from_query( cls,query:str ):
         
-        rows = SerialDBPy.query( sql=query )
+        rows = Serializable.query( sql=query )
 
         return [ cls().get_from_json( data=row ) for row in rows ]
     
     @_valid_mapping
     def get_all( self, **kwargs ):
 
         """
@@ -285,31 +285,31 @@
         Grabs all items
 
         if kwargs are found, use them as WHERE clauses
         """
 
         server,db,table,map = self._get_vars()
 
-        n_map = [ f'{key} as {val}' for key,val in map.items() if key not in SerialDBPy.key_types ]
+        n_map = [ f'{key} as {val}' for key,val in map.items() if key not in Serializable.key_types ]
         columns = ','.join(n_map)
         instances = []
-        sql = f'select distinct {columns} from {self.resource_db}.{SerialDBPy.default_middleware}.{self.resource_table}'
+        sql = f'select distinct {columns} from {self.resource_db}.{Serializable.default_middleware}.{self.resource_table}'
 
         if len( kwargs.items() ) > 0:
-            sql += f' WHERE {SerialDBPy._generate_sql_clauses( filters=kwargs.items() )}'
+            sql += f' WHERE {Serializable._generate_sql_clauses( filters=kwargs.items() )}'
         
         resp = iQuery( ).execute(sql=sql)
 
         for item in resp:
             
             instance = self.__class__( self )
 
             for key,val in item.items():
 
-                if SerialDBPy.OVERRIDE_UNDERSCORE_WITH_PROPERTY and hasattr( instance,f'_{key}'.lower() ):
+                if Serializable.OVERRIDE_UNDERSCORE_WITH_PROPERTY and hasattr( instance,f'_{key}'.lower() ):
                     setattr(instance, f'_{key}'.lower() ,val)
                 else:
                     setattr(instance, f'{key}'.lower() ,val)
 
             instances.append( instance )
            
         return instances
@@ -322,31 +322,31 @@
         Limited to one item
 
         if kwargs are found, use them as WHERE clauses
         """
 
         server,db,table,map = self._get_vars()
 
-        n_map = [ f'{key} as {val}' for key,val in map.items() if key not in SerialDBPy.key_types ]
+        n_map = [ f'{key} as {val}' for key,val in map.items() if key not in Serializable.key_types ]
         columns = ','.join(n_map)
         
-        sql = f'select top 1 {columns} from {db}.{SerialDBPy.default_middleware}.{table}'
-        sql += f' WHERE {SerialDBPy._generate_sql_clauses( filters=kwargs.items() )}' if len( kwargs.items() ) > 0 else self._key_clauses
+        sql = f'select top 1 {columns} from {db}.{Serializable.default_middleware}.{table}'
+        sql += f' WHERE {Serializable._generate_sql_clauses( filters=kwargs.items() )}' if len( kwargs.items() ) > 0 else self._key_clauses
 
         try:
             resp = iQuery( ).execute(sql=sql)
         except Exception as SQLException:
             resp = []
 
         if not isinstance( resp,list ) or ( isinstance( resp,list ) and len(resp) < 1 ) or ( isinstance( resp,list ) and len( resp ) > 0 and not isinstance( resp[0],dict ) ):
             return self
 
         for key,val in resp[0].items():
 
-            if SerialDBPy.OVERRIDE_UNDERSCORE_WITH_PROPERTY and hasattr( self,f'_{key}'.lower() ):
+            if Serializable.OVERRIDE_UNDERSCORE_WITH_PROPERTY and hasattr( self,f'_{key}'.lower() ):
                 setattr(self, f'_{key}'.lower() ,val)
             else:
                 setattr(self, f'{key}'.lower() ,val)
 
             
         return self
 
@@ -357,15 +357,15 @@
         Pivots instance of class into HTML target
 
         :param html: The HTML to which we will serialize
         """
 
         server,db,table,map = self._get_vars()
         
-        vars = [ val for key,val in map.items() if key not in SerialDBPy.key_types ]
+        vars = [ val for key,val in map.items() if key not in Serializable.key_types ]
         override = lambda a : a if a not in vars else getattr( self,a,a )
         new_html = html
 
         for var in vars:
 
             new_html = new_html.replace( f'@{var}@', str( override( var ) ) )
 
@@ -398,22 +398,22 @@
         Deletes the instance from the database
         """
 
         server,db,table,map = self._get_vars()
         
         if not kwargs:
 
-            sql = f'delete from {db}.{SerialDBPy.default_middleware}.{table} {self._key_clauses}'
+            sql = f'delete from {db}.{Serializable.default_middleware}.{table} {self._key_clauses}'
             iQuery().execute( sql=sql )
             return self
 
         else:
 
             clauses = [ f'{key} = {val}' for key,val in kwargs.items() ]
-            sql = f'delete from {db}.{SerialDBPy.default_middleware}.{table} where { " AND ".join( clauses ) }'
+            sql = f'delete from {db}.{Serializable.default_middleware}.{table} where { " AND ".join( clauses ) }'
             iQuery().execute( sql=sql )
 
             return self
 
     @_valid_mapping
     def insert(self):
 
@@ -449,22 +449,22 @@
         """
 
         server,db,table,map = self._get_vars()
         que = []
 
         for key,val in map.items():
 
-            if key not in SerialDBPy.key_types:
+            if key not in Serializable.key_types:
 
                 _val = (f"{getattr(self,val,'')}").replace("'","\\'")
                 que.append( f'{key} = \'{_val}\'' )
 
         val_sql = ', '.join(que)
 
-        return iQuery().execute(sql=f'update {db}.{SerialDBPy.default_middleware}.{table} set {val_sql} {self._key_clauses}') 
+        return iQuery().execute(sql=f'update {db}.{Serializable.default_middleware}.{table} set {val_sql} {self._key_clauses}') 
     
     @_valid_mapping
     def serialize_to_sql(self):
 
         """
         Creates a SQL statement to insert a valid instance of a class into the database
         
@@ -475,27 +475,27 @@
         
         server,db,table,map = self._get_vars()
         n_map:list = []
         columns:list = []
 
         for key,val in map.items():
 
-            if key not in SerialDBPy.key_types:
+            if key not in Serializable.key_types:
 
                 n_val = (f"{getattr(self,val,'')}").replace("'","\\'")
                 if n_val != 'None':
                     n_map.append( f"'{n_val}'" )
                 else:
                     n_map.append( "''" )
                 columns.append(f"{key}") # key = col name; surround by '' 
         
         col_sql = ','.join(columns)
         val_sql = ','.join(n_map)
 
-        return f'insert into {db}.{SerialDBPy.default_middleware}.{table} ({col_sql}) values ({val_sql})'
+        return f'insert into {db}.{Serializable.default_middleware}.{table} ({col_sql}) values ({val_sql})'
         
     @_valid_mapping
     def generate_primary_key(self,length:int = 10):
 
         """
         Queries object from db and serializes it into an instance of the parent class
         """
@@ -506,15 +506,15 @@
             
             """
             generates primary keys
             """
             
             if key == '<pk>':
 
-                setattr(self,str(key).lower(), SerialDBPy._uuid( length=length ) )
+                setattr(self,str(key).lower(), Serializable._uuid( length=length ) )
 
         return self
     
     @staticmethod
     def _generate_sql_clauses( filters:dict ):
 
         clause_parts = []
```

### Comparing `SerialDBPy-0.1.3.9/SerialDBPy.egg-info/PKG-INFO` & `SerialDBPy-0.1.4.0/SerialDBPy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.9
+Version: 0.1.4.0
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.9.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.0.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.9/setup.py` & `SerialDBPy-0.1.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SerialDBPy',
-    version='0.1.3.9',
+    version='0.1.4.0',
     author='G',
     author_email='serialdbpy@swimhdr.com',
     description='Lightweight Python ORM for basic CRUD operations.',
     license='MIT',
     url = 'https://github.com/publicsignal',
-    download_url='https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.9.tar.gz',
+    download_url='https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.0.tar.gz',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

