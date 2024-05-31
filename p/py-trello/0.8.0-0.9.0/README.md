# Comparing `tmp/py-trello-0.8.0.tar.gz` & `tmp/py-trello-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-trello-0.8.0.tar", last modified: Wed Dec 14 14:05:36 2016, max compression
+gzip compressed data, was "dist/py-trello-0.9.0.tar", last modified: Sat Feb 18 17:53:45 2017, max compression
```

## Comparing `py-trello-0.8.0.tar` & `py-trello-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 richard   (1001) staff       (20)        0 2016-12-14 14:05:36.000000 py-trello-0.8.0/
--rw-r--r--   0 richard   (1001) staff       (20)       19 2014-03-12 19:07:51.000000 py-trello-0.8.0/MANIFEST.in
--rw-r--r--   0 richard   (1001) staff       (20)     3849 2016-12-14 14:05:36.000000 py-trello-0.8.0/PKG-INFO
-drwxr-xr-x   0 richard   (1001) staff       (20)        0 2016-12-14 14:05:36.000000 py-trello-0.8.0/py_trello.egg-info/
--rw-r--r--   0 richard   (1001) staff       (20)        1 2016-12-14 14:05:35.000000 py-trello-0.8.0/py_trello.egg-info/dependency_links.txt
--rw-r--r--   0 richard   (1001) staff       (20)     3849 2016-12-14 14:05:35.000000 py-trello-0.8.0/py_trello.egg-info/PKG-INFO
--rw-r--r--   0 richard   (1001) staff       (20)       57 2016-12-14 14:05:35.000000 py-trello-0.8.0/py_trello.egg-info/requires.txt
--rw-r--r--   0 richard   (1001) staff       (20)      562 2016-12-14 14:05:35.000000 py-trello-0.8.0/py_trello.egg-info/SOURCES.txt
--rw-r--r--   0 richard   (1001) staff       (20)       12 2016-12-14 14:05:35.000000 py-trello-0.8.0/py_trello.egg-info/top_level.txt
--rw-r--r--   0 richard   (1001) staff       (20)     2463 2016-08-08 19:59:17.000000 py-trello-0.8.0/README.rst
--rw-r--r--   0 richard   (1001) staff       (20)       59 2016-12-14 14:05:36.000000 py-trello-0.8.0/setup.cfg
--rwxr-xr-x   0 richard   (1001) staff       (20)     1095 2016-12-14 14:04:48.000000 py-trello-0.8.0/setup.py
-drwxr-xr-x   0 richard   (1001) staff       (20)        0 2016-12-14 14:05:36.000000 py-trello-0.8.0/test/
--rw-r--r--   0 richard   (1001) staff       (20)        0 2016-07-11 19:39:15.000000 py-trello-0.8.0/test/__init__.py
--rw-r--r--   0 richard   (1001) staff       (20)     8530 2016-07-11 19:39:15.000000 py-trello-0.8.0/test/test_board.py
--rw-r--r--   0 richard   (1001) staff       (20)     4898 2016-07-11 19:39:15.000000 py-trello-0.8.0/test/test_card.py
--rw-r--r--   0 richard   (1001) staff       (20)     4230 2016-07-11 19:39:15.000000 py-trello-0.8.0/test/test_checklist.py
--rw-r--r--   0 richard   (1001) staff       (20)     4301 2016-07-11 19:39:15.000000 py-trello-0.8.0/test/test_trello_client.py
-drwxr-xr-x   0 richard   (1001) staff       (20)        0 2016-12-14 14:05:36.000000 py-trello-0.8.0/trello/
--rw-r--r--   0 richard   (1001) staff       (20)      412 2016-11-20 18:34:32.000000 py-trello-0.8.0/trello/__init__.py
--rw-r--r--   0 richard   (1001) staff       (20)     1992 2016-11-20 18:34:32.000000 py-trello-0.8.0/trello/attachments.py
--rw-r--r--   0 richard   (1001) staff       (20)    10527 2016-11-20 18:34:32.000000 py-trello-0.8.0/trello/board.py
--rw-r--r--   0 richard   (1001) staff       (20)    24077 2016-12-14 14:03:52.000000 py-trello-0.8.0/trello/card.py
--rw-r--r--   0 richard   (1001) staff       (20)     4121 2016-08-08 19:59:17.000000 py-trello-0.8.0/trello/checklist.py
--rw-r--r--   0 richard   (1001) staff       (20)      413 2016-08-08 19:59:17.000000 py-trello-0.8.0/trello/compat.py
--rw-r--r--   0 richard   (1001) staff       (20)      461 2015-07-24 17:44:31.000000 py-trello-0.8.0/trello/exceptions.py
--rw-r--r--   0 richard   (1001) staff       (20)     1243 2016-07-11 19:39:15.000000 py-trello-0.8.0/trello/label.py
--rw-r--r--   0 richard   (1001) staff       (20)     2469 2016-07-11 19:39:15.000000 py-trello-0.8.0/trello/member.py
--rw-r--r--   0 richard   (1001) staff       (20)     2520 2016-08-11 16:47:04.000000 py-trello-0.8.0/trello/organization.py
--rw-r--r--   0 richard   (1001) staff       (20)     9424 2016-11-20 18:34:32.000000 py-trello-0.8.0/trello/trelloclient.py
--rw-r--r--   0 richard   (1001) staff       (20)     3556 2016-11-20 18:34:32.000000 py-trello-0.8.0/trello/trellolist.py
--rwxr-xr-x   0 richard   (1001) staff       (20)     4017 2015-07-24 17:44:31.000000 py-trello-0.8.0/trello/util.py
--rw-r--r--   0 richard   (1001) staff       (20)      681 2015-07-24 17:44:31.000000 py-trello-0.8.0/trello/webhook.py
+drwxr-xr-x   0 richard   (1001) staff       (20)        0 2017-02-18 17:53:45.000000 py-trello-0.9.0/
+-rw-r--r--   0 richard   (1001) staff       (20)       19 2014-03-12 19:07:51.000000 py-trello-0.9.0/MANIFEST.in
+-rw-r--r--   0 richard   (1001) staff       (20)     3849 2017-02-18 17:53:45.000000 py-trello-0.9.0/PKG-INFO
+drwxr-xr-x   0 richard   (1001) staff       (20)        0 2017-02-18 17:53:45.000000 py-trello-0.9.0/py_trello.egg-info/
+-rw-r--r--   0 richard   (1001) staff       (20)        1 2017-02-18 17:53:44.000000 py-trello-0.9.0/py_trello.egg-info/dependency_links.txt
+-rw-r--r--   0 richard   (1001) staff       (20)     3849 2017-02-18 17:53:44.000000 py-trello-0.9.0/py_trello.egg-info/PKG-INFO
+-rw-r--r--   0 richard   (1001) staff       (20)       57 2017-02-18 17:53:44.000000 py-trello-0.9.0/py_trello.egg-info/requires.txt
+-rw-r--r--   0 richard   (1001) staff       (20)      562 2017-02-18 17:53:44.000000 py-trello-0.9.0/py_trello.egg-info/SOURCES.txt
+-rw-r--r--   0 richard   (1001) staff       (20)       12 2017-02-18 17:53:44.000000 py-trello-0.9.0/py_trello.egg-info/top_level.txt
+-rw-r--r--   0 richard   (1001) staff       (20)     2463 2016-08-08 19:59:17.000000 py-trello-0.9.0/README.rst
+-rw-r--r--   0 richard   (1001) staff       (20)       59 2017-02-18 17:53:45.000000 py-trello-0.9.0/setup.cfg
+-rwxr-xr-x   0 richard   (1001) staff       (20)     1095 2017-02-18 17:52:29.000000 py-trello-0.9.0/setup.py
+drwxr-xr-x   0 richard   (1001) staff       (20)        0 2017-02-18 17:53:45.000000 py-trello-0.9.0/test/
+-rw-r--r--   0 richard   (1001) staff       (20)        0 2016-07-11 19:39:15.000000 py-trello-0.9.0/test/__init__.py
+-rw-r--r--   0 richard   (1001) staff       (20)     8530 2016-07-11 19:39:15.000000 py-trello-0.9.0/test/test_board.py
+-rw-r--r--   0 richard   (1001) staff       (20)     4898 2016-07-11 19:39:15.000000 py-trello-0.9.0/test/test_card.py
+-rw-r--r--   0 richard   (1001) staff       (20)     4230 2016-07-11 19:39:15.000000 py-trello-0.9.0/test/test_checklist.py
+-rw-r--r--   0 richard   (1001) staff       (20)     4301 2016-07-11 19:39:15.000000 py-trello-0.9.0/test/test_trello_client.py
+drwxr-xr-x   0 richard   (1001) staff       (20)        0 2017-02-18 17:53:45.000000 py-trello-0.9.0/trello/
+-rw-r--r--   0 richard   (1001) staff       (20)      412 2016-11-20 18:34:32.000000 py-trello-0.9.0/trello/__init__.py
+-rw-r--r--   0 richard   (1001) staff       (20)     1992 2016-11-20 18:34:32.000000 py-trello-0.9.0/trello/attachments.py
+-rw-r--r--   0 richard   (1001) staff       (20)    11216 2017-02-18 17:51:43.000000 py-trello-0.9.0/trello/board.py
+-rw-r--r--   0 richard   (1001) staff       (20)    24244 2017-02-18 17:51:43.000000 py-trello-0.9.0/trello/card.py
+-rw-r--r--   0 richard   (1001) staff       (20)     4121 2016-08-08 19:59:17.000000 py-trello-0.9.0/trello/checklist.py
+-rw-r--r--   0 richard   (1001) staff       (20)      413 2016-08-08 19:59:17.000000 py-trello-0.9.0/trello/compat.py
+-rw-r--r--   0 richard   (1001) staff       (20)      461 2015-07-24 17:44:31.000000 py-trello-0.9.0/trello/exceptions.py
+-rw-r--r--   0 richard   (1001) staff       (20)     1243 2016-07-11 19:39:15.000000 py-trello-0.9.0/trello/label.py
+-rw-r--r--   0 richard   (1001) staff       (20)     2469 2016-07-11 19:39:15.000000 py-trello-0.9.0/trello/member.py
+-rw-r--r--   0 richard   (1001) staff       (20)     2486 2017-02-18 17:51:43.000000 py-trello-0.9.0/trello/organization.py
+-rw-r--r--   0 richard   (1001) staff       (20)    12796 2017-02-18 17:51:43.000000 py-trello-0.9.0/trello/trelloclient.py
+-rw-r--r--   0 richard   (1001) staff       (20)     4555 2017-02-18 17:51:43.000000 py-trello-0.9.0/trello/trellolist.py
+-rwxr-xr-x   0 richard   (1001) staff       (20)     4017 2015-07-24 17:44:31.000000 py-trello-0.9.0/trello/util.py
+-rw-r--r--   0 richard   (1001) staff       (20)      681 2015-07-24 17:44:31.000000 py-trello-0.9.0/trello/webhook.py
```

### Comparing `py-trello-0.8.0/PKG-INFO` & `py-trello-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: py-trello
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python wrapper around the Trello API
 Home-page: https://trello.com/board/py-trello/4f145d87b2f9f15d6d027b53
 Author: Richard Kolkovich
 Author-email: richard@sigil.org
 License: BSD License
 Description: A wrapper around the Trello API written in Python. Each Trello object is
         represented by a corresponding Python object. The attributes of these objects
