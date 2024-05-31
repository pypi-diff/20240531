# Comparing `tmp/pyerualjetwork-1.3.7.tar.gz` & `tmp/pyerualjetwork-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.7.tar", last modified: Thu May 30 23:25:29 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.8.tar", last modified: Fri May 31 01:07:20 2024, max compression
```

## Comparing `pyerualjetwork-1.3.7.tar` & `pyerualjetwork-1.3.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 23:25:29.161381 pyerualjetwork-1.3.7/
--rw-rw-rw-   0        0        0      391 2024-05-30 23:25:29.160379 pyerualjetwork-1.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-30 23:25:29.110507 pyerualjetwork-1.3.7/plan/
--rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.7/plan/__init__.py
--rw-rw-rw-   0        0        0    44862 2024-05-30 23:23:36.000000 pyerualjetwork-1.3.7/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-30 23:25:29.157448 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      391 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 23:25:29.162379 pyerualjetwork-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      570 2024-05-30 23:24:45.000000 pyerualjetwork-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:07:20.475019 pyerualjetwork-1.3.8/
+-rw-rw-rw-   0        0        0      391 2024-05-31 01:07:20.474020 pyerualjetwork-1.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 01:07:20.425104 pyerualjetwork-1.3.8/plan/
+-rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.8/plan/__init__.py
+-rw-rw-rw-   0        0        0    45348 2024-05-31 01:04:03.000000 pyerualjetwork-1.3.8/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:07:20.471029 pyerualjetwork-1.3.8/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      391 2024-05-31 01:07:19.000000 pyerualjetwork-1.3.8/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-31 01:07:20.000000 pyerualjetwork-1.3.8/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 01:07:19.000000 pyerualjetwork-1.3.8/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-31 01:07:19.000000 pyerualjetwork-1.3.8/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 01:07:20.476016 pyerualjetwork-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      570 2024-05-31 01:05:05.000000 pyerualjetwork-1.3.8/setup.py
```

### Comparing `pyerualjetwork-1.3.7/plan/plan.py` & `pyerualjetwork-1.3.8/plan/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,21 +708,37 @@
         if acc >= 0.8:
             print(Fore.GREEN + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
         
         elif acc < 0.8 and acc > 0.6:
             print(Fore.MAGENTA + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
         
         elif acc <= 0.6:
-            print(Fore.RED+ '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)   
+            print(Fore.RED+ '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)  
+
+        
+        y_testVisual = np.copy(y_test) 
+        y_testVisual = np.argmax(y_testVisual, axis=1)
+        
+        plt.figure(figsize=(12, 6))
+        sns.kdeplot(y_testVisual, label='Real Outputs', fill=True)
+        sns.kdeplot(TestPredictions, label='Predictions', fill=True)
+        plt.legend()
+        plt.xlabel('Class')
+        plt.ylabel('Data size')
+        plt.title('Predictions and Real Outputs for Testing KDE Plot')
+        plt.show()
+        
     
     except:
         
         print(Fore.RED + "ERROR: Testing model parameters like 'layers' 'MembranCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
         return 'e'
    
+
+   
     return W,TestPredictions,acc
 
 def SavePLAN(model_name,
              model_type,
              layers,
              class_count,
              membran_thresholds,
```

### Comparing `pyerualjetwork-1.3.7/setup.py` & `pyerualjetwork-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.7",
+      version = "1.3.8",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library. MASSIVE Technic Update, unlocked class limits. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
```

