# Comparing `tmp/huscy.project_design-0.4.0b14.tar.gz` & `tmp/huscy.project_design-0.4.1b15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_design-0.4.0b14.tar", last modified: Tue May 28 12:14:25 2024, max compression
+gzip compressed data, was "huscy.project_design-0.4.1b15.tar", last modified: Fri May 31 08:50:58 2024, max compression
```

## Comparing `huscy.project_design-0.4.0b14.tar` & `huscy.project_design-0.4.1b15.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-28 12:14:25.450046 huscy.project_design-0.4.0b14/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-05-28 12:14:25.450046 huscy.project_design-0.4.0b14/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.4.0b14/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-28 12:14:25.446046 huscy.project_design-0.4.0b14/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-28 12:14:25.450046 huscy.project_design-0.4.0b14/huscy/project_design/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2024-05-28 11:20:38.000000 huscy.project_design-0.4.0b14/huscy/project_design/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.4.0b14/huscy/project_design/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.4.0b14/huscy/project_design/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-28 12:14:25.450046 huscy.project_design-0.4.0b14/huscy/project_design/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3755 2024-05-28 12:14:24.000000 huscy.project_design-0.4.0b14/huscy/project_design/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.4.0b14/huscy/project_design/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2571 2024-02-23 10:51:00.000000 huscy.project_design-0.4.0b14/huscy/project_design/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3108 2024-05-28 11:20:38.000000 huscy.project_design-0.4.0b14/huscy/project_design/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2962 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b14/huscy/project_design/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      847 2023-09-08 08:27:43.000000 huscy.project_design-0.4.0b14/huscy/project_design/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2591 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b14/huscy/project_design/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-28 12:14:25.450046 huscy.project_design-0.4.0b14/huscy.project_design.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-05-28 12:14:25.000000 huscy.project_design-0.4.0b14/huscy.project_design.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      579 2024-05-28 12:14:25.000000 huscy.project_design-0.4.0b14/huscy.project_design.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2024-05-28 12:14:25.000000 huscy.project_design-0.4.0b14/huscy.project_design.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       70 2024-05-28 12:14:25.000000 huscy.project_design-0.4.0b14/huscy.project_design.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2024-05-28 12:14:25.000000 huscy.project_design-0.4.0b14/huscy.project_design.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2024-05-28 12:14:25.450046 huscy.project_design-0.4.0b14/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1508 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b14/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-31 08:50:58.722798 huscy.project_design-0.4.1b15/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-05-31 08:50:58.722798 huscy.project_design-0.4.1b15/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.4.1b15/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-31 08:50:58.718798 huscy.project_design-0.4.1b15/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-31 08:50:58.722798 huscy.project_design-0.4.1b15/huscy/project_design/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2024-05-31 07:57:36.000000 huscy.project_design-0.4.1b15/huscy/project_design/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.4.1b15/huscy/project_design/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.4.1b15/huscy/project_design/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-31 08:50:58.722798 huscy.project_design-0.4.1b15/huscy/project_design/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3755 2024-05-31 08:50:58.000000 huscy.project_design-0.4.1b15/huscy/project_design/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.4.1b15/huscy/project_design/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2571 2024-02-23 10:51:00.000000 huscy.project_design-0.4.1b15/huscy/project_design/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3114 2024-05-31 07:57:36.000000 huscy.project_design-0.4.1b15/huscy/project_design/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2962 2024-05-27 09:33:00.000000 huscy.project_design-0.4.1b15/huscy/project_design/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      847 2023-09-08 08:27:43.000000 huscy.project_design-0.4.1b15/huscy/project_design/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2591 2024-05-27 09:33:00.000000 huscy.project_design-0.4.1b15/huscy/project_design/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-31 08:50:58.718798 huscy.project_design-0.4.1b15/huscy.project_design.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-05-31 08:50:58.000000 huscy.project_design-0.4.1b15/huscy.project_design.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      579 2024-05-31 08:50:58.000000 huscy.project_design-0.4.1b15/huscy.project_design.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2024-05-31 08:50:58.000000 huscy.project_design-0.4.1b15/huscy.project_design.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       70 2024-05-31 08:50:58.000000 huscy.project_design-0.4.1b15/huscy.project_design.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2024-05-31 08:50:58.000000 huscy.project_design-0.4.1b15/huscy.project_design.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2024-05-31 08:50:58.722798 huscy.project_design-0.4.1b15/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1508 2024-05-27 09:33:00.000000 huscy.project_design-0.4.1b15/setup.py
```

### Comparing `huscy.project_design-0.4.0b14/PKG-INFO` & `huscy.project_design-0.4.1b15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project_design
-Version: 0.4.0b14
+Version: 0.4.1b15
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.project_design
```

### Comparing `huscy.project_design-0.4.0b14/huscy/project_design/migrations/0001_initial.py` & `huscy.project_design-0.4.1b15/huscy/project_design/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.4.0b14/huscy/project_design/models.py` & `huscy.project_design-0.4.1b15/huscy/project_design/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.4.0b14/huscy/project_design/serializer.py` & `huscy.project_design-0.4.1b15/huscy/project_design/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         read_only_fields = 'id', 'project'
 
     def update(self, experiment, validated_data):
         return services.update_experiment(experiment, **validated_data)
 
 
 class CreateExperimentSerializer(serializers.ModelSerializer):
-    sessions = SessionSerializer(many=True, required=False)
+    sessions = CreateSessionSerializer(many=True, required=False)
     title = serializers.CharField(required=False)
 
     class Meta:
         model = models.Experiment
         fields = (
             'description',
             'sessions',
```

### Comparing `huscy.project_design-0.4.0b14/huscy/project_design/services.py` & `huscy.project_design-0.4.1b15/huscy/project_design/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.4.0b14/huscy/project_design/urls.py` & `huscy.project_design-0.4.1b15/huscy/project_design/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.4.0b14/huscy/project_design/views.py` & `huscy.project_design-0.4.1b15/huscy/project_design/views.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.4.0b14/huscy.project_design.egg-info/PKG-INFO` & `huscy.project_design-0.4.1b15/huscy.project_design.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project-design
-Version: 0.4.0b14
+Version: 0.4.1b15
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.project_design
```

### Comparing `huscy.project_design-0.4.0b14/huscy.project_design.egg-info/SOURCES.txt` & `huscy.project_design-0.4.1b15/huscy.project_design.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.4.0b14/setup.py` & `huscy.project_design-0.4.1b15/setup.py`

 * *Files identical despite different names*

