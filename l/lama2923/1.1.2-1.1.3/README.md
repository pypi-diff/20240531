# Comparing `tmp/lama2923-1.1.2.tar.gz` & `tmp/lama2923-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-1.1.2.tar", last modified: Fri May 31 11:19:59 2024, max compression
+gzip compressed data, was "lama2923-1.1.3.tar", last modified: Fri May 31 11:24:20 2024, max compression
```

## Comparing `lama2923-1.1.2.tar` & `lama2923-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:19:59.229035 lama2923-1.1.2/
--rw-rw-rw-   0        0        0      962 2024-05-31 11:19:59.227960 lama2923-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 11:19:59.203961 lama2923-1.1.2/lama2923/
--rw-rw-rw-   0        0        0    24301 2024-05-31 11:19:09.000000 lama2923-1.1.2/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:19:59.224969 lama2923-1.1.2/lama2923.egg-info/
--rw-rw-rw-   0        0        0      962 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-31 11:19:59.000000 lama2923-1.1.2/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 11:19:59.229035 lama2923-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1300 2024-05-31 11:19:49.000000 lama2923-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:24:20.504682 lama2923-1.1.3/
+-rw-rw-rw-   0        0        0      962 2024-05-31 11:24:20.503684 lama2923-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 11:24:20.484659 lama2923-1.1.3/lama2923/
+-rw-rw-rw-   0        0        0    24301 2024-05-31 11:23:54.000000 lama2923-1.1.3/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:24:20.496681 lama2923-1.1.3/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      962 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 11:24:20.000000 lama2923-1.1.3/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:24:20.504682 lama2923-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-05-31 11:24:14.000000 lama2923-1.1.3/setup.py
```

### Comparing `lama2923-1.1.2/PKG-INFO` & `lama2923-1.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.1.2/lama2923/__init__.py` & `lama2923-1.1.3/lama2923/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
             if files is not None and isinstance(files, list):
                 files_data = {
                     os.path.basename(file_name): open(file_name, "rb").read()
                     for file_name in files if os.path.getsize(file_name) > 0
                 }
                 response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, files=files_data, headers=headers)
             else:
-                response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
+                response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', json=payload, headers=headers)
             return response.status_code
  
         def delete_message(self, Channel_id, Message_id):
             headers = {'Authorization': self.token}
             response = requests.delete(f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}', headers=headers)
             return response.status_code
```

### Comparing `lama2923-1.1.2/lama2923.egg-info/PKG-INFO` & `lama2923-1.1.3/lama2923.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.1.2/setup.py` & `lama2923-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='1.1.2',
+    version='1.1.3',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Api ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve Api işlemleri için kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

