# Comparing `tmp/eurlex-parser-0.0.2.tar.gz` & `tmp/eurlex-parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurlex-parser-0.0.2.tar", last modified: Thu May 30 18:45:21 2024, max compression
+gzip compressed data, was "eurlex-parser-0.0.3.tar", last modified: Fri May 31 21:09:53 2024, max compression
```

## Comparing `eurlex-parser-0.0.2.tar` & `eurlex-parser-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 18:45:21.834942 eurlex-parser-0.0.2/
--rw-rw-rw-   0        0        0     3464 2024-05-30 18:45:21.833940 eurlex-parser-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2922 2024-05-30 18:42:53.000000 eurlex-parser-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-30 18:45:21.834942 eurlex-parser-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1184 2024-05-30 18:45:03.000000 eurlex-parser-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:45:21.806814 eurlex-parser-0.0.2/src/
--rw-rw-rw-   0        0        0     7327 2024-05-30 16:52:13.000000 eurlex-parser-0.0.2/src/eurlex.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:45:21.833940 eurlex-parser-0.0.2/src/eurlex_parser.egg-info/
--rw-rw-rw-   0        0        0     3464 2024-05-30 18:45:21.000000 eurlex-parser-0.0.2/src/eurlex_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 18:45:21.000000 eurlex-parser-0.0.2/src/eurlex_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 18:45:21.000000 eurlex-parser-0.0.2/src/eurlex_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-30 18:45:21.000000 eurlex-parser-0.0.2/src/eurlex_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 18:45:21.000000 eurlex-parser-0.0.2/src/eurlex_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 21:09:53.135050 eurlex-parser-0.0.3/
+-rw-rw-rw-   0        0        0     4293 2024-05-31 21:09:53.134048 eurlex-parser-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3751 2024-05-31 21:06:08.000000 eurlex-parser-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 21:09:53.135050 eurlex-parser-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2024-05-31 21:07:41.000000 eurlex-parser-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:09:53.103388 eurlex-parser-0.0.3/src/
+-rw-rw-rw-   0        0        0     9131 2024-05-31 21:02:50.000000 eurlex-parser-0.0.3/src/eurlex.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:09:53.133046 eurlex-parser-0.0.3/src/eurlex_parser.egg-info/
+-rw-rw-rw-   0        0        0     4293 2024-05-31 21:09:53.000000 eurlex-parser-0.0.3/src/eurlex_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-31 21:09:53.000000 eurlex-parser-0.0.3/src/eurlex_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 21:09:53.000000 eurlex-parser-0.0.3/src/eurlex_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-31 21:09:53.000000 eurlex-parser-0.0.3/src/eurlex_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-31 21:09:53.000000 eurlex-parser-0.0.3/src/eurlex_parser.egg-info/top_level.txt
```

### Comparing `eurlex-parser-0.0.2/PKG-INFO` & `eurlex-parser-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurlex-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Eurlex parser for fetching and parsing Eurlex data.
 Home-page: https://github.com/noworneverev/eurlex-parser
 Author: Yan-Ying Liao
 Author-email: n9102125@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -29,14 +29,15 @@
 
 - `get_data_by_celex_id(celex_id: str, language: str = "en") -> dict`: Fetches and parses the data for the given CELEX ID. Returns a dictionary with the document's title, preamble, articles, final part, and annexes.
   
 - `get_json_by_celex_id(celex_id: str) -> str`: Fetches and parses the data for the given CELEX ID and returns it in JSON format.
 
 - `get_articles_by_celex_id(celex_id: str) -> pd.DataFrame`: Fetches and parses the articles for the given CELEX ID and returns them as a Pandas DataFrame.
 