```

### Comparing `py-trello-0.8.0/py_trello.egg-info/PKG-INFO` & `py-trello-0.9.0/py_trello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: py-trello
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python wrapper around the Trello API
 Home-page: https://trello.com/board/py-trello/4f145d87b2f9f15d6d027b53
 Author: Richard Kolkovich
 Author-email: richard@sigil.org
 License: BSD License
 Description: A wrapper around the Trello API written in Python. Each Trello object is
         represented by a corresponding Python object. The attributes of these objects
```

### Comparing `py-trello-0.8.0/py_trello.egg-info/SOURCES.txt` & `py-trello-0.9.0/py_trello.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/README.rst` & `py-trello-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/setup.py` & `py-trello-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name="py-trello",
-    version="0.8.0",
+    version="0.9.0",
 
     description='Python wrapper around the Trello API',
     long_description=open('README.rst').read(),
     author='Richard Kolkovich',
     author_email='richard@sigil.org',
     url='https://trello.com/board/py-trello/4f145d87b2f9f15d6d027b53',
     keywords='python',
```

### Comparing `py-trello-0.8.0/test/test_board.py` & `py-trello-0.9.0/test/test_board.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/test/test_card.py` & `py-trello-0.9.0/test/test_card.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/test/test_checklist.py` & `py-trello-0.9.0/test/test_checklist.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/test/test_trello_client.py` & `py-trello-0.9.0/test/test_trello_client.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/trello/attachments.py` & `py-trello-0.9.0/trello/attachments.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/trello/board.py` & `py-trello-0.9.0/trello/board.py`

 * *Files 7% similar despite different names*

```diff
@@ -333,18 +333,37 @@
             m.status = obj.get('status', '')
             m.id = obj.get('id', '')
             m.bio = obj.get('bio', '')
             m.url = obj.get('url', '')
             m.username = obj['username']
             m.full_name = obj['fullName']
             m.initials = obj.get('initials', '')
