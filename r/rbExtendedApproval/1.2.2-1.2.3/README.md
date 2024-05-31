# Comparing `tmp/rbextendedapproval-1.2.2.tar.gz` & `tmp/rbextendedapproval-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbextendedapproval-1.2.2.tar", last modified: Thu May 30 14:43:23 2024, max compression
+gzip compressed data, was "rbextendedapproval-1.2.3.tar", last modified: Thu May 30 22:23:00 2024, max compression
```

## Comparing `rbextendedapproval-1.2.2.tar` & `rbextendedapproval-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/extended_approval/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/admin_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:23:00.498810 rbextendedapproval-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 22:22:30.000000 rbextendedapproval-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 22:23:00.498810 rbextendedapproval-1.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:23:00.494810 rbextendedapproval-1.2.3/extended_approval/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:22:30.000000 rbextendedapproval-1.2.3/extended_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 22:22:30.000000 rbextendedapproval-1.2.3/extended_approval/admin_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18981 2024-05-30 22:22:30.000000 rbextendedapproval-1.2.3/extended_approval/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-30 22:22:30.000000 rbextendedapproval-1.2.3/extended_approval/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:23:00.498810 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 22:23:00.000000 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 22:23:00.000000 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:23:00.000000 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 22:23:00.000000 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:23:00.000000 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 22:23:00.000000 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 22:23:00.000000 rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:23:00.498810 rbextendedapproval-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 22:22:30.000000 rbextendedapproval-1.2.3/setup.py
```

### Comparing `rbextendedapproval-1.2.2/LICENSE` & `rbextendedapproval-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rbextendedapproval-1.2.2/PKG-INFO` & `rbextendedapproval-1.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbExtendedApproval
-Version: 1.2.2
+Version: 1.2.3
 Summary: Review Board extension: ExtendedApproval
 Home-page: https://github.com/misery/ExtendedApproval
 Author: Andre Klitzing
 Author-email: aklitzing@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Review Board
 Classifier: Intended Audience :: Developers
```

### Comparing `rbextendedapproval-1.2.2/extended_approval/extension.py` & `rbextendedapproval-1.2.3/extended_approval/extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,44 +33,72 @@
 CONFIG_GRACE_PERIOD_SHIPIT = 'grace_period_shipit'
 CONFIG_ENABLE_REVOKE_SHIPITS = 'enable_revoke_shipits'
 CONFIG_ENABLE_TARGET_SHIPITS = 'enable_target_shipits'
 CONFIG_ENABLE_LEGACY_BUTTONS = 'enable_legacy_buttons'
 CONFIG_ENABLE_WAIT_IT_BUTTON = 'enable_wait_it_button'
 CONFIG_FORBIDDEN_USER_SHIPITS = 'forbidden_user_shipits'
 CONFIG_FORBIDDEN_APPROVE_PREFIXES = 'forbidden_approve_prefixes'
-CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT = 'forbidden_approve_prefixes_dict'
 CONFIG_FORBIDDEN_APPROVE_SUFFIXES = 'forbidden_approve_suffixes'
-CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT = 'forbidden_approve_suffixes_dict'
+
+FORBIDDEN_APPROVE = {}
 
 
 class ReqReviews(object):
     def __init__(self, r):
         self.request = r
         self.diffset = r.get_latest_diffset()
+        self.commits = None
+        self.total = None
+        self.latest = None
+        self.self = None
+        self.revoked = None
+
+    def _calc_diffsets(self):
         self.total = []
         self.latest = []
         self.self = []
-        self.revoked = None
-
         if self.diffset:
-            shipit_reviews = r.reviews.filter(public=True, ship_it=True)
+            shipit_reviews = self.request.reviews.filter(public=True,
+                                                         ship_it=True)
             for shipit in shipit_reviews:
-                if r.submitter == shipit.user:
+                if self.request.submitter == shipit.user:
                     self.self.append(shipit)
                 else:
                     self.total.append(shipit)
 
                     if shipit.timestamp > self.diffset.timestamp:
                         self.latest.append(shipit)
 
+    def _fetch_commits(self):
+        self.commits = self.diffset.commits.all()
+
     def getDiffset(self):
         return self.diffset
 