+- `get_summary_by_celex_id(celex_id: str, language: str = "en")` -> dict: Fetches and parses the summary for the given CELEX ID and returns it as a dictionary containing the document's title, chapters, and the last modified date. (Note: The summary is not available for all documents.)
 
 ### Examples
 
 Following are some examples of how to use the functions to fetch and parse data from a CELEX ID. For example, the CELEX ID `32013R0575` corresponds to the following URL: https://eur-lex.europa.eu/legal-content/en/TXT/?uri=celex:32013R0575
 1. Fetch and print data for a given CELEX ID:
     ```python
     from eurlex import get_data_by_celex_id
@@ -57,14 +58,22 @@
 3. Load articles into a Pandas DataFrame:
     ```python
     from eurlex import get_articles_by_celex_id
 
     df = get_articles_by_celex_id('32013R0575')
     print(df.head())
     ```
+4. Fetch and print summary for a given CELEX ID:
+    ```python
+    from eurlex import get_summary_by_celex_id
+
+    summary = get_summary_by_celex_id('32013R0575')
+    print(summary)
+    ```
+
 
 You can find some generated JSON files in the `examples` directory.
 
 ### Data Structure
 
 The main data structure returned by `get_data_by_celex_id` is a dictionary with the following format:
 ```json
@@ -94,23 +103,38 @@
           "id": "1",
           "text": "Note text",
           "url": "https://eur-lex.europa.eu/..."
         }
       ]
     }
   ],
+  "notes": [
+    {
+      "id": "1",
+      "text": "Note text",
+      "url": "https://eur-lex.europa.eu/..."
+    }
+  ],
   "final_part": "Final part text",
   "annexes": [
     {
       "id": "Annex ID",
       "title": "Annex Title",
       "text": "Annex text",
       "table": "Markdown table text"
     }
-  ]
+  ],
+  "summary": {
+    "title": "Document Title",
+    "chapters": {
+      "Chapter Title 1": "Chapter content 1",
+      "Chapter Title 2": "Chapter content 2"
+    },
+    "last_modified": "Last modified date"
+  }
 }
 ```
 
 ### Notes
 
 - The script currently supports fetching data in English (`en`) only.
```

### Comparing `eurlex-parser-0.0.2/README.md` & `eurlex-parser-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 - `get_data_by_celex_id(celex_id: str, language: str = "en") -> dict`: Fetches and parses the data for the given CELEX ID. Returns a dictionary with the document's title, preamble, articles, final part, and annexes.
   
 - `get_json_by_celex_id(celex_id: str) -> str`: Fetches and parses the data for the given CELEX ID and returns it in JSON format.
 
 - `get_articles_by_celex_id(celex_id: str) -> pd.DataFrame`: Fetches and parses the articles for the given CELEX ID and returns them as a Pandas DataFrame.
 
+- `get_summary_by_celex_id(celex_id: str, language: str = "en")` -> dict: Fetches and parses the summary for the given CELEX ID and returns it as a dictionary containing the document's title, chapters, and the last modified date. (Note: The summary is not available for all documents.)
 
 ### Examples
 
 Following are some examples of how to use the functions to fetch and parse data from a CELEX ID. For example, the CELEX ID `32013R0575` corresponds to the following URL: https://eur-lex.europa.eu/legal-content/en/TXT/?uri=celex:32013R0575
 1. Fetch and print data for a given CELEX ID:
     ```python
     from eurlex import get_data_by_celex_id
@@ -42,14 +43,22 @@
 3. Load articles into a Pandas DataFrame:
     ```python
     from eurlex import get_articles_by_celex_id
 
     df = get_articles_by_celex_id('32013R0575')
     print(df.head())
     ```
+4. Fetch and print summary for a given CELEX ID:
+    ```python
+    from eurlex import get_summary_by_celex_id
+
+    summary = get_summary_by_celex_id('32013R0575')
+    print(summary)
+    ```
+
 
 You can find some generated JSON files in the `examples` directory.
 
 ### Data Structure
 
 The main data structure returned by `get_data_by_celex_id` is a dictionary with the following format:
 ```json
@@ -79,23 +88,38 @@
           "id": "1",
           "text": "Note text",
           "url": "https://eur-lex.europa.eu/..."
         }
       ]
     }
   ],
+  "notes": [
+    {
+      "id": "1",
+      "text": "Note text",
+      "url": "https://eur-lex.europa.eu/..."
+    }
+  ],
   "final_part": "Final part text",
   "annexes": [
     {
       "id": "Annex ID",
       "title": "Annex Title",
       "text": "Annex text",
       "table": "Markdown table text"
     }
-  ]
+  ],
+  "summary": {
+    "title": "Document Title",
+    "chapters": {
+      "Chapter Title 1": "Chapter content 1",
+      "Chapter Title 2": "Chapter content 2"
+    },
+    "last_modified": "Last modified date"
+  }
 }
 ```
 
 ### Notes
 
 - The script currently supports fetching data in English (`en`) only.
```

