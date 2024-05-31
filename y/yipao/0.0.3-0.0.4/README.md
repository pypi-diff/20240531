# Comparing `tmp/yipao-0.0.3.tar.gz` & `tmp/yipao-0.0.4.tar.gz`

## Comparing `yipao-0.0.3.tar` & `yipao-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/LLM/__init__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/LLM/customllm.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/LLM/gemini.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/LLM/vertex.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/agent/__init__.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/agent/core.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/databases/__init__.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/databases/mysql.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/prompts/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/prompts/builder.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/prompts/prompts.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/retrievers/__init__.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/retrievers/vectorStoreRetriever.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/utils/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/utils/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/utils/logger.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/utils/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/vectorstores/__init__.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/vectorstores/chromadb.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 yipao-0.0.3/yipao/vectorstores/qdrant.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 yipao-0.0.3/.gitignore
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 yipao-0.0.3/README.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 yipao-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 yipao-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/LLM/__init__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/LLM/customllm.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/LLM/gemini.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/LLM/vertex.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/agent/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/agent/core.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/databases/__init__.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/databases/mysql.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/prompts/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/prompts/builder.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/prompts/prompts.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/retrievers/__init__.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/retrievers/vectorStoreRetriever.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/utils/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/utils/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/utils/logger.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/utils/utils.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/vectorstores/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/vectorstores/chromadb.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 yipao-0.0.4/yipao/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 yipao-0.0.4/.gitignore
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 yipao-0.0.4/README.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 yipao-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 yipao-0.0.4/PKG-INFO
```

### Comparing `yipao-0.0.3/yipao/LLM/customllm.py` & `yipao-0.0.4/yipao/LLM/customllm.py`

 * *Files identical despite different names*

### Comparing `yipao-0.0.3/yipao/LLM/vertex.py` & `yipao-0.0.4/yipao/LLM/vertex.py`

 * *Files identical despite different names*

### Comparing `yipao-0.0.3/yipao/agent/core.py` & `yipao-0.0.4/yipao/agent/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         vectorstore: The storage for vector embeddings of SQL statements.
         retriever (VectorStoreRetriever): A retriever for related data definitions.
         promptBuilder (PromptBuilder): A builder for creating SQL prompts.
         history (str): A record of executed SQL queries.
     """
 
 
-    def __init__(self, llm: CustomLLM, database, vectorstore, name_collection):
+    def __init__(self, llm: CustomLLM, database, vectorstore, name_collection = 'ddl'):
         """
         Initializes the Agent with a language model, database, and vector store.
 
         Args:
             llm (CustomLLM): The language model used to generate SQL queries.
             database: The database interface to execute SQL queries.
             vectorstore: The vector store interface for saving SQL statement embeddings.
```

### Comparing `yipao-0.0.3/yipao/databases/mysql.py` & `yipao-0.0.4/yipao/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `yipao-0.0.3/yipao/prompts/builder.py` & `yipao-0.0.4/yipao/prompts/builder.py`

 * *Files identical despite different names*

### Comparing `yipao-0.0.3/yipao/prompts/prompts.py` & `yipao-0.0.4/yipao/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `yipao-0.0.3/yipao/retrievers/vectorStoreRetriever.py` & `yipao-0.0.4/yipao/retrievers/vectorStoreRetriever.py`

 * *Files identical despite different names*

### Comparing `yipao-0.0.3/yipao/utils/constants.py` & `yipao-0.0.4/yipao/utils/constants.py`

 * *Files identical despite different names*

### Comparing `yipao-0.0.3/yipao/vectorstores/chromadb.py` & `yipao-0.0.4/yipao/vectorstores/chromadb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import chromadb
-from chromadb.config import Settings
-from chromadb.utils import embedding_functions
 import uuid
 from typing import Dict 
 
 class ChromaDB:
+
+
     """
     Class for interacting with ChromaDB, a database designed for handling and querying embedded documents.
 
     Attributes:
         client (PersistentClient or HttpClient): The database client for interacting with ChromaDB.
         ddl_collection (Collection): A collection for DDL (Data Definition Language) statements.
     """
@@ -20,15 +19,22 @@
         Args:
             cfg (Dict[str, int] or str): If string, it represents the file path to the database;
                                          if dictionary, it specifies configuration settings for HTTP connection.
             settings (dict): Additional settings for the ChromaDB client, passed to the Settings object.
 
         Raises:
             TypeError: If cfg is neither a dict nor a string.
-        """
+        """ 
+        try: 
+            import chromadb
+            from chromadb.config import Settings
+            from chromadb.utils import embedding_functions
+        except ImportError:
+            raise ImportError("Please install the chromadb package using 'pip install chromadb'")
+        
         if isinstance(cfg, str):
             self.client = chromadb.PersistentClient(path=cfg, settings=Settings(**settings))
         elif isinstance(cfg, Dict):
             self.client = chromadb.HttpClient(**cfg, settings=Settings(**settings))
         else:
             raise TypeError("Configuration must be either a path (str) or settings (dict).")
