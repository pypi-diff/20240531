# Comparing `tmp/datonius-0.2.0.tar.gz` & `tmp/datonius-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datonius-0.2.0.tar", last modified: Tue Aug 16 07:44:37 2022, max compression
+gzip compressed data, was "datonius-1.2.0.tar", last modified: Fri May 31 03:58:01 2024, max compression
```

## Comparing `datonius-0.2.0.tar` & `datonius-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-16 07:44:37.000000 datonius-0.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      273 2022-08-16 04:18:46.000000 datonius-0.2.0/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-16 07:44:37.000000 datonius-0.2.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2022-08-16 04:18:47.000000 datonius-0.2.0/tests/test_datonius.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2022-08-16 04:18:47.000000 datonius-0.2.0/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24458 2022-08-16 07:23:09.000000 datonius-0.2.0/datonius/datonius.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      471 2022-08-16 04:18:41.000000 datonius-0.2.0/datonius/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4942 2022-08-16 04:18:41.000000 datonius-0.2.0/datonius/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1060 2022-08-16 07:44:37.000000 datonius-0.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2022-08-16 07:44:28.000000 datonius-0.2.0/HISTORY.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-16 07:44:37.000000 datonius-0.2.0/docs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4993 2022-08-16 04:18:44.000000 datonius-0.2.0/docs/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2022-08-16 04:18:44.000000 datonius-0.2.0/docs/contributing.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2022-08-16 04:18:45.000000 datonius-0.2.0/docs/make.bat
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1207 2022-08-16 04:18:45.000000 datonius-0.2.0/docs/installation.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       28 2022-08-16 04:18:45.000000 datonius-0.2.0/docs/readme.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2022-08-16 04:18:45.000000 datonius-0.2.0/docs/usage.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      629 2022-08-16 04:18:45.000000 datonius-0.2.0/docs/Makefile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2022-08-16 04:18:44.000000 datonius-0.2.0/docs/history.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2022-08-16 04:18:45.000000 datonius-0.2.0/docs/index.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2022-08-16 04:18:44.000000 datonius-0.2.0/docs/authors.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      391 2022-08-16 07:44:37.000000 datonius-0.2.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      101 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1060 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      570 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-08-16 07:44:37.000000 datonius-0.2.0/datonius.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2022-08-16 04:18:40.000000 datonius-0.2.0/AUTHORS.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3687 2022-08-16 04:18:41.000000 datonius-0.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1622 2022-08-16 07:42:44.000000 datonius-0.2.0/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      123 2022-08-16 04:18:46.000000 datonius-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:58:01.646739 datonius-1.2.0/
+-rw-rw-rw-   0        0        0      175 2024-05-10 02:08:28.000000 datonius-1.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3687 2024-05-10 02:08:28.000000 datonius-1.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      573 2024-05-31 03:53:35.000000 datonius-1.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0      273 2024-05-10 02:08:28.000000 datonius-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1588 2024-05-31 03:58:01.642746 datonius-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2024-05-10 02:08:28.000000 datonius-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:58:01.459324 datonius-1.2.0/datonius/
+-rw-rw-rw-   0        0        0      471 2024-05-10 02:08:38.000000 datonius-1.2.0/datonius/__init__.py
+-rw-rw-rw-   0        0        0     6522 2024-05-31 03:50:36.000000 datonius-1.2.0/datonius/cli.py
+-rw-rw-rw-   0        0        0    25916 2024-05-31 03:50:36.000000 datonius-1.2.0/datonius/datonius.py
+-rw-rw-rw-   0        0        0     2903 2024-05-31 03:50:36.000000 datonius-1.2.0/datonius/ontology.py
+-rw-rw-rw-   0        0        0     2983 2024-05-31 03:50:36.000000 datonius-1.2.0/datonius/util.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:58:01.635733 datonius-1.2.0/datonius.egg-info/
+-rw-rw-rw-   0        0        0     1588 2024-05-31 03:58:01.000000 datonius-1.2.0/datonius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2024-05-31 03:58:01.000000 datonius-1.2.0/datonius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:58:01.000000 datonius-1.2.0/datonius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:58:01.000000 datonius-1.2.0/datonius.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 02:08:38.000000 datonius-1.2.0/datonius.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      132 2024-05-31 03:58:01.000000 datonius-1.2.0/datonius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 03:58:01.000000 datonius-1.2.0/datonius.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 03:58:01.574936 datonius-1.2.0/docs/
+-rw-rw-rw-   0        0        0      629 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-10 02:08:38.000000 datonius-1.2.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4993 2024-05-31 03:50:36.000000 datonius-1.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/history.rst
+-rw-rw-rw-   0        0        0      335 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1207 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       88 2024-05-10 02:08:39.000000 datonius-1.2.0/docs/usage.rst
+-rw-rw-rw-   0        0        0      416 2024-05-31 03:58:01.650757 datonius-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1732 2024-05-31 03:53:10.000000 datonius-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:58:01.620784 datonius-1.2.0/tests/
+-rw-rw-rw-   0        0        0       39 2024-05-10 02:08:39.000000 datonius-1.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1710 2024-05-31 03:50:36.000000 datonius-1.2.0/tests/test_datonius.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datonius-0.2.0/datonius/datonius.py` & `datonius-1.2.0/datonius/datonius.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Main module."""
 
 # from peewee import AutoField
-from peewee import SqliteDatabase, Field, Model, CharField, TextField, IntegerField, ForeignKeyField, DateField, DatabaseProxy, PostgresqlDatabase
+from peewee import SqliteDatabase, Field, Model, CharField, TextField, IntegerField, ForeignKeyField, DateField, DatabaseProxy, PostgresqlDatabase, ProgrammingError
 from os import environ
 from itertools import chain
 from contextlib import contextmanager
 from datetime import timedelta
 from pathlib import Path
 from sys import stderr
 
+import logging
+
 from . import __version__
 
 
 database_proxy = DatabaseProxy()
 # database = MssqlDatabase('ORDSS_FACTS_GIMS', host=environ.get("DATONIUS_DB", 'csvcesrv014.fda.gov'), user=environ.get("DATONIUS_USER") or input("Enter username credential for Datonius DB:"), password=environ.get("DATONIUS_PASS") or input("Enter password:"))
 
 
@@ -257,15 +259,15 @@
 
 class Sample(BaseModel):
 
     oradss_id=IntegerField(unique=True)
 
 
     collection_date = DateField(null=True) # breaking my own rule, here, and not normalizing out a 'Collection' type
-    collection_date_accuracy_mask = TimedeltaField(null=True) # an idea I've been kicking around with Nabil-Fareed Alikhan
+    collection_date_accuracy_mask = TimedeltaField(default=timedelta(0)) # an idea I've been kicking around with Nabil-Fareed Alikhan
     collection_method = CharField(null=True)
     collection_remarks = TextField(default="", null=True)
     collection_reason = TextField(default="", null=True)
 
     sample_description = TextField(null=True)
     product_description = TextField(null=True)
 
@@ -294,15 +296,16 @@
 
     @staticmethod
     def of(name):
         return SampleName.lookup(name)
 
     @property
     def collected_date_range(self):
-        return self.collection_date - self.collection_date_accuracy_mask, self.collection_date + self.collection_date_accuracy_mask
+        if self.isolation_date is not null:
+            return self.collection_date - self.collection_date_accuracy_mask, self.collection_date + self.collection_date_accuracy_mask
 
     @property
     def barcode(self):
         return self.name_in(Namespace.GIMS_BARCODES)
 
     @property
     def firms(self):
@@ -335,18 +338,26 @@
     firm = ForeignKeyField(Firm, null=False, backref='sample_relationships')
     relationship_code = CharField(null=True)
     responsibility = IntegerField(null=False, default=0)
 
 
 class Isolate(BaseModel):
 
-    gims_pk = IntegerField(unique=True)
+    gims_pk = IntegerField(unique=True) # need to make this less than a key now
     sample = ForeignKeyField(Sample)
     _taxonomy = ForeignKeyField(Taxon, backref='_isolates', null=True) # this field is worth hiding a little
 
+    isolation_date = DateField(null=True) # breaking my own rule, here, and not normalizing out a 'Collection' type
+    isolation_date_accuracy_mask = TimedeltaField(default=timedelta(0)) # an idea I've been kicking around with Nabil-Fareed Alikhan
+
+    @property
+    def isolation_date_range(self):
+        if self.isolation_date is not null:
+            return self.isolation_date - self.isolation_date_accuracy_mask, self.isolation_date + self.isolation_date_accuracy_mask
+
     @property
     def binomial(self):
         return self._taxonomy.binomial
 
     #convenience property to expose an iterator over the taxonomic chain
 
     @property
@@ -512,29 +523,33 @@
         "Really easy to implement a universal name lookup this way."
         name = cls.get_or_none(cls.name == name)
         if name:
             return name.isolate
 
 @contextmanager
 def make_connection(path=None):
+    log = logging.getLogger("datonius")
     if path:
-        if ":memory:" in path:
+        log.info(f"Found path {path}")
+        if ":memory:" not in path:
             path = str(Path(path).absolute())
         database = SqliteDatabase(path, pragmas=dict(journal_mode='wal', foreign_keys=1, cache_size=10000))
     else:
         # database = MssqlDatabase('ORDSS_FACTS_GIMS', 
         #                          host=environ.get("DATONIUS_DB", 'csvcesrv014.fda.gov'), 
         #                          user=environ.get("DATONIUS_USER") or input("Enter username credential for Datonius DB:"), 
         #                          password=environ.get("DATONIUS_PASS") or input("Enter password:")
         #                          )
 
         host = environ.get('DATONIUS_DB', 'localhost').strip()
-        user = environ.get('DATONIUS_USER' or '').strip()
-        passwd = environ.get('DATONIUS_PASS' or '').strip()
-        port = environ.get('DATONIUS_PORT' or 5432)
+        user = environ.get('DATONIUS_USER', '').strip()
+        passwd = environ.get('DATONIUS_PASS', '').strip()
+        port = environ.get('DATONIUS_PORT', 5432)
+
+        log.info(f"Found host={host}, user={user}, port={port}, and password of length {len(passwd)}")
 
         if False: # "amazonaws" in host:
             region = environ.get('DATONIUS_AWS_REGION' or 'us-east-1a')
             cert = environ.get('DATONIUS_SSL_CERTIFICATE' or False)
             if not cert:
                 raise ValueError('''can't connect to AWS RDS; path to SSL certificate not set (see 'https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.SSL.html'.)''')
             try:
@@ -552,26 +567,40 @@
                     user=user,
                     password=passwd,
                     port=port,
                     ssl_ca=cert
                 )
         else:
             database = PostgresqlDatabase(
-                    'Datonius',
+                    'datoniusdb',
                     host=host,
                     user=user,
                     password=passwd,
                     port=port,
                 )
-    database_proxy.initialize(database)
-    database_proxy.connect()
-    database_proxy.create_tables([Address, Country, Firm, Taxon, Isolate, State, Sample, Namespace, SampleName, IsolateName, FirmSampleRelationship])
+
     try:
+        database_proxy.initialize(database)
+        database_proxy.connect()
+        database_proxy.session_start()
+        try:
+            database_proxy.create_tables([Address, Country, Firm, Taxon, Isolate, State, Sample, Namespace, SampleName, IsolateName, FirmSampleRelationship])
+        except ProgrammingError as e:
+            try:
+                import psycopg2
+                if hasattr(e, '__context__') and isinstance(e.__context__, psycopg2.errors.InsufficientPrivilege):
+                    log.getChild("psycopg").warning(e.__context__)
+            except ImportError:
+                pass
+            log.getChild("peewee").warning("Wasn't able to ensure table creation, but they may already be created")
+            database_proxy.session_rollback()
+            database_proxy.session_start()
         yield database_proxy
     finally:
+        database_proxy.session_commit()
         database_proxy.close()
 
 # Set up fixtures and constants
 
 # Taxon.of('Listeria', 'monocytogenes')
 # sal = Taxon.of('Salmonella', 'enterica', subspecies='enterica', serovar='Javiana')
 # sal = Taxon.of('Salmonella', 'enterica', subspecies="enterica")
```

### Comparing `datonius-0.2.0/datonius/cli.py` & `datonius-1.2.0/datonius/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import click
 
 import simplejson
 
 import functools
+import logging
 
 from tabulate import tabulate
 from datonius import *
+import datonius.util as util
 from peewee import DoesNotExist
 
 @click.group()
 @click.option('-d', '--db', 'database', default=None, metavar='PATH', help='path to a Datonius database in SQLite format.')
+@click.option('-v', '--verbose', count=True)
 @click.pass_context
-def cli(ctx, database):
+def cli(ctx, database, verbose):
     ctx.ensure_object(dict)
     ctx.obj['database'] = database
+    log_level = {0:60, 1:30, 2:20, 3:10}[verbose]
+    logging.basicConfig(level=log_level,
+                        format='[%(asctime)s][%(name)-12s][%(levelname)-8s] %(message)s',
+                        datefmt='%m-%d %H:%M')
 
 
 def first_value_or_default(iterable, default=None):
     try:
         return next(iter(iterable))
     except StopIteration:
         class DefaultEmptyObject:
@@ -72,41 +79,66 @@
 table = functools.partial(tabulate, headers='keys', tablefmt='simple')
 tsv = functools.partial(tabulate, headers='keys', tablefmt='tsv')
 json = functools.partial(simplejson.dumps, indent=2, iterable_as_array=True)
 
 @cli.command()
 @click.argument('names', nargs=-1, metavar="NAME")
 @click.option('-o', '--output', type=click.File('wt'), default=click.get_text_stream('stdout'))
-@click.option('-h', '--human-readable', 'output_format', flag_value=table, help='Output in a human-readable table.', default=table)
-@click.option('-j', '--json', 'output_format', flag_value=json, help='Output in JSON.')
-@click.option('-t', '--tsv', 'output_format', flag_value=tsv, help='output in TSV format.')
+@click.option('-h', '--human-readable', 'output_format', flag_value=util.TABLE, help='Output in a human-readable table.', default=util.TABLE)
+@click.option('-j', '--json', 'output_format', flag_value=util.JSON, help='Output in JSON.')
+@click.option('-t', '--tsv', 'output_format', flag_value=util.TSV, help='output in TSV format.')
 @click.option('-a', '--all-fields', flag_value=True, default=False)
 @click.pass_context
 def lookup(ctx, names, output, output_format, all_fields=False):
     "Lookup a name and retreive isolate information."
-    use_full_data = all_fields or output_format is json
-    if output_format is table and output is not click.get_text_stream('stdout'):
-        output_format = tsv # coerce to TSV if we're going to a file
-    with make_connection(ctx.obj['database']):
-        click.echo(output_format([isolate_to_dict(name, Isolate.of(name), use_full_data) for name in names]), file=output)
+    if output_format is util.TABLE and output is not click.get_text_stream('stdout'):
+        output_format = util.TSV # coerce to TSV if we're going to a file
+    try:
+        with make_connection(ctx.obj['database']):
+            click.echo(util.lookup(names, output_format, all_fields) or f"{names} not found.", file=output)
+    except Exception as e:
+        click.echo(str(e), err=True)
+        exit(1)
 
 @cli.command()
 @click.argument('names', nargs=-1, metavar="TAXON")
 @click.option('-o', '--output', type=click.File('wt'), default=click.get_text_stream('stdout'))
-@click.option('-h', '--human-readable', 'output_format', flag_value=table, help='Output in a human-readable table.', default=table)
-@click.option('-j', '--json', 'output_format', flag_value=json, help='Output in JSON.')
-@click.option('-t', '--tsv', 'output_format', flag_value=tsv, help='output in TSV format.')
+@click.option('-h', '--human-readable', 'output_format', flag_value=util.TABLE, help='Output in a human-readable table.', default=util.TABLE)
+@click.option('-j', '--json', 'output_format', flag_value=util.JSON, help='Output in JSON.')
+@click.option('-t', '--tsv', 'output_format', flag_value=util.TSV, help='output in TSV format.')
 @click.option('-a', '--all-fields', flag_value=True, default=False)
 @click.pass_context
 def tax(ctx, names, output, output_format, all_fields=False):
     "Lookup a taxon and retreive information for its isolates."
-    use_full_data = all_fields or output_format is json
-    if output_format is table and output is not click.get_text_stream('stdout'):
-        output_format = tsv # coerce to TSV if we're going to a file
+    if output_format is util.TABLE and output is not click.get_text_stream('stdout'):
+        output_format = util.TSV # coerce to TSV if we're going to a file
     with make_connection(ctx.obj['database']):
         try:
-            click.echo(output_format((isolate_to_dict(names[-1], iso, use_full_data) for iso in Taxon.get(name=names[-1]).isolates)), file=output)
+            click.echo(util.tax(names, output_format, all_fields), file=output)
         except DoesNotExist:
-            click.echo(f"{' '.join(names)} isn't a taxon in the database.")
+            click.echo(f"{' '.join(names)} isn't a taxon in the database.", err=True)
+            exit(1)
+        except Exception as e:
+            click.echo(str(e), err=True)
+            exit(1)
+
+@cli.command()
+@click.argument('names', nargs=1, metavar="ONTOLOGY TERM")
+@click.option('-o', '--output', type=click.File('wt'), default=click.get_text_stream('stdout'))
+@click.option('-h', '--human-readable', 'output_format', flag_value=util.TABLE, help='Output in a human-readable table.', default=util.TABLE)
+@click.option('-j', '--json', 'output_format', flag_value=util.JSON, help='Output in JSON.')
+@click.option('-t', '--tsv', 'output_format', flag_value=util.TSV, help='output in TSV format.')
+@click.option('-a', '--all-fields', flag_value=True, default=False)
+@click.pass_context
+def ontology(ctx, names, output, output_format, all_fields=False):
+    "Find isolates according to one or more ontology terms from the FOODON ontology."
+    if output_format is util.TABLE and output is not click.get_text_stream('stdout'):
+        output_format = util.TSV # coerce to TSV if we're going to a file
+    with make_connection(ctx.obj['database']):
+        try:
+            click.echo(util.ontology(names, output_format, all_fields), file=output)
+        except Exception as e:
+            click.echo(str(e), err=True)
+            exit(1)
 
 if __name__ == '__main__':
     cli(obj={})
```

### Comparing `datonius-0.2.0/docs/conf.py` & `datonius-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datonius-0.2.0/docs/make.bat` & `datonius-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datonius-0.2.0/docs/installation.rst` & `datonius-1.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `datonius-0.2.0/docs/Makefile` & `datonius-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datonius-0.2.0/datonius.egg-info/SOURCES.txt` & `datonius-1.2.0/datonius.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 datonius/__init__.py
 datonius/cli.py
 datonius/datonius.py
+datonius/ontology.py
+datonius/util.py
 datonius.egg-info/PKG-INFO
 datonius.egg-info/SOURCES.txt
 datonius.egg-info/dependency_links.txt
 datonius.egg-info/entry_points.txt
 datonius.egg-info/not-zip-safe
 datonius.egg-info/requires.txt
 datonius.egg-info/top_level.txt
```

### Comparing `datonius-0.2.0/CONTRIBUTING.rst` & `datonius-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `datonius-0.2.0/setup.py` & `datonius-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = [ 'peewee==3.14.4',
+requirements = [ 'peewee~=3.14.4',
                  'psycopg2-binary~=2.9.3',
-                 'boto3==1.17.53',
-                 'tabulate==0.8.9',
-                 'click==7.1.2',
-                 'simplejson==3.17.2',
+                 'boto3~=1.17.53',
+                 'tabulate~=0.8.9',
+                 'click~=7.1.2',
+                 'simplejson~=3.17.2',
+                 #'owlready2~=0.37',
+                 'requests~=2.28.0',
+                 'rdflib~=6.3.2'
                 ]
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
@@ -41,15 +44,15 @@
     keywords='datonius',
     name='datonius',
     packages=find_packages(include=['datonius', 'datonius.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/crashfrog/datonius',
-    version="0.2.0",
+    version="1.2.0",
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'dtns=datonius.cli:cli'
         ]
     }
 )
```