-    def getSelf(self):
-        return self.self
+    def checkForbiddenPrefix(self):
+        if self.commits is None:
+            self._fetch_commits()
+
+        prefixes = FORBIDDEN_APPROVE[CONFIG_FORBIDDEN_APPROVE_PREFIXES]
+        for key, value in prefixes.items():
+            for commit in self.commits:
+                if commit.commit_message.startswith(key):
+                    return (value, commit)
+        return (None, None)
+
+    def checkForbiddenSuffix(self):
+        if self.commits is None:
+            self._fetch_commits()
+
+        suffixes = FORBIDDEN_APPROVE[CONFIG_FORBIDDEN_APPROVE_SUFFIXES]
+        for key, value in suffixes.items():
+            for commit in self.commits:
+                if commit.commit_message.endswith(key):
+                    return (value, commit)
+        return (None, None)
 
     def getRevoked(self):
         if self.revoked is None:
             self.revoked = []
             if self.diffset:
                 reviews = self.request.reviews.filter(public=True,
                                                       ship_it=False)
@@ -78,24 +106,33 @@
                     if self.request.submitter != shipit.user:
                         e = shipit.extra_data
                         if 'revoked_ship_it' in e and e['revoked_ship_it']:
                             self.revoked.append(shipit)
         return self.revoked
 
     def getTotal(self):
+        if self.total is None:
+            self._calc_diffsets()
         return self.total
 
     def getTotalUser(self):
-        return self._distinct_user(self.total)
+        return self._distinct_user(self.getTotal())
 
     def getLatest(self):
+        if self.latest is None:
+            self._calc_diffsets()
         return self.latest
 
     def getLatestUser(self):
-        return self._distinct_user(self.latest)
+        return self._distinct_user(self.getLatest())
+
+    def getSelf(self):
+        if self.self is None:
+            self._calc_diffsets()
+        return self.self
 
     def _distinct_user(self, sourceList):
         distinct = []
         for r in sourceList:
             if r.user not in distinct:
                 distinct.append(r.user)
         return distinct
@@ -165,31 +202,41 @@
                     '<div class="rb-icon rb-icon-{icon_name}"'
                     '      title="{title}" style="{style}"></div>',
                     **dict({'style': '', }, **detail))
                 for detail in details
             ))
 
     def render_data(self, state, review_request):
-        prefixes = self.settings[CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT]
+        prefixes = FORBIDDEN_APPROVE[CONFIG_FORBIDDEN_APPROVE_PREFIXES]
         for key, value in prefixes.items():
             if review_request.summary.startswith(key):
                 return self._render([{
                         'icon_name': 'issue-dropped',
                         'title': _(value),
                 }])
 
-        suffixes = self.settings[CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT]
+        suffixes = FORBIDDEN_APPROVE[CONFIG_FORBIDDEN_APPROVE_SUFFIXES]
         for key, value in suffixes.items():
             if review_request.summary.endswith(key):
                 return self._render([{
                         'icon_name': 'issue-dropped',
                         'title': _(value),
                 }])
 
         r = ReqReviews(review_request)