+            m.member_type = obj.get('memberType', '')
             members.append(m)
 
         return members
 
+    # Add a member to a board
+    def add_member(self, member, member_type="normal"):
+        json_obj = self.client.fetch_json(
+            '/boards/{0}/members/{1}'.format(self.id, member.id),
+            http_method='PUT',
+            post_args={'idMember': member.id, "type": member_type},
+        )
+        return json_obj
+
+    # Removes an existing member of a board
+    def remove_member(self, member):
+        json_obj = self.client.fetch_json(
+            '/boards/{0}/members/{1}'.format(self.id, member.id),
+            http_method='DELETE',
+            post_args={'idMember': member.id},
+        )
+        return json_obj
+
     def fetch_actions(self, action_filter, action_limit=50, before=None, since=None):
         query_params = {'filter': action_filter, 'limit':  action_limit}
 
         if since:
             query_params["since"] = since
 
         if before:
```

### Comparing `py-trello-0.8.0/trello/card.py` & `py-trello-0.9.0/trello/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -481,14 +481,21 @@
 
         :due: a datetime object
         """
         datestr = due.strftime('%Y-%m-%dT%H:%M:%S')
         self._set_remote_attribute('due', datestr)
         self.due = datestr
 
+    def remove_due(self):
+        """
+        Remove the due datetime of this card.
+        """
+        self._set_remote_attribute('due', None)
+        self.due = ''
+
     def set_pos(self, pos):
         """
         Update card position in list
 
         :pos: 'top', 'bottom' or int
         """
         self._set_remote_attribute('pos', pos)
```

### Comparing `py-trello-0.8.0/trello/checklist.py` & `py-trello-0.9.0/trello/checklist.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/trello/label.py` & `py-trello-0.9.0/trello/label.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/trello/member.py` & `py-trello-0.9.0/trello/member.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/trello/organization.py` & `py-trello-0.9.0/trello/organization.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,54 +22,52 @@
         Deserialize the board json object to a Organization object
 
         :trello_client: the trello client
         :json_obj: the board json object
         """
         organization = Organization(trello_client, json_obj['id'], name=json_obj['name'])
         organization.description = json_obj.get('desc', '')
