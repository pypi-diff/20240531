# Comparing `tmp/mo_sql_parsing-9.640.24141.tar.gz` & `tmp/mo_sql_parsing-9.642.24144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_sql_parsing-9.640.24141.tar", last modified: Mon May 20 16:35:41 2024, max compression
+gzip compressed data, was "mo_sql_parsing-9.642.24144.tar", last modified: Thu May 23 01:45:36 2024, max compression
```

## Comparing `mo_sql_parsing-9.640.24141.tar` & `mo_sql_parsing-9.642.24144.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/
--rw-rw-rw-   0        0        0    15922 2024-05-13 01:12:26.000000 mo_sql_parsing-9.640.24141/LICENSE
--rw-rw-rw-   0        0        0    10151 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/PKG-INFO
--rw-rw-rw-   0        0        0     8521 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 16:35:41.372149 mo_sql_parsing-9.640.24141/mo_sql_parsing/
--rw-rw-rw-   0        0        0     6723 2024-05-14 02:14:17.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/__init__.py
--rw-rw-rw-   0        0        0    25509 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/formatting.py
--rw-rw-rw-   0        0        0    11503 2024-05-14 02:14:17.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/keywords.py
--rw-rw-rw-   0        0        0    43041 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/sql_parser.py
--rw-rw-rw-   0        0        0     8811 2024-05-14 02:14:17.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/types.py
--rw-rw-rw-   0        0        0    24893 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/utils.py
--rw-rw-rw-   0        0        0     2949 2024-05-13 01:12:26.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/
--rw-rw-rw-   0        0        0    10151 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-03 00:09:26.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/setup.cfg
--rw-rw-rw-   0        0        0    10158 2024-05-20 16:35:35.000000 mo_sql_parsing-9.640.24141/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:45:36.110791 mo_sql_parsing-9.642.24144/
+-rw-rw-rw-   0        0        0    15922 2024-05-13 01:12:26.000000 mo_sql_parsing-9.642.24144/LICENSE
+-rw-rw-rw-   0        0        0    10151 2024-05-23 01:45:36.110791 mo_sql_parsing-9.642.24144/PKG-INFO
+-rw-rw-rw-   0        0        0     8521 2024-05-23 01:43:55.000000 mo_sql_parsing-9.642.24144/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 01:45:36.074627 mo_sql_parsing-9.642.24144/mo_sql_parsing/
+-rw-rw-rw-   0        0        0     6723 2024-05-14 02:14:17.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing/__init__.py
+-rw-rw-rw-   0        0        0    25509 2024-05-23 01:43:55.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing/formatting.py
+-rw-rw-rw-   0        0        0    11503 2024-05-14 02:14:17.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing/keywords.py
+-rw-rw-rw-   0        0        0    44403 2024-05-23 01:45:28.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing/sql_parser.py
+-rw-rw-rw-   0        0        0     8844 2024-05-23 01:45:28.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing/types.py
+-rw-rw-rw-   0        0        0    25655 2024-05-23 01:45:28.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing/utils.py
+-rw-rw-rw-   0        0        0     2949 2024-05-13 01:12:26.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:45:36.109580 mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/
+-rw-rw-rw-   0        0        0    10151 2024-05-23 01:45:36.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2024-05-23 01:45:36.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 01:45:36.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-05-23 01:45:36.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 01:45:36.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-03 00:09:26.000000 mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-23 01:45:36.110791 mo_sql_parsing-9.642.24144/setup.cfg
+-rw-rw-rw-   0        0        0    10158 2024-05-23 01:45:31.000000 mo_sql_parsing-9.642.24144/setup.py
```

### Comparing `mo_sql_parsing-9.640.24141/LICENSE` & `mo_sql_parsing-9.642.24144/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.640.24141/PKG-INFO` & `mo_sql_parsing-9.642.24144/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.640.24141
+Version: 9.642.24144
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_sql_parsing-9.640.24141/README.md` & `mo_sql_parsing-9.642.24144/README.md`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing/__init__.py` & `mo_sql_parsing-9.642.24144/mo_sql_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing/formatting.py` & `mo_sql_parsing-9.642.24144/mo_sql_parsing/formatting.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing/keywords.py` & `mo_sql_parsing-9.642.24144/mo_sql_parsing/keywords.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing/sql_parser.py` & `mo_sql_parsing-9.642.24144/mo_sql_parsing/sql_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     mysql_string = regex_string | ansi_string | mysql_doublequote_string
     atomic_ident = mysql_backtick_ident | sqlserver_ident | ident_w_dash_warning
     return parser(mysql_string, atomic_ident, all_columns=all_columns)
 
 
 def sqlserver_parser(all_columns):
-    atomic_ident = ansi_ident | mysql_backtick_ident | sqlserver_ident | simple_ident
+    atomic_ident = ansi_ident | mysql_backtick_ident | sqlserver_ident | sqlserver_local_ident
     return parser(regex_string | ansi_string, atomic_ident, sqlserver=True, all_columns=all_columns)
 
 
 def bigquery_parser(all_columns):
     mysql_string = regex_string | ansi_string | mysql_doublequote_string
     atomic_ident = ansi_ident | mysql_backtick_ident | ident_w_dash
     return parser(mysql_string, atomic_ident, all_columns=all_columns)
@@ -723,15 +723,17 @@
                 Optional(keyword("or") + flag("replace"))(INDEX | KEY)
                 + Optional((keyword("if not exists") / False)("replace"))
                 + identifier("name")
             ),
         )
 
         use_schema = assign("use", identifier)
-
+        open_cursor = assign("open", identifier)
+        close_cursor = assign("close", identifier)
+        fetch_cursor = assign("fetch", identifier) + INTO + delimited_list(ident)
         cache_options = Optional((
             keyword("options").suppress()
             + LB
             + Dict(delimited_list(Group(
                 literal_string / (lambda tokens: tokens[0]["literal"]) + Optional(EQ) + identifier
             )))
             + RB
@@ -744,36 +746,47 @@
             + identifier("name")
             + cache_options
             + Optional(AS + query("query"))
         )("cache")
 
         drops = assign(
             "drop",
-            MatchFirst([
+            temporary
+            +MatchFirst([
                 keyword(item).suppress() + Optional(flag("if exists")) + Group(identifier)(item)
                 for item in ["table", "view", "index", "schema"]
             ]),
         )
 
         returning = Optional(delimited_list(select_column)("returning"))
 
         insert = (
             Optional(assign("with", with_clause))
             + keyword("insert").suppress()
+            + Optional(flag("ignore"))
             + (
                 flag("overwrite") + keyword("table").suppress()
                 | keyword("into").suppress() + Optional(keyword("table").suppress())
             )
             + identifier("table")
             + Optional(LB + delimited_list(identifier)("columns") + RB)
             + Optional(flag("if exists"))
             + (values | query)("query")
             + returning
         ) / to_insert_call
 
+        replace = (
+            Optional(assign("with", with_clause))
+            + keyword("replace").suppress()
+            + Optional(keyword("into").suppress())
+            + identifier("table")
+            + Optional(LB + delimited_list(identifier)("columns") + RB)
+            + (values | query)("query")
+        ) / to_replace_call
+
         update = (
             keyword("update")("op")
             + (delimited_list(table_source) + ZeroOrMore(join))("params")
             + assign("set", Dict(delimited_list(Group(identifier + EQ + expression))))
             + Optional((FROM + delimited_list(table_source) + ZeroOrMore(join))("from"))
             + Optional(WHERE + expression("where"))
             + Optional(ORDER_BY + delimited_list(Group(sort_column))("orderby"))
@@ -870,14 +883,15 @@
                 + RB
             )
         )
 
         #############################################################
         # GET/SET
         #############################################################
+        statement = Forward()
         special_ident = keyword("masking policy") | identifier / (lambda t: t[0].lower())
         declare_variable = assign("declare", column_definition)
         set_one_variable = SET + (
             (special_ident + Optional(EQ) + expression)
             / (lambda t: {t[0].lower(): t[1].lower() if isinstance(t[1], str) else t[1]})
         )("set")
         set_variables = SET + delimited_list((
@@ -929,15 +943,14 @@
                 | unset_one_variable
                 | assign("drop", column_option | special_ident)
                 | Optional(keyword("set")) + column_option
             )
         ))
 
         # EXPLAIN
-        statement = Forward()
         explain_option = MatchFirst([
             (
                 Keyword(option, caseless=True)
                 + Optional(EQ)
                 + (
                     TRUE
                     | FALSE
@@ -1012,22 +1025,32 @@
         )
 
         #############################################################
         # USER FUNCTIONS
         #############################################################
 
         many_command = Forward()
-        block = Group(Optional(identifier("label") + ":") + BEGIN + Group(many_command)("block") + END)
+        block = BEGIN + Group(many_command)("block") + END
         if_block = (
             assign("if", expression)
             + assign("then", many_command)
             + Optional(assign("else", many_command))
             + keyword("end if").suppress()
         )
         leave = assign("leave", identifier)
+        while_block = (
+            assign("while", expression)
+            + assign("do", many_command)
+            + keyword("end while").suppress()
+        )
+        loop_block = (
+            keyword("loop").suppress()
+            + many_command("loop")
+            + keyword("end loop").suppress()
+        )
 
         create_trigger = assign(
             "create trigger",
             (
                 identifier("name")
                 + MatchFirst([keyword(k) for k in ["before", "after"]])("when")
                 + MatchFirst([keyword(k) for k in ["insert", "update", "delete"]])("event")
@@ -1052,15 +1075,15 @@
 
         create_procedure = Group(
             CREATE
             + definer
             + keyword("procedure")
             + identifier("name")
             + LB
-            + Group(delimited_list(proc_param))("params")
+            + Group(Optional(delimited_list(proc_param)))("params")
             + RB
             + characteristic
             + statement("body")
         )("create_procedure")
 
         create_function = Group(
             CREATE
@@ -1088,47 +1111,66 @@
             keyword("declare")
             + Group(keyword("continue") | keyword("exit") | keyword("undo"))("action")
             + keyword("handler for")
             + delimited_list(handler_condition)("conditions")
             + statement("body")
         )("declare_handler")
 
+        declare_cursor = Group(
+            keyword("declare").suppress()
+            + identifier("name")
+            + keyword("cursor for").suppress()
+            + query("query")
+        )("declare_cursor")
+
+
         transact = (
             Group(keyword("start transaction")("op")) / to_json_call
             | Group(keyword("commit")("op")) / to_json_call
             | Group(keyword("rollback")("op")) / to_json_call
         )
 
-        flow = block | if_block | leave | assign("return", expression)
+        blocks = Group(Optional(identifier("label") + ":") + (
+            block
+            | if_block
+            | while_block
+            | loop_block
+        ))
 
         #############################################################
         # FINALLY ASSEMBLE THE PARSER
         #############################################################
 
         with NO_WHITESPACE:
             delimiter_command = assign("delimiter", Regex(r"[^\n]+") / (lambda t: t[0].strip()))
 
         set_parser_names()
 
         debugger.__enter__()
 
         statement << Group(
             query
-            | (insert | update | delete | merge | truncate | use_schema)
+            | (insert | replace | update | delete | merge | truncate | use_schema)
             | (create_table | create_view | create_cache | create_index | create_schema)
             | drops
             | (copy | alter)
             | create_trigger
             | create_procedure
             | create_function
             | explain
             | delimiter_command
             | declare_hanlder
-            | flow
+            | declare_cursor
+            | leave
+            | assign("return", expression)
             | transact
+            | open_cursor
+            | close_cursor
+            | fetch_cursor
+            | blocks
             | (Optional(keyword("alter session")).suppress() + (set_variables | unset_one_variable | declare_variable))
         )
 
         many_command << (
             ZeroOrMore(delimiter_pattern)
             + Optional(statement)
             + ZeroOrMore(OneOrMore(delimiter_pattern) + Optional(statement))
```

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing/types.py` & `mo_sql_parsing-9.642.24144/mo_sql_parsing/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,17 +160,17 @@
     DOUBLE,
     FLOAT64,
     BIGNUMERIC,
     BIGDECIMAL,
     FLOAT,
     GEOMETRY,
     MAP_TYPE,
