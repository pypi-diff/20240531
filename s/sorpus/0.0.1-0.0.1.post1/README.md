# Comparing `tmp/sorpus-0.0.1.tar.gz` & `tmp/sorpus-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorpus-0.0.1.tar", last modified: Fri May 24 14:03:57 2024, max compression
+gzip compressed data, was "sorpus-0.0.1.post1.tar", last modified: Fri May 31 10:08:14 2024, max compression
```

## Comparing `sorpus-0.0.1.tar` & `sorpus-0.0.1.post1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 siwon     (1000) siwon     (1000)        0 2024-05-24 14:03:57.726885 sorpus-0.0.1/
--rw-r--r--   0 siwon     (1000) siwon     (1000)    11339 2024-05-24 10:32:36.000000 sorpus-0.0.1/LICENSE
--rw-r--r--   0 siwon     (1000) siwon     (1000)      564 2024-05-24 14:03:57.726885 sorpus-0.0.1/PKG-INFO
--rw-r--r--   0 siwon     (1000) siwon     (1000)       51 2024-05-24 10:32:36.000000 sorpus-0.0.1/README.md
--rw-r--r--   0 siwon     (1000) siwon     (1000)      494 2024-05-24 14:03:40.000000 sorpus-0.0.1/pyproject.toml
--rw-r--r--   0 siwon     (1000) siwon     (1000)       38 2024-05-24 14:03:57.726885 sorpus-0.0.1/setup.cfg
-drwxr-xr-x   0 siwon     (1000) siwon     (1000)        0 2024-05-24 14:03:57.716885 sorpus-0.0.1/src/
-drwxr-xr-x   0 siwon     (1000) siwon     (1000)        0 2024-05-24 14:03:57.726885 sorpus-0.0.1/src/sorpus/
--rw-r--r--   0 siwon     (1000) siwon     (1000)      100 2024-05-24 13:13:27.000000 sorpus-0.0.1/src/sorpus/__init__.py
--rw-r--r--   0 siwon     (1000) siwon     (1000)       22 2024-05-24 13:13:34.000000 sorpus-0.0.1/src/sorpus/__version__.py
--rw-r--r--   0 siwon     (1000) siwon     (1000)     1445 2024-05-24 13:13:22.000000 sorpus-0.0.1/src/sorpus/masker.py
--rw-r--r--   0 siwon     (1000) siwon     (1000)     1302 2024-05-24 12:58:44.000000 sorpus-0.0.1/src/sorpus/sentences.py
-drwxr-xr-x   0 siwon     (1000) siwon     (1000)        0 2024-05-24 14:03:57.726885 sorpus-0.0.1/src/sorpus.egg-info/
--rw-r--r--   0 siwon     (1000) siwon     (1000)      564 2024-05-24 14:03:57.000000 sorpus-0.0.1/src/sorpus.egg-info/PKG-INFO
--rw-r--r--   0 siwon     (1000) siwon     (1000)      262 2024-05-24 14:03:57.000000 sorpus-0.0.1/src/sorpus.egg-info/SOURCES.txt
--rw-r--r--   0 siwon     (1000) siwon     (1000)        1 2024-05-24 14:03:57.000000 sorpus-0.0.1/src/sorpus.egg-info/dependency_links.txt
--rw-r--r--   0 siwon     (1000) siwon     (1000)        7 2024-05-24 14:03:57.000000 sorpus-0.0.1/src/sorpus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:08:14.739370 sorpus-0.0.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-31 10:08:01.000000 sorpus-0.0.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-31 10:08:14.739370 sorpus-0.0.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-31 10:08:01.000000 sorpus-0.0.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-31 10:08:01.000000 sorpus-0.0.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:08:14.739370 sorpus-0.0.1.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:08:14.735370 sorpus-0.0.1.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:08:14.739370 sorpus-0.0.1.post1/src/sorpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 10:08:01.000000 sorpus-0.0.1.post1/src/sorpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 10:08:01.000000 sorpus-0.0.1.post1/src/sorpus/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-31 10:08:01.000000 sorpus-0.0.1.post1/src/sorpus/replacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-31 10:08:01.000000 sorpus-0.0.1.post1/src/sorpus/sentences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:08:14.739370 sorpus-0.0.1.post1/src/sorpus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-31 10:08:14.000000 sorpus-0.0.1.post1/src/sorpus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 10:08:14.000000 sorpus-0.0.1.post1/src/sorpus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:08:14.000000 sorpus-0.0.1.post1/src/sorpus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 10:08:14.000000 sorpus-0.0.1.post1/src/sorpus.egg-info/top_level.txt
```

### Comparing `sorpus-0.0.1/LICENSE` & `sorpus-0.0.1.post1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2014 Siwon Seo
+   Copyright 2024 Siwon Seo
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sorpus-0.0.1/src/sorpus/masker.py` & `sorpus-0.0.1.post1/src/sorpus/replacer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import List
+from typing import List, Tuple
 