-        # cannot close an organization
-        # organization.closed = json_obj['closed']
         organization.url = json_obj['url']
         return organization
 
     def __repr__(self):
         return force_str(u'<Organization %s>' % self.name)
 
     def fetch(self):
         """Fetch all attributes for this organization"""
         json_obj = self.client.fetch_json('/organizations/' + self.id)
         self.name = json_obj['name']
         self.description = json_obj.get('desc', '')
-        self.closed = json_obj['closed']
         self.url = json_obj['url']
 
     def all_boards(self):
         """Returns all boards on this organization"""
         return self.get_boards('all')
 
     def get_boards(self, list_filter):
         """Get boards using filter
 
         :rtype: list of Board
         """
-        # error checking
+        from trello.board import Board
         json_obj = self.client.fetch_json(
             '/organizations/' + self.id + '/boards',
             query_params={'lists': 'none', 'filter': list_filter})
         return [Board.from_json(organization=self, json_obj=obj) for obj in json_obj]
 
     def get_board(self, field_name):
         """Get board
 
         :rtype: list of Board
         """
-        # error checking
+        from trello.board import Board
         json_obj = self.client.fetch_json(
             '/organizations/' + self.id + '/boards',
             query_params={'filter': 'open', 'fields': field_name})
         return [Board.from_json(organization=self, json_obj=obj) for obj in json_obj]
 
     def get_members(self):
         json_obj = self.client.fetch_json(
             '/organizations/' + self.id + '/members',
-            query_params={'filter': 'all'})
+            query_params={'filter': 'all',
+                          'fields': 'id,fullName,username,initials'})
         return [Member.from_json(trello_client=self.client, json_obj=obj) for obj in json_obj]