### Comparing `eurlex-parser-0.0.2/setup.py` & `eurlex-parser-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.2'  
+VERSION = '0.0.3'  
 DESCRIPTION  = 'Eurlex parser for fetching and parsing Eurlex data.'
 
 def read_requirements():
     with open('requirements.txt') as req_file:
         return req_file.read().splitlines()
 
 def read_long_description():
```

### Comparing `eurlex-parser-0.0.2/src/eurlex.py` & `eurlex-parser-0.0.3/src/eurlex.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,38 +4,20 @@
 import json
 from src.utils import html_table_to_markdown
 import pandas as pd
 import warnings
 
 warnings.filterwarnings("ignore", category=XMLParsedAsHTMLWarning)
 
-def get_data_by_celex_id(celex_id: str, language: str = "en") -> dict:
-    """
-    Only support English for now
-    """    
-
-    url = f"https://eur-lex.europa.eu/legal-content/{language}/TXT/HTML/?uri=CELEX:{celex_id}"    
-    response = requests.get(url)     
-
-    soup = BeautifulSoup(response.text, 'lxml')
-                       
-    return {
-        'title': parse_title(soup),
-        'preamble': parse_pbl(soup),        
-        'articles': parse_articles(soup),
-        'final_part': parse_fnp(soup),
-        'annexes': parse_annexes(soup)
-    }
-
 def parse_title(soup):
     title_text = ''
     tit_1_div = soup.find('div', id="tit_1")
     if tit_1_div:
         title_text = tit_1_div.text
-        title_text = title_text.replace('\u00a0',' ')
+        title_text = title_text.replace('\u00a0',' ').strip()
     return title_text
 
 def parse_fnp(soup):
     fnp_text = ''
     fnp_1_div = soup.find('div', id="fnp_1")
     if fnp_1_div:
         res = [line for line in fnp_1_div.text.split('\n') if line.strip()]
@@ -176,16 +158,83 @@
             href = second_a_tag.get('href')
             index = href.find("legal-content")
             url = "https://eur-lex.europa.eu/" + href[index:]
         note_dic['url'] = url     
         notes.append(note_dic)
     return notes
 
+def get_summary_by_celex_id(celex_id: str, language: str = "en") -> dict:
+    """
+    Support multiple languages
+    """        
+    url = f"https://eur-lex.europa.eu/legal-content/{language}/LSU/?uri=CELEX:{celex_id}"        
+    response = requests.get(url)     
+
+    soup = BeautifulSoup(response.text, 'lxml')
+
+    # title
+    title_h1 = soup.find("h1", class_="ti-main")
+    title_text = title_h1.text if title_h1 else ''    
+
+    # last modified    
+    lastmod_div = soup.find('p', class_="lastmod")
+    last_modified = lastmod_div.text.strip() if lastmod_div else ''
+        
+    chapter_contents = {}
+    chapters = soup.find_all("h2", class_="ti-chapter")
+    for chapter in chapters:
+        chapter_title = chapter.text.strip()        
+
+        content = []
+        for sibling in chapter.find_next_siblings():
+            if sibling.name == 'h2' and 'ti-chapter' in sibling.get('class', []) or 'lastmod' in sibling.get('class', []):
+                break
+
+            if sibling.name == 'ul':
+                list_items = sibling.find_all('li')
+                for item in list_items:
+                    text = "- " + item.get_text().strip().replace('\xa0', '')
+                    content.append(text)
+            else:
+                content.append(sibling.get_text().replace('\xa0', ''))
+        
+        chapter_contents[chapter_title] = '\n'.join(content)    
+
+    return {
+        'title': title_text,        
+        'chapters': chapter_contents,
+        'last_modified': last_modified
+    }
+
+
+def get_data_by_celex_id(celex_id: str, language: str = "en") -> dict:
+    """
+    Only support English for now
+    """    
+
+    url = f"https://eur-lex.europa.eu/legal-content/{language}/TXT/HTML/?uri=CELEX:{celex_id}"    
+    response = requests.get(url)     
+
+    soup = BeautifulSoup(response.text, 'lxml')
+        
+    preamble = parse_pbl(soup)
+    articles = parse_articles(soup)
+    article_notes = [note for article in articles for note in article["notes"]]
+        
+    return {
+        'title': parse_title(soup),
+        'preamble': preamble,
+        'articles': articles,
+        'final_part': parse_fnp(soup),
+        'notes': preamble["notes"] + article_notes,
+        'annexes': parse_annexes(soup),
+        'summary': get_summary_by_celex_id(celex_id, language)
+    }
 
 def get_json_by_celex_id(celex_id) -> str:
     data = get_data_by_celex_id(celex_id)
     return json.dumps(data, indent=4)
 
 def get_articles_by_celex_id(celex_id) -> pd.DataFrame:
     data = get_data_by_celex_id(celex_id)
     articles = data['articles']