```

### Comparing `yipao-0.0.3/yipao/vectorstores/qdrant.py` & `yipao-0.0.4/yipao/vectorstores/qdrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 class QdrantDB:
     """
     Class for interacting with Qdrant, a vector store designed for handling and querying embedded documents.
 
 
     """
-    def __init__(self, cfg: str, api_key: str=None, embedding_model: str="sentence-transformers/all-MiniLM-L6-v2"):
+    def __init__(self, cfg: str, api_key: str=None, embedding_model: str="sentence-transformers/all-MiniLM-L6-v2", name_collection:str = 'ddl'):
         """
         Initializes the Qdrant client based on configuration.
 
         Args:
             cfg (str): Can be ":memory:", "/path/to/db" or "http://host:port".
             api_key (str): The API key for the Qdrant client (default is None).
 
         Raises:
             TypeError: If cfg is not a string.
         """
         self.client = QdrantClient(cfg, api_key=api_key)
         self.client.set_model(embedding_model)
+        self.initialize(name_collection)
         print(f"Qdrant client initialized with Embedding-Model: {embedding_model}")
 
     
     def initialize(self, name_collection: str):
         """
         Initializes the Qdrant client.
         """
```

### Comparing `yipao-0.0.3/README.md` & `yipao-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,40 +28,41 @@
 ```python
 import os
 from dotenv import load_dotenv
 load_dotenv()
 
 import yipao as yp
 from yipao.databases import MySql
-from yipao.vectorstores import ChromaDB
+from yipao.vectorstores import QdrantDB
 from yipao.LLM import GoogleGenAi
 
 connection = {
     'host': os.getenv('HOST'),
     'user': os.getenv('USERDB'),
     'password': os.getenv('PASSWORD'),
     'database': os.getenv('DATABASE'),
     'port': int(os.getenv('PORT'))
 }
 
 mysql = MySql(**connection)
 
-chroma = ChromaDB(path='vectorstore', allow_reset=True)
+qdrant =  QdrantDB(':memory:')
 
 gemini = GoogleGenAi(model='gemini-pro', api_key=os.getenv('APIKEYGEMINI'))
 
 agent = yp.Agent(llm=gemini, 
                  database=mysql, 
-                 vectorstore=chroma)
+                 vectorstore=qdrant)
 
 agent.document_database()
 
 prompt = f"What is my best selling product?"
 
 res = agent.invoke(prompt)
 
+print(res)
 # your best products are...
 ```
 
 # Contributing 👋
 
 Want to help improve Yipao? Contributions are welcome! 🎉
```

### Comparing `yipao-0.0.3/PKG-INFO` & `yipao-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.3
 Name: yipao
-Version: 0.0.3
+Version: 0.0.4
 Summary: Yipao is a library enabling AI-driven interactions with SQL databases, facilitating dynamic SQL query generation and execution.
+Project-URL: Homepage, https://facil-pos.github.io/yipao/
+Project-URL: Development, https://github.com/facil-pos/yipao
 Author-email: factral <nelsonfabiancs8@gmail.com>, Daniel <manosalvasierra@gmail.com>
+License: MIT License
 Keywords: ai,database,dynamic,execution,generation,query,rag,sql
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3
-Requires-Dist: chromadb
 Requires-Dist: google-generativeai
 Requires-Dist: pandas
 Requires-Dist: pymysql
-Requires-Dist: python-dotenv
 Requires-Dist: qdrant-client[fastembed]
-Requires-Dist: tabulate
 Requires-Dist: vertexai
+Provides-Extra: chroma
+Requires-Dist: chromadb; extra == 'chroma'
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-autodoc-annotation; extra == 'doc'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
 Requires-Dist: sphinxawesome-theme; extra == 'doc'
 Description-Content-Type: text/markdown
 
@@ -50,40 +61,41 @@
 ```python
 import os
 from dotenv import load_dotenv
 load_dotenv()
 
 import yipao as yp
 from yipao.databases import MySql
-from yipao.vectorstores import ChromaDB
+from yipao.vectorstores import QdrantDB
 from yipao.LLM import GoogleGenAi
 
 connection = {
     'host': os.getenv('HOST'),
     'user': os.getenv('USERDB'),
     'password': os.getenv('PASSWORD'),
     'database': os.getenv('DATABASE'),
     'port': int(os.getenv('PORT'))
 }
 
 mysql = MySql(**connection)
 
-chroma = ChromaDB(path='vectorstore', allow_reset=True)
+qdrant =  QdrantDB(':memory:')
 
 gemini = GoogleGenAi(model='gemini-pro', api_key=os.getenv('APIKEYGEMINI'))
 
 agent = yp.Agent(llm=gemini, 
                  database=mysql, 
-                 vectorstore=chroma)
+                 vectorstore=qdrant)
 
 agent.document_database()
 
 prompt = f"What is my best selling product?"
 
 res = agent.invoke(prompt)
 
+print(res)
 # your best products are...
 ```
 
 # Contributing 👋
 
 Want to help improve Yipao? Contributions are welcome! 🎉
```

