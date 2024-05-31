# Comparing `tmp/xphonebr-0.0.1.tar.gz` & `tmp/xphonebr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xphonebr-0.0.1.tar", last modified: Fri May 31 08:54:40 2024, max compression
+gzip compressed data, was "xphonebr-0.0.2.tar", last modified: Fri May 31 10:15:24 2024, max compression
```

## Comparing `xphonebr-0.0.1.tar` & `xphonebr-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:54:40.879881 xphonebr-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-31 08:54:40.879881 xphonebr-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:54:23.000000 xphonebr-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 08:54:40.879881 xphonebr-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-31 08:54:23.000000 xphonebr-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:54:40.875881 xphonebr-0.0.1/xphonebr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:54:40.875881 xphonebr-0.0.1/xphonebr/Util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:54:23.000000 xphonebr-0.0.1/xphonebr/Util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-31 08:54:23.000000 xphonebr-0.0.1/xphonebr/Util/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-31 08:54:23.000000 xphonebr-0.0.1/xphonebr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:54:40.879881 xphonebr-0.0.1/xphonebr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-31 08:54:40.000000 xphonebr-0.0.1/xphonebr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-31 08:54:40.000000 xphonebr-0.0.1/xphonebr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:54:40.000000 xphonebr-0.0.1/xphonebr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 08:54:40.000000 xphonebr-0.0.1/xphonebr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 08:54:40.000000 xphonebr-0.0.1/xphonebr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:15:24.026914 xphonebr-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 10:15:12.000000 xphonebr-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 10:15:24.026914 xphonebr-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-31 10:15:12.000000 xphonebr-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 10:15:24.026914 xphonebr-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-31 10:15:12.000000 xphonebr-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:15:24.026914 xphonebr-0.0.2/xphonebr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:15:24.026914 xphonebr-0.0.2/xphonebr/Util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:15:12.000000 xphonebr-0.0.2/xphonebr/Util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-31 10:15:12.000000 xphonebr-0.0.2/xphonebr/Util/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-31 10:15:12.000000 xphonebr-0.0.2/xphonebr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:15:24.026914 xphonebr-0.0.2/xphonebr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 10:15:24.000000 xphonebr-0.0.2/xphonebr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 10:15:24.000000 xphonebr-0.0.2/xphonebr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:15:24.000000 xphonebr-0.0.2/xphonebr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 10:15:24.000000 xphonebr-0.0.2/xphonebr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 10:15:24.000000 xphonebr-0.0.2/xphonebr.egg-info/top_level.txt
```

### Comparing `xphonebr-0.0.1/PKG-INFO` & `xphonebr-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xphonebr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Grapheme to phoneme conversion and tools for tts with deep learning.
 Author: Emerson Pedroso
 Author-email: traderpedroso@icloud.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Requires-Dist: tqdm>=4.38.0
 Requires-Dist: deep-phonemizer==0.0.19
 Requires-Dist: num2words==0.5.12
 
 XphoneBR is a portuguese transformer base grapheme-to-phoneme normalization  tool modeling library that leverages recent deep learning 
 technology and is optimized for usage in production systems such as TTS. In particular, the library should
 be accurate, fast, easy to use.
```

### Comparing `xphonebr-0.0.1/setup.py` & `xphonebr-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 long_description = """XphoneBR is a portuguese transformer base grapheme-to-phoneme normalization  tool modeling library that leverages recent deep learning 
 technology and is optimized for usage in production systems such as TTS. In particular, the library should
 be accurate, fast, easy to use. 
 
 DeepPhonemizerBR is compatible with Python 3.6+ and is distributed under the MIT license.
 
 """