-    return pd.DataFrame(articles, columns=["id", "title", "text", "metadata", "notes"])
+    return pd.DataFrame(articles, columns=["id", "title", "text", "metadata", "notes"])
```

### Comparing `eurlex-parser-0.0.2/src/eurlex_parser.egg-info/PKG-INFO` & `eurlex-parser-0.0.3/src/eurlex_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurlex-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Eurlex parser for fetching and parsing Eurlex data.
 Home-page: https://github.com/noworneverev/eurlex-parser
 Author: Yan-Ying Liao
 Author-email: n9102125@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -29,14 +29,15 @@
 
 - `get_data_by_celex_id(celex_id: str, language: str = "en") -> dict`: Fetches and parses the data for the given CELEX ID. Returns a dictionary with the document's title, preamble, articles, final part, and annexes.
   
 - `get_json_by_celex_id(celex_id: str) -> str`: Fetches and parses the data for the given CELEX ID and returns it in JSON format.
 
 - `get_articles_by_celex_id(celex_id: str) -> pd.DataFrame`: Fetches and parses the articles for the given CELEX ID and returns them as a Pandas DataFrame.
 
+- `get_summary_by_celex_id(celex_id: str, language: str = "en")` -> dict: Fetches and parses the summary for the given CELEX ID and returns it as a dictionary containing the document's title, chapters, and the last modified date. (Note: The summary is not available for all documents.)
 
 ### Examples
 
 Following are some examples of how to use the functions to fetch and parse data from a CELEX ID. For example, the CELEX ID `32013R0575` corresponds to the following URL: https://eur-lex.europa.eu/legal-content/en/TXT/?uri=celex:32013R0575
 1. Fetch and print data for a given CELEX ID:
     ```python
     from eurlex import get_data_by_celex_id
@@ -57,14 +58,22 @@
 3. Load articles into a Pandas DataFrame:
     ```python
     from eurlex import get_articles_by_celex_id
 
     df = get_articles_by_celex_id('32013R0575')
     print(df.head())
     ```
+4. Fetch and print summary for a given CELEX ID:
+    ```python
+    from eurlex import get_summary_by_celex_id
+
+    summary = get_summary_by_celex_id('32013R0575')
+    print(summary)
+    ```
+
 
 You can find some generated JSON files in the `examples` directory.
 
 ### Data Structure
 
 The main data structure returned by `get_data_by_celex_id` is a dictionary with the following format:
 ```json
@@ -94,23 +103,38 @@
           "id": "1",
           "text": "Note text",
           "url": "https://eur-lex.europa.eu/..."
         }
       ]
     }
   ],
+  "notes": [
+    {
+      "id": "1",
+      "text": "Note text",
+      "url": "https://eur-lex.europa.eu/..."
+    }
+  ],
   "final_part": "Final part text",
   "annexes": [
     {
       "id": "Annex ID",
       "title": "Annex Title",
       "text": "Annex text",
       "table": "Markdown table text"
     }
-  ]
+  ],
+  "summary": {
+    "title": "Document Title",
+    "chapters": {
+      "Chapter Title 1": "Chapter content 1",
+      "Chapter Title 2": "Chapter content 2"
+    },
+    "last_modified": "Last modified date"
+  }
 }
 ```
 
 ### Notes
 
 - The script currently supports fetching data in English (`en`) only.
```