```

### Comparing `py-trello-0.8.0/trello/trelloclient.py` & `py-trello-0.9.0/trello/trelloclient.py`

 * *Files 22% similar despite different names*

```diff
@@ -256,7 +256,87 @@
         response = requests.post(url, data=data, auth=self.oauth)
 
         if response.status_code == 200:
             hook_id = response.json()['id']
             return WebHook(self, token, hook_id, desc, id_model, callback_url, True)
         else:
             return False
+
+    def search(self, query, partial_match=False, models=[],
+               board_ids=[], org_ids=[], card_ids=[]):
+        """
+        Search trello given a query string.
+
+        :param str query: A query string up to 16K characters
+        :param bool partial_match: True means that trello will look for
+                content that starts with any of the words in your query.
+        :param list models: Comma-separated list of types of objects to search.
+                This can be 'actions', 'boards', 'cards', 'members',
+                or 'organizations'.  The default is 'all' models.
+        :param list board_ids: Comma-separated list of boards to limit search
+        :param org_ids: Comma-separated list of organizations to limit search
+        :param card_ids: Comma-separated list of cards to limit search
+
+        :return: All objects matching the search criterial.  These can
+            be Cards, Boards, Organizations, and Members.  The attributes
+            of the objects in the results are minimal; the user must call
+            the fetch method on the resulting objects to get a full set
+            of attributes populated.
+        :rtype list:
+        """
+
+        query_params = {'query': query}
+
+        if partial_match:
+            query_params['partial'] = 'true'
+
+        # Limit search to one or more object types
+        if models:
+            query_params['modelTypes'] = models
+
+        # Limit search to a particular subset of objects
+        if board_ids:
+            query_params['idBoards'] = board_ids
+        if org_ids:
+            query_params['idOrganizations'] = org_ids
+        if card_ids:
+            query_params['idCards'] = card_ids
+
+        # Request result fields required to instantiate class objects
+        query_params['board_fields'] = ['name,url,desc,closed']
+        query_params['member_fields'] = ['fullName,initials,username']
+        query_params['organization_fields'] = ['name,url,desc']
+
+        json_obj = self.fetch_json('/search', query_params=query_params)
+        if not json_obj:
+            return []
+
+        results = []
+        board_cache = {}
+
+        for board_json in json_obj.get('boards', []):
+            # Cache board objects
+            if board_json['id'] not in board_cache:
+                board_cache[board_json['id']] = Board.from_json(
+                    self, json_obj=board_json)
+            results.append(board_cache[board_json['id']])
+
+        for card_json in json_obj.get('cards', []):
+            # Cache board objects
+            if card_json['idBoard'] not in board_cache:
+                board_cache[card_json['idBoard']] = Board(
+                    self, card_json['idBoard'])
+                # Fetch the board attributes as the Board object created
+                # from the card initially result lacks a URL and name.
+                # This Board will be stored in Card.parent
+                board_cache[card_json['idBoard']].fetch()
+            results.append(Card.from_json(board_cache[card_json['idBoard']],
+                                          card_json))
+
+        for member_json in json_obj.get('members', []):
+            results.append(Member.from_json(self, member_json))
+
+        for org_json in json_obj.get('organizations', []):
+            org = Organization.from_json(self, org_json)
+            results.append(org)
+
+        return results
```

### Comparing `py-trello-0.8.0/trello/trellolist.py` & `py-trello-0.9.0/trello/trellolist.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,38 +46,66 @@
         self.pos = json_obj['pos']
 
     def list_cards(self, card_filter="open"):
         """Lists all cards in this list"""
         json_obj = self.client.fetch_json('/lists/' + self.id + '/cards/' + card_filter)
         return [Card.from_json(self, c) for c in json_obj]
 