-# Version: 0.0.1
+# Version: 0.0.2
 setup(
     name="xphonebr",
-    version="0.0.1",
+    version="0.0.2",
     author="Emerson Pedroso",
     author_email="traderpedroso@icloud.com",
     description="Grapheme to phoneme conversion and tools for tts with deep learning.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="MIT",
     install_requires=[
```

### Comparing `xphonebr-0.0.1/xphonebr/Util/norm.py` & `xphonebr-0.0.2/xphonebr/Util/norm.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,22 +105,20 @@
 
 
 def remove_aux_symbols(text):
     text = re.sub(r"[\<\>\(\)\[\]\"\«\»\']+", "", text)
     return text
 
 
-# Função para normalizar porcentagens
 def _normalize_percentages(text):
     return re.sub(
         r"(\d+)%", lambda m: num2words(m.group(1), lang="pt") + " por cento", text
     )
 
 
-# Função para normalizar horas
 def _normalize_time(text):
     def time_to_words(match):
         hours = int(match.group(1))
         minutes = int(match.group(2))
         hours_text = num2words(hours, lang="pt", to="cardinal")
         if minutes == 0:
             return f"{hours_text} hora" + ("s" if hours > 1 else "")
@@ -131,47 +129,73 @@
             + f" e {minutes_text} minuto"
             + ("s" if minutes > 1 else "")
         )
 
     return re.sub(r"(\d{1,2}):(\d{2})", time_to_words, text)
 
 
-# Função para normalizar valores monetários
 def _normalize_money(text):
     def money_to_words(match):
-        integer_part = int(match.group(1).replace(".", ""))
-        cents = int(match.group(2))
-        integer_part_text = num2words(integer_part, lang="pt") + (
-            " reais" if integer_part > 1 else " real"
-        )
-        if cents == 0:
-            return integer_part_text
-        cents_text = (
-            num2words(cents, lang="pt") + " centavo" + ("s" if cents > 1 else "")
-        )
-        return f"{integer_part_text} e {cents_text}"
-
-    return re.sub(r"R\$ (\d+[\.\d]*),(\d{2})", money_to_words, text)
+        currency = match.group(1)
+        amount = int(match.group(2).replace(".", ""))
+        currency_text = {
+            "R$": "reais" if amount > 1 else "real",
+            "$": "dólares" if amount > 1 else "dólar",
+            "€": "euros",
+            "£": "libras",
+        }.get(currency, "reais")
+
+        amount_text = num2words(amount, lang="pt")
+        return f"{amount_text} {currency_text}"
+
+    # Regular expressions for different currency formats
+    text = re.sub(r"(R\$|€|£|\$) (\d+[\.\d]*)", money_to_words, text)
+    text = re.sub(r"(R\$|€|£|\$)(\d+[\.\d]*)", money_to_words, text)
+    text = re.sub(r"R\$ (\d+[\.\d]*),(\d{2})", money_to_words, text)
+    return text
 
 
-# Função para converter todos os números isolados no texto para palavras
 def _normalize_numbers(text):
     return re.sub(r"\b\d+\b", lambda x: num2words(x.group(), lang="pt"), text)
 
 
 def _normalize_abbreviations(text):
     for regex, substitutions in abbreviations:
         text = re.sub(regex, substitutions, text)
     return text
 
 
+def _normalize_am_pm_times(text):
+    def am_pm_to_words(match):
+        hours = int(match.group(1))
+        period = match.group(2).lower()
+        if period == "pm" and hours != 12:
+            hours += 12
+        elif period == "am" and hours == 12:
+            hours = 0
+        hours_text = num2words(hours, lang="pt", to="cardinal")
+        return f"{hours_text} horas"
+
+    return re.sub(r"(\d{1,2})(am|pm)", am_pm_to_words, text)
+
+
+def _normalize_numbers_with_letters(text):
+    return re.sub(
+        r"(\d+)([a-zA-Z]+)",
+        lambda m: f"{num2words(m.group(1), lang='pt')} {m.group(2)}",
+        text,
+    )
+
+
 def normalizer(text):
     text = _normalize_percentages(text)
     text = _normalize_time(text)
     text = _normalize_money(text)
+    text = _normalize_am_pm_times(text)
+    text = _normalize_numbers_with_letters(text)
     text = _normalize_numbers(text)
     text = _normalize_abbreviations(text)
     text = replace_punctuation(text)
     text = remove_aux_symbols(text)
     text = remove_punctuation_at_begin(text)
     text = collapse_whitespace(text)
     text = re.sub(r"([^\.,!\?\-…])$", r"\1.", text)
```

### Comparing `xphonebr-0.0.1/xphonebr/__init__.py` & `xphonebr-0.0.2/xphonebr/__init__.py`

 * *Files identical despite different names*

### Comparing `xphonebr-0.0.1/xphonebr.egg-info/PKG-INFO` & `xphonebr-0.0.2/xphonebr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xphonebr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Grapheme to phoneme conversion and tools for tts with deep learning.
 Author: Emerson Pedroso
 Author-email: traderpedroso@icloud.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Requires-Dist: tqdm>=4.38.0
 Requires-Dist: deep-phonemizer==0.0.19
 Requires-Dist: num2words==0.5.12
 
 XphoneBR is a portuguese transformer base grapheme-to-phoneme normalization  tool modeling library that leverages recent deep learning 
 technology and is optimized for usage in production systems such as TTS. In particular, the library should
 be accurate, fast, easy to use.
```

