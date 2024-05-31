# Comparing `tmp/mutt_html_reply-0.3.1.tar.gz` & `tmp/mutt_html_reply-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutt_html_reply-0.3.1.tar", last modified: Thu May 30 03:24:05 2024, max compression
+gzip compressed data, was "mutt_html_reply-0.3.2.tar", last modified: Thu May 30 04:41:15 2024, max compression
```

## Comparing `mutt_html_reply-0.3.1.tar` & `mutt_html_reply-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/
--rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.3.1/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      807 2024-05-30 03:23:26.000000 mutt_html_reply-0.3.1/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-05-30 03:22:28.000000 mutt_html_reply-0.3.1/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/setup.cfg
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/src/
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/src/mutt_html_reply/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.3.1/src/mutt_html_reply/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3441 2024-05-30 03:02:53.000000 mutt_html_reply-0.3.1/src/mutt_html_reply/mutt_html_reply.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 04:41:15.108390 mutt_html_reply-0.3.2/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.3.2/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-30 04:41:15.108390 mutt_html_reply-0.3.2/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      807 2024-05-30 03:23:26.000000 mutt_html_reply-0.3.2/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-05-30 04:40:40.000000 mutt_html_reply-0.3.2/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-30 04:41:15.108390 mutt_html_reply-0.3.2/setup.cfg
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 04:41:15.108390 mutt_html_reply-0.3.2/src/
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 04:41:15.108390 mutt_html_reply-0.3.2/src/mutt_html_reply/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.3.2/src/mutt_html_reply/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4057 2024-05-30 04:40:14.000000 mutt_html_reply-0.3.2/src/mutt_html_reply/mutt_html_reply.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 04:41:15.108390 mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-30 04:41:15.000000 mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-05-30 04:41:15.000000 mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-30 04:41:15.000000 mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-05-30 04:41:15.000000 mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-05-30 04:41:15.000000 mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-05-30 04:41:15.000000 mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/top_level.txt
```

### Comparing `mutt_html_reply-0.3.1/LICENSE` & `mutt_html_reply-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.3.1/PKG-INFO` & `mutt_html_reply-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.3.1
+Version: 0.3.2
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `mutt_html_reply-0.3.1/README.md` & `mutt_html_reply-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.3.1/pyproject.toml` & `mutt_html_reply-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mutt-html-reply"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
 	"bs4",
 	"css_inline"
 ]
 authors = [
 	{name = "Erik Rogers", email = "erik@rogers-family.net"}
 ]
```

### Comparing `mutt_html_reply-0.3.1/src/mutt_html_reply/mutt_html_reply.py` & `mutt_html_reply-0.3.2/src/mutt_html_reply/mutt_html_reply.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     ## headers
     bs4_original_headers = BeautifulSoup(html_original_headers, 'html.parser')
 
     # Combine converted HTML together
     bs4_final = bs4_msg
     bs4_final.body.append(BeautifulSoup('<hr></hr>', 'html.parser')) #type: ignore
     bs4_final.body.append(bs4_original_headers) #type: ignore
+    bs4_final.body.append(BeautifulSoup('<br></br>', 'html.parser')) #type: ignore
     bs4_final.body.append(bs4_original_msg) #type: ignore
 
     # Write output
     args.output.write(str(bs4_final))
 
 
 def _get_header_html(message):
@@ -77,24 +78,36 @@
     if message['subject'] is not None:
         headers = headers + '<b>Subject</b>: ' + html.escape(message['subject']) + '<br></br>'
     return headers
 
 
 def _get_message_html(message):
     body = None
+    first_part = True
     if message.is_multipart():
         for part in message.walk():
             ctype = part.get_content_type()
             cdispo = str(part.get('Content-Disposition'))
+            cquote = str(part.get('Content-Transfer-Encoding'))
             if ctype == 'text/html' and 'attachment' not in cdispo:
-                body = part.get_payload()
-                break
-    else:
-        body = message.get_payload()
-
+                if first_part:
+                    if cquote == 'quoted-printable':
+                        body = part.get_payload(decode=True)
+                        first_part = False
+                    else:
+                        body = part.get_payload()
+                else:
+                    if cquote == 'quoted-printable':
+                        body = body + part.get_payload(decode=True)
+                    else:
+                        body = body + part.get_payload()
     if body is not None:
-        return str(body)
+        try:
+            return body.decode("utf-8")
+        except:
+            return body
     else:
         raise ValueError
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/PKG-INFO` & `mutt_html_reply-0.3.2/src/mutt_html_reply.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.3.1
+Version: 0.3.2
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