-    def add_card(self, name, desc=None, labels=[], due="null", source=None):
+    def add_card(self, name, desc=None, labels=None, due="null", source=None, position=None):
         """Add a card to this list
 
         :name: name for the card
         :desc: the description of the card
         :labels: a list of label IDs to be added
         :due: due date for the card
         :source: card ID from which to clone from
+        :position: position of the card in the list. Must be "top", "bottom" or a positive number.
         :return: the card
         """
         labels_str = ""
-        for label in labels:
-            labels_str += label.id + ","
+        if labels:
+            for label in labels:
+                labels_str += label.id + ","
+
+        post_args = {
+            'name': name,
+            'idList': self.id,
+            'desc': desc,
+            'idLabels': labels_str[:-1],
+            'due': due,
+            'idCardSource': source,
+        }
+        if position is not None:
+            post_args["pos"] = position
+
         json_obj = self.client.fetch_json(
             '/cards',
             http_method='POST',
-            post_args={'name': name, 'idList': self.id, 'desc': desc, 'idLabels': labels_str[:-1], 'due': due, 'idCardSource': source})
+            post_args=post_args)
         return Card.from_json(self, json_obj)
 
     def archive_all_cards(self):
         self.client.fetch_json(
             '/lists/' + self.id + '/archiveAllCards',
             http_method='POST')
 
+    def move_all_cards(self, destination_list):
+        """
+        Move all cards of this list to another list.
+        The list can be in the same board (or not).
+        """
+
+        self.client.fetch_json(
+            '/lists/' + self.id + '/moveAllCards',
+            http_method='POST',
+            post_args = {
+                "idBoard": destination_list.board.id,
+                "idList": destination_list.id,
+            })
+
     def fetch_actions(self, action_filter):
         """
         Fetch actions for this list can give more argv to action_filter,
         split for ',' json_obj is list
         """
         json_obj = self.client.fetch_json(
             '/lists/' + self.id + '/actions',
@@ -100,12 +128,20 @@
     def open(self):
         self.client.fetch_json(
             '/lists/' + self.id + '/closed',
             http_method='PUT',
             post_args={'value': 'false', }, )
         self.closed = False
 
+    # Move this list
+    def move(self, position):
+        self.client.fetch_json(
+            '/lists/' + self.id + '/pos',
+            http_method='PUT',
+            post_args={'value': position, }, )
+        self.pos = position
+
     def cardsCnt(self):
         return len(self.list_cards())
 
 
 from trello.card import Card
```

### Comparing `py-trello-0.8.0/trello/util.py` & `py-trello-0.9.0/trello/util.py`

 * *Files identical despite different names*

### Comparing `py-trello-0.8.0/trello/webhook.py` & `py-trello-0.9.0/trello/webhook.py`

 * *Files identical despite different names*