-class SpecialWordMasker:
+class SpecialWordReplacer:
     """
-    This class masks special words in a text.
+    This class replace or mask special words between in particular words in a text.
 
-    :param special_words: List of special words to mask
-    :param target_word: Word to mask in special words
+    :param special_words: List of special words to replace or mask
+    :param target_word: Word to replace or mask in special words
     :param replacement_char: Character to replace the target word with
 
-    >>> masker = MaskSpecialWords(['New York', 'El Nino'], ' ', '•')
-    >>> masker.mask_special_char_in_words('New York is affected by El Nino.')
-    'New•York is affected by El•Nino.'
+    >>> replacer = SpecialWordReplacer(['New York', 'El Nino'], ' ', '•')
+    >>> print(replacer.mask_words('New York is affected by El Nino.'))
+    New•York is affected by El•Nino.
+    >>> replacer = SpecialWordReplacer(['"apple"'], 'apple', 'green apple')
+    >>> print(replacer.mask_words('He said the word "apple" while pointing at an apple.'))
+    He said the word "green apple" while pointing at an apple.
     """
     def __init__(self, special_words: List[str], target_word: str, replacement_char: str):
-        import re
-        
         self.special_words = special_words
         self.target_word = target_word
         self.replacement_char = replacement_char
-        self.patterns = [re.compile(r'\b' + re.escape(word) + r'\b') for word in special_words]
 
     def mask_words(self, text: str) -> str:
         """
         This function masks special words in a text.
 
         :param text: Text to mask special words in
 
         :return: Text with special words masked
         """
-        for i, word in enumerate(self.special_words):
+        for word in self.special_words:
             masked_word = word.replace(self.target_word, self.replacement_char)
-            text = self.patterns[i].sub(masked_word, text)
+            text = text.replace(word, masked_word)
         return text
     
     def __repr__(self):
-        return f'<SpecialWordMasker(special_words={self.special_words}, target_word={self.target_word}, replacement_char={self.replacement_char})>'
+        return f'<SpecialWordReplacer(special_words={self.special_words}, target_word=\'{self.target_word}\', replacement_char=\'{self.replacement_char}\')>'
```

### Comparing `sorpus-0.0.1/src/sorpus/sentences.py` & `sorpus-0.0.1.post1/src/sorpus/sentences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List
 
+
 def find_with_word(word: str, sentences: List[str]) -> List[str]:
     """
     This function checks if a word is in a list of sentences.
 
     :param word: Word to check
     :param sentences: List of sentences
     
@@ -12,14 +13,15 @@
     >>> print(find_with_word('experience', [
     ...     'Proverbs are short sentences drawn from long experience.', 
     ...     'Naked I came into the world, and naked I must go out.']))
     ['Proverbs are short sentences drawn from long experience.']
     """
     return [sentence for sentence in sentences if word in sentence]
 
+
 def replace_word(word: str, new_word: str, sentences: List[str]) -> List[str]:
     """
     This function replaces a word with a new word in a list of sentences.
 
     :param word: Word to replace
     :param new_word: New word to replace with
     :param sentences: List of sentences
```

