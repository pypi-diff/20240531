# Comparing `tmp/lama2923-1.1.3.tar.gz` & `tmp/lama2923-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-1.1.3.tar", last modified: Fri May 31 11:24:20 2024, max compression
+gzip compressed data, was "lama2923-1.1.5.tar", last modified: Fri May 31 16:46:59 2024, max compression
```

## Comparing `lama2923-1.1.3.tar` & `lama2923-1.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:24:20.504682 lama2923-1.1.3/
--rw-rw-rw-   0        0        0      962 2024-05-31 11:24:20.503684 lama2923-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 11:24:20.484659 lama2923-1.1.3/lama2923/
--rw-rw-rw-   0        0        0    24301 2024-05-31 11:23:54.000000 lama2923-1.1.3/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:24:20.496681 lama2923-1.1.3/lama2923.egg-info/
--rw-rw-rw-   0        0        0      962 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 11:24:20.504682 lama2923-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1300 2024-05-31 11:24:14.000000 lama2923-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 16:46:59.629565 lama2923-1.1.5/
+-rw-rw-rw-   0        0        0      962 2024-05-31 16:46:59.616567 lama2923-1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 16:46:59.600564 lama2923-1.1.5/lama2923/
+-rw-rw-rw-   0        0        0    24365 2024-05-31 16:44:48.000000 lama2923-1.1.5/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 16:46:59.613564 lama2923-1.1.5/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      962 2024-05-31 16:46:59.000000 lama2923-1.1.5/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-31 16:46:59.000000 lama2923-1.1.5/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 16:46:59.000000 lama2923-1.1.5/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 16:46:59.000000 lama2923-1.1.5/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 16:46:59.000000 lama2923-1.1.5/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 16:46:59.629565 lama2923-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-05-31 16:46:33.000000 lama2923-1.1.5/setup.py
```

### Comparing `lama2923-1.1.3/PKG-INFO` & `lama2923-1.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.1.3
+Version: 1.1.5
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.1.3/lama2923/__init__.py` & `lama2923-1.1.5/lama2923/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,17 +233,18 @@
         
         def edit_message(self, Channel_id, Message_id, Message_Content):
             headers = {'Authorization': self.token}
             payload = {'content': str(Message_Content)}
             response = requests.patch(f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}', json=payload, headers=headers)
             return response.status_code
         
-        def get_channel_messages(self, Channel_id):
+        def get_channel_messages(self, Channel_id, limit=50):
             headers = {'Authorization': self.token}
-            response = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/messages', headers=headers)
+            params = {'limit': limit}
+            response = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/messages', headers=headers, params=params)
             return response.status_code, response.json() if response.status_code == 200 else response.status_code
 
         def get_channel_message(self, Channel_id, Message_id):
             headers = {'Authorization': self.token}
             response = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}', headers=headers)
             return response.status_code, response.json() if response.status_code == 200 else response.status_code
```

### Comparing `lama2923-1.1.3/lama2923.egg-info/PKG-INFO` & `lama2923-1.1.5/lama2923.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.1.3
+Version: 1.1.5
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.1.3/setup.py` & `lama2923-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='1.1.3',
+    version='1.1.5',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Api ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve Api işlemleri için kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