+    INT,
     INTEGER,
     INTERVAL,
-    INT,
     INT32,
     INT64,
     BYTEINT,
     JSON,
     NCHAR,
     NVARCHAR,
     NUMBER,
@@ -261,14 +261,15 @@
         | assign("collate", Optional(EQ) + identifier)
         | flag("primary key")
         | column_def_identity("identity")
         | column_def_references
         | assign("check", LB + expr + RB)
         | assign("default", expr)
         | assign("on update", expr)
+        | (EQ + expr)("default")
     )
 
     column_definition << Group(
         identifier("name") + (column_type | identifier("type")) + ZeroOrMore(column_options)
     ) / to_flat_column_type
 
     set_parser_names()
```

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing/utils.py` & `mo_sql_parsing-9.642.24144/mo_sql_parsing/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -686,14 +686,32 @@
                 return Call("insert", [tokens["table"]], {"values": values, **options})
     except Exception:
         pass
 
     return Call("insert", [tokens["table"]], {"columns": columns, "query": query, **options})
 
 
+def to_replace_call(tokens):
+    options = {k: v for k, v in tokens.items() if k not in ["columns", "table", "query"]}
+    query = tokens["query"]
+    columns = tokens["columns"]
+    try:
+        values = query["from"]["literal"]
+        if values:
+            if columns:
+                data = [dict(zip(columns, row)) for row in values]
+                return Call("replace", [tokens["table"]], {"values": data, **options})
+            else:
+                return Call("replace", [tokens["table"]], {"values": values, **options})
+    except Exception:
+        pass
+
+    return Call("replace", [tokens["table"]], {"columns": columns, "query": query, **options})
+
+
 def to_update_call(tokens):
     value = tokens["value"]
     name = tokens["name"]
     if name:
         value = {"name": name, "value": value}
     set = tokens["set"]
     frum = tokens["from"]
@@ -891,7 +909,8 @@
 
 digit = Char("0123456789")
 with whitespaces.NO_WHITESPACE:
     ident_w_dash = Char(FIRST_IDENT_CHAR) + (Regex("(?<=[^ 0-9])\\-(?=[^ 0-9])") | Char(IDENT_CHAR))[...]
     ident_w_dash_warning = Regex(ident_w_dash.__regex__()[1]).set_parser_name("identifier_with_dashes") / no_dashes
 
 simple_ident = Word(FIRST_IDENT_CHAR, IDENT_CHAR).set_parser_name("identifier")
+sqlserver_local_ident = Word("@" + FIRST_IDENT_CHAR, IDENT_CHAR).set_parser_name("identifier")
```

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing/windows.py` & `mo_sql_parsing-9.642.24144/mo_sql_parsing/windows.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/PKG-INFO` & `mo_sql_parsing-9.642.24144/mo_sql_parsing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.640.24141
+Version: 9.642.24144
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_sql_parsing-9.640.24141/setup.py` & `mo_sql_parsing-9.642.24144/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     install_requires=["mo-dots==10.632.24139","mo-future==7.584.24095","mo-imports==7.584.24095","mo-parsing==8.639.24140"],
     license='MPL 2.0',
     long_description='# More SQL Parsing!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-sql-parsing.svg)](https://pypi.org/project/mo-sql-parsing/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/mo-sql-parsing.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-sql-parsing)\n[![Downloads](https://pepy.tech/badge/mo-sql-parsing/month)](https://pepy.tech/project/mo-sql-parsing)\n\n\nParse SQL into JSON so we can translate it for other datastores!\n\n[See changes](https://github.com/klahnakoski/mo-sql-parsing#version-changes-features)\n\n## Objective\n\nThe objective is to convert SQL queries to JSON-izable parse trees. This originally targeted MySQL, but has grown to include other database engines. *Please [paste some SQL into a new issue](https://github.com/klahnakoski/mo-sql-parsing/issues) if it does not work for you*\n\n\n## Project Status\n\nDecember 2023 -  I continue to resolve issues as they are raised. There are [over 1100 tests](https://app.travis-ci.com/github/klahnakoski/mo-sql-parsing), that cover most SQL for most databases, with limited DML and UDF support, including:\n\n  * inner queries, \n  * with clauses, \n  * window functions\n  * create/drop/alter tables and views\n  * insert/update/delete statements\n  * create procedure and function statements (MySQL only)\n\n\n## Install\n\n    pip install mo-sql-parsing\n\n## Parsing SQL\n\n    >>> from mo_sql_parsing import parse\n    >>> parse("select count(1) from jobs")\n    {\'select\': {\'value\': {\'count\': 1}}, \'from\': \'jobs\'}\n    \nEach SQL query is parsed to an object: Each clause is assigned to an object property of the same name. \n\n    >>> parse("select a as hello, b as world from jobs")\n    {\'select\': [{\'value\': \'a\', \'name\': \'hello\'}, {\'value\': \'b\', \'name\': \'world\'}], \'from\': \'jobs\'}\n\nThe `SELECT` clause is an array of objects containing `name` and `value` properties. \n\n\n### SQL Flavours \n\nThere are a few parsing modes you may be interested in:\n\n#### Double-quotes for literal strings\n\nMySQL uses both double quotes and single quotes to declare literal strings.  This is not ansi behaviour, but it is more forgiving for programmers coming from other languages. A specific parse function is provided: \n\n    result = parse_mysql(sql)\n\n#### SQLServer Identifiers (`[]`)\n\nSQLServer uses square brackets to delimit identifiers. For example\n\n    SELECT [Timestamp] FROM [table]\n    \nwhich conflicts with BigQuery array constructor (eg `[1, 2, 3, 4]`). You may use the SqlServer flavour with \n    \n    from mo_sql_parsing import parse_sqlserver as parse\n\n#### NULL is None\n\nThe default output for this parser is to emit a null function `{"null":{}}` wherever `NULL` is encountered in the SQL.  If you would like something different, you can replace nulls with `None` (or anything else for that matter):\n\n    result = parse(sql, null=None)\n    \nthis has been implemented with a post-parse rewriting of the parse tree.\n\n\n#### Normalized function call form\n\nThe default behaviour of the parser is to output function calls in `simple_op` format: The operator being a key in the object; `{op: params}`.  This form can be difficult to work with because the object must be scanned for known operators, or possible optional arguments, or at least distinguished from a query object.\n\nYou can have the parser emit function calls in `normal_op` format\n\n    >>> from mo_sql_parsing import parse, normal_op\n    >>> parse("select trim(\' \' from b+c)", calls=normal_op)\n    \nwhich produces calls in a normalized format\n\n    {"op": op, "args": args, "kwargs": kwargs}\n\nhere is the pretty-printed JSON from the example above:\n\n```\n{\'select\': {\'value\': {\n    \'op\': \'trim\', \n    \'args\': [{\'op\': \'add\', \'args\': [\'b\', \'c\']}], \n    \'kwargs\': {\'characters\': {\'literal\': \' \'}}\n}}}\n```\n\n\n## Generating SQL\n\nYou may also generate SQL from a given JSON document. This is done by the formatter, which is usually lagging the parser (Dec2023).\n\n    >>> from mo_sql_parsing import format\n    >>> format({"from":"test", "select":["a.b", "c"]})\n    \'SELECT a.b, c FROM test\'\n\n## Contributing\n\nIn the event that the parser is not working for you, you can help make this better but simply pasting your sql (or JSON) into a new issue. Extra points if you describe the problem. Even more points if you submit a PR with a test.  If you also submit a fix, then you also have my gratitude. \n\n\n### Run Tests\n\nSee [the tests directory](https://github.com/klahnakoski/mo-sql-parsing/tree/dev/tests) for instructions running tests, or writing new ones.\n\n## More about implementation\n\nSQL queries are translated to JSON objects: Each clause is assigned to an object property of the same name.\n\n    \n    # SELECT * FROM dual WHERE a>b ORDER BY a+b\n    {\n        "select": "*", \n        "from": "dual", \n        "where": {"gt": ["a", "b"]}, \n        "orderby": {"value": {"add": ["a", "b"]}}\n    }\n        \nExpressions are also objects, but with only one property: The name of the operation, and the value holding (an array of) parameters for that operation. \n\n    {op: parameters}\n\nand you can see this pattern in the previous example:\n\n    {"gt": ["a","b"]}\n    \n## Array Programming\n\nThe `mo-sql-parsing.scrub()` method is used liberally throughout the code, and it "simplifies" the JSON.  You may find this form a bit tedious to work with because the JSON property values can be values, lists of values, or missing.  Please consider converting everything to arrays: \n\n\n```\ndef listwrap(value):\n    if value is None:\n        return []\n    elif isinstance(value, list)\n        return value\n    else:\n        return [value]\n```  \n\nthen you may avoid all the is-it-a-list checks :\n\n```\nfor select in listwrap(parsed_result.get(\'select\')):\n    do_something(select)\n```\n\n## Version Changes, Features\n\n\n### Version 10\n\n*December 2023*\n\n`SELECT *` now emits an `all_columns` call instead of plain star (`*`).  \n\n```\n>>> from mo_sql_parsing import parse\n>>> parse("SELECT * FROM table")\n{\'select\': {\'all_columns\': {}}, \'from\': \'table\'}\n```\n\nThis works better with the `except` clause, and is more explicit when selecting all child properties.\n\n``` \n>>> parse("SELECT a.* EXCEPT b FROM table")\n>>> {"select": {"all_columns": "a", "except": "b"}, "from": "table"}\n```\n\nYou may get the original behaviour by staying with version 9, or by using `all_columns="*"`:\n\n```\n>>> parse("SELECT * FROM table", all_columns="*")\n{\'select\': "*", \'from\': \'table\'}\n```\n\n\n### Version 9\n\n*November 2022*\n\nOutput for `COUNT(DISTINCT x)` has changed from function composition\n\n    {"count": {"distinct": x}}\n\nto named parameters\n\n    {"count": x, "distinct": true}\n     \nThis was part of a bug fix [issue142](https://github.com/klahnakoski/mo-sql-parsing/issues/142) - realizing `distinct` is just one parameter of many in an aggregate function. Specifically, using the `calls=normal_op` for clarity:\n    \n    >>> from mo_sql_parsing import parse, normal_op\n    >>> parse("select count(distinct x)", calls=normal_op)\n    \n    {\'select\': {\'value\': {\n        \'op\': \'count\', \n        \'args\': [x], \n        \'kwargs\': {\'distinct\': True}\n    }}}\n\n### Version 8.200+\n\n*September 2022*\n\n* Added `ALTER TABLE` and `COPY` command parsing for Snowflake \n\n\n### Version 8\n \n*November 2021*\n\n* Prefer BigQuery `[]` (create array) over SQLServer `[]` (identity) \n* Added basic DML (`INSERT`/`UPDATE`/`DELETE`)              \n* flatter `CREATE TABLE` structures. The `option` list in column definition has been flattened:<br>\n    **Old column format**\n    \n        {"create table": {\n            "columns": {\n                "name": "name",\n                "type": {"decimal": [2, 3]},\n                "option": [\n                    "not null",\n                    "check": {"lt": [{"length": "name"}, 10]}\n                ]\n            }\n        }}\n        \n    **New column format**\n                \n        {"create table": {\n            "columns": {\n                "name": "name", \n                "type": {"decimal": [2, 3]}\n                "nullable": False,\n                "check": {"lt": [{"length": "name"}, 10]} \n            }\n        }}\n\n### Version 7 \n\n*October 2021*\n\n* changed error reporting; still terrible\n* upgraded mo-parsing library which forced version change\n\n### Version 6 \n\n*October 2021*\n\n* fixed `SELECT DISTINCT` parsing\n* added `DISTINCT ON` parsing\n\n### Version 5 \n\n*August 2021*\n\n* remove inline module `mo-parsing`\n* support `CREATE TABLE`, add SQL "flavours" emit `{null:{}}` for None\n\n### Version 4\n\n*November 2021*\n\n* changed parse result of `SELECT DISTINCT`\n* simpler `ORDER BY` clause in window functions\n',
     long_description_content_type='text/markdown',
     name='mo-sql-parsing',
     packages=["mo_sql_parsing"],
     url='https://github.com/klahnakoski/mo-sql-parsing',
-    version='9.640.24141',
+    version='9.642.24144',
     zip_safe=True
 )
```