+
+        info, commit = r.checkForbiddenPrefix()
+        if info is None:
+            info, commit = r.checkForbiddenSuffix()
+        if info is not None:
+            return self._render([{
+                    'icon_name': 'issue-dropped',
+                    'title': _(info),
+            }])
+
         if len(r.getTotal()) > 0 or len(r.getRevoked()) > 0:
             if len(r.getLatest()) > 0:
                 period = check_grace_period(self.settings, r.getDiffset(),
                                             r.getLatest()[0])
 
                 if period is not None:
                     return self._render([{
@@ -230,28 +277,37 @@
         self.settings = extension.settings
 
     def is_approved(self, review_request, prev_approved, prev_failure):
         if (review_request.issue_open_count > 0 or
            review_request.issue_verifying_count > 0):
             return False, 'The review request has open issues'
 
-        prefixes = self.settings[CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT]
+        markedTempl = 'The review request is marked as "%s"'
+        prefixes = FORBIDDEN_APPROVE[CONFIG_FORBIDDEN_APPROVE_PREFIXES]
         for key, value in prefixes.items():
             if review_request.summary.startswith(key):
-                return False, 'The review request is marked as "%s"' % value
+                return False, markedTempl % value
 
-        suffixes = self.settings[CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT]
+        suffixes = FORBIDDEN_APPROVE[CONFIG_FORBIDDEN_APPROVE_SUFFIXES]
         for key, value in suffixes.items():
             if review_request.summary.endswith(key):
-                return False, 'The review request is marked as "%s"' % value
+                return False, markedTempl % value
 
         if not prev_approved:
             return False, prev_failure
 
         r = ReqReviews(review_request)
+
+        info, commit = r.checkForbiddenPrefix()
+        if info is None:
+            info, commit = r.checkForbiddenSuffix()
+        if info is not None:
+            markedTempl = 'The commit is marked as "%s": %s'
+            return False, markedTempl % (info, commit.commit_id)
+
         if len(r.getLatest()) == 0:
             return False, 'The latest diff has not been marked' \
                           ' "Ship It!" by someone else'
 
         period = check_grace_period(self.settings, r.getDiffset(),
                                     r.getLatest()[0])
         if period is not None:
@@ -403,17 +459,15 @@
         CONFIG_GRACE_PERIOD_SHIPIT: 15,
         CONFIG_ENABLE_REVOKE_SHIPITS: False,
         CONFIG_ENABLE_TARGET_SHIPITS: False,
         CONFIG_ENABLE_LEGACY_BUTTONS: False,
         # CONFIG_ENABLE_WAIT_IT_BUTTON: False,
         CONFIG_FORBIDDEN_USER_SHIPITS: '',
         CONFIG_FORBIDDEN_APPROVE_PREFIXES: 'WIP|work in progress',
-        CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT: None,
         CONFIG_FORBIDDEN_APPROVE_SUFFIXES: '',
-        CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT: None,
     }
 
     def initialize(self):
         ConfigurableApprovalHook(self)
 
         columns = [ApprovalColumn(self, id='approved')]
         DataGridColumnsHook(self, ReviewRequestDataGrid, columns)
@@ -426,28 +480,26 @@
             AdvancedPingItAction(self.settings),
             AdvancedLegacyEditReviewAction(self.settings),
             AdvancedLegacyAddGeneralCommentAction(self.settings),
             AdvancedLegacyShipItAction(self.settings),
             # AdvancedLegacyWaitItAction(self.settings),
         ])
 
-        self._init_dict(CONFIG_FORBIDDEN_APPROVE_PREFIXES,
-                        CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT)
-
-        self._init_dict(CONFIG_FORBIDDEN_APPROVE_SUFFIXES,
-                        CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT)
+        self._init_dict(CONFIG_FORBIDDEN_APPROVE_PREFIXES)
+        self._init_dict(CONFIG_FORBIDDEN_APPROVE_SUFFIXES)
 
-    def _init_dict(self, configName, configNameDict):
+    def _init_dict(self, configName):
         entries = {}
         for entry in self.settings.get(configName).splitlines():
             lineSplit = entry.split('|', 1)
             entries[lineSplit[0]] = (lineSplit[1]
                                      if len(lineSplit) > 1
                                      else lineSplit[0])
-        self.settings[configNameDict] = entries
+        global FORBIDDEN_APPROVE
+        FORBIDDEN_APPROVE[configName] = entries
 
     def shutdown(self):
         super(ExtendedApproval, self).shutdown()
 
     def _revoke_shipits(self, reviews, request):
         for r in reviews:
             r.revoke_ship_it(request.owner)
```

### Comparing `rbextendedapproval-1.2.2/extended_approval/forms.py` & `rbextendedapproval-1.2.3/extended_approval/forms.py`

 * *Files identical despite different names*

### Comparing `rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/PKG-INFO` & `rbextendedapproval-1.2.3/rbExtendedApproval.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbExtendedApproval
-Version: 1.2.2
+Version: 1.2.3
 Summary: Review Board extension: ExtendedApproval
 Home-page: https://github.com/misery/ExtendedApproval
 Author: Andre Klitzing
 Author-email: aklitzing@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Review Board
 Classifier: Intended Audience :: Developers
```

### Comparing `rbextendedapproval-1.2.2/setup.py` & `rbextendedapproval-1.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from reviewboard.extensions.packaging import setup
 
 
 PACKAGE = "rbExtendedApproval"
-VERSION = "1.2.2"
+VERSION = "1.2.3"
 
 setup(
     name=PACKAGE,
     version=VERSION,
     description='Review Board extension: ExtendedApproval',
     author='Andre Klitzing',
     author_email='aklitzing@gmail.com',
```

