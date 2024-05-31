# Comparing `tmp/rag_cli-0.2.4.tar.gz` & `tmp/rag_cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_cli-0.2.4.tar", max compression
+gzip compressed data, was "rag_cli-0.2.5.tar", max compression
```

## Comparing `rag_cli-0.2.4.tar` & `rag_cli-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2024-05-18 23:12:26.306548 rag_cli-0.2.4/LICENSE
--rw-r--r--   0        0        0     4571 2024-05-18 23:12:26.306548 rag_cli-0.2.4/README.md
--rw-r--r--   0        0        0     2755 2024-05-18 23:12:26.310548 rag_cli-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-18 23:12:26.310548 rag_cli-0.2.4/src/rag_cli/__init__.py
--rw-r--r--   0        0        0     2562 2024-05-18 23:12:26.310548 rag_cli-0.2.4/src/rag_cli/cli.py
--rw-r--r--   0        0        0     1067 2024-05-18 23:12:26.310548 rag_cli-0.2.4/src/rag_cli/embedder.py
--rw-r--r--   0        0        0      859 2024-05-18 23:12:26.310548 rag_cli-0.2.4/src/rag_cli/main.py
--rw-r--r--   0        0        0      983 2024-05-18 23:12:26.310548 rag_cli-0.2.4/src/rag_cli/vector_store.py
--rw-r--r--   0        0        0     5352 1970-01-01 00:00:00.000000 rag_cli-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-31 20:55:22.336185 rag_cli-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5898 2024-05-31 20:55:22.336185 rag_cli-0.2.5/README.md
+-rw-r--r--   0        0        0     2755 2024-05-31 20:55:22.336185 rag_cli-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 20:55:22.336185 rag_cli-0.2.5/src/rag_cli/__init__.py
+-rw-r--r--   0        0        0     3721 2024-05-31 20:55:22.336185 rag_cli-0.2.5/src/rag_cli/cli.py
+-rw-r--r--   0        0        0     1067 2024-05-31 20:55:22.336185 rag_cli-0.2.5/src/rag_cli/embedder.py
+-rw-r--r--   0        0        0     1451 2024-05-31 20:55:22.336185 rag_cli-0.2.5/src/rag_cli/main.py
+-rw-r--r--   0        0        0     2898 2024-05-31 20:55:22.336185 rag_cli-0.2.5/src/rag_cli/rag.py
+-rw-r--r--   0        0        0      983 2024-05-31 20:55:22.336185 rag_cli-0.2.5/src/rag_cli/vector_store.py
+-rw-r--r--   0        0        0     6679 1970-01-01 00:00:00.000000 rag_cli-0.2.5/PKG-INFO
```

### Comparing `rag_cli-0.2.4/LICENSE` & `rag_cli-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rag_cli-0.2.4/README.md` & `rag_cli-0.2.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 - Vector store (Qdrant)
 
 ## Usage
 
 ### Docker
 
 If you don't have a running instance of [Qdrant](https://qdrant.tech/) or [Ollama](https://ollama.com/), you can use the provided docker-compose file to start one.
-  
+
 ```bash
 docker-compose up --build -d
 ```
 
 This will start Ollama on `http://localhost:11434` and Qdrant on `http://localhost:6333`.
 
 #### Development
@@ -86,17 +86,42 @@
 cat <INPUT_FILE> | \
 rag-cli vector-store \
 --qdrant-url http://localhost:6333 \
 --collection-name <COLLECTION_NAME> \
 --data '{<JSON_DATA>}'
 ```
 
-### End-to-end Pipeline
+### RAG Chat
+
+```bash
+rag-cli rag \
+--ollama-embedding-url http://localhost:11434 \
+--ollama-chat-url http://localhost:11435 \
+--qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \
+--top-k 5 \
+--min-similarity 0.5
+--file <INPUT_FILE>
+```
+
+You can alternatively use stdin to pass the text:
+
+```bash
+cat <INPUT_FILE> | \
+--ollama-embedding-url http://localhost:11434 \
+--ollama-chat-url http://localhost:11435 \
+--qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \
+--top-k 5 \
+--min-similarity 0.5
+```
 
-Here is an example of an end-to-end pipeline. It takes the following steps:
+### End-to-end Pipeline For Storing Embeddings
+
+Here is an example of an end-to-end pipeline for storing embeddings. It takes the following steps:
 
 - Get a random Wikipedia article
 - Embed the article
 - Store the embedding in Qdrant
 
 Before running the pipeline make sure you have the following installed:
 
@@ -148,16 +173,37 @@
 
 ### Store All Embeddings In Qdrant
 
 ```bash
 parallel rag-cli vector-store --qdrant-url http://localhost:6333 --collection-name nomic-embed-text-v1.5 2>> output.log ::: $(find data/embeddings/*)
 ```
 
+### Run RAG Chat On A Query
+
+```bash
+echo "Who invented the blue LED?" | \
+rag-cli rag \
+--ollama-embedding-url http://localhost:11434 \
+--ollama-chat-url http://localhost:11435 \
+--qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \
+--top-k 5 \
+--min-similarity 0.5 \
+2>> output.log
+```
+
+This example obviously requires that the articles similar to the query have been embedded and stored in Qdrant. You can do this with the example found in the next section.
+
 ### End-to-end Pipeline For A Single Article
 
 ```bash
-curl -L -s "https://en.wikipedia.org/api/rest_v1/page/random/summary" | \
-jq -r ".title, .description, .extract" | \
+wikipedia_data=$(curl -L -s "https://en.wikipedia.org/api/rest_v1/page/summary/Shuji_Nakamura") && \
+payload_data=$(jq "{title: .title, description: .description, extract: .extract}"  <(echo $wikipedia_data)) && \
+text_to_embed=$(jq -r ".title, .description, .extract" <(echo $wikipedia_data)) && \
+echo $text_to_embed | \
 rag-cli embed --ollama-url http://localhost:11434 | \
-jq ".embedding" | \
-rag-cli vector-store --qdrant-url http://localhost:6333 --collection-name nomic-embed-text-v1.5
+jq -r ".embedding" | \
+rag-cli vector-store \
+  --qdrant-url http://localhost:6333 \
+  --collection-name nomic-embed-text-v1.5 \
+  --data "$payload_data"
 ```
```

#### html2text {}

```diff
@@ -22,31 +22,48 @@
 is available: ```bash ollama pull nomic-embed-text:v1.5 ``` ```bash rag-cli
 embed --ollama-url http://localhost:11434 --file ``` You can alternatively use
 stdin to pass the text: ```bash cat | rag-cli embed --ollama-url http://
 localhost:11434 ``` ### Vector store ```bash rag-cli vector-store \ --qdrant-
 url http://localhost:6333 \ --collection-name \ --data '{}' --embedding ``` You
 can alternatively use stdin to pass embeddings: ```bash cat | \ rag-cli vector-
 store \ --qdrant-url http://localhost:6333 \ --collection-name \ --data '{}'
-``` ### End-to-end Pipeline Here is an example of an end-to-end pipeline. It
-takes the following steps: - Get a random Wikipedia article - Embed the article
-- Store the embedding in Qdrant Before running the pipeline make sure you have
-the following installed: ```bash sudo apt-get update && sudo apt-get install
-parallel jq curl ``` Also make sure that the `data/articles` and `data/
-embeddings` directories exist: ```bash mkdir -p data/articles data/embeddings
-``` Then run the pipeline: ```bash bash scripts/run_pipeline.sh ``` ####
-Parallel Pipeline The script `scripts/run_pipeline.sh` can be run in parallel
-with [GNU Parallel](https://www.gnu.org/software/parallel/) to speed up the
-process. ```bash parallel -j 5 -n0 bash scripts/run_pipeline.sh ::: {0..10} ```
-## Examples ### Get 10 Random Wikipedia Articles ```bash parallel -n0 -j 10 '
-curl -L -s "https://en.wikipedia.org/api/rest_v1/page/random/summary" | \ jq -
-r ".title, .description, .extract" | \ tee data/articles/$(cat /proc/sys/
-kernel/random/uuid).txt ' ::: {0..10} ``` ### Run Embedder On All Articles
-```bash parallel ' rag-cli embed --ollama-url http://localhost:11434 --file {1}
-2>> output.log | \ jq ".embedding" | \ tee data/embeddings/$(basename {1} .txt)
-1> /dev/null ' ::: $(find data/articles/*.txt) ``` ### Store All Embeddings In
-Qdrant ```bash parallel rag-cli vector-store --qdrant-url http://localhost:6333
---collection-name nomic-embed-text-v1.5 2>> output.log ::: $(find data/
-embeddings/*) ``` ### End-to-end Pipeline For A Single Article ```bash curl -
-L -s "https://en.wikipedia.org/api/rest_v1/page/random/summary" | \ jq -
-r ".title, .description, .extract" | \ rag-cli embed --ollama-url http://
-localhost:11434 | \ jq ".embedding" | \ rag-cli vector-store --qdrant-url http:
-//localhost:6333 --collection-name nomic-embed-text-v1.5 ```
+``` ### RAG Chat ```bash rag-cli rag \ --ollama-embedding-url http://localhost:
+11434 \ --ollama-chat-url http://localhost:11435 \ --qdrant-url http://
+localhost:6333 \ --collection-name nomic-embed-text-v1.5 \ --top-k 5 \ --min-
+similarity 0.5 --file ``` You can alternatively use stdin to pass the text:
+```bash cat | \ --ollama-embedding-url http://localhost:11434 \ --ollama-chat-
+url http://localhost:11435 \ --qdrant-url http://localhost:6333 \ --collection-
+name nomic-embed-text-v1.5 \ --top-k 5 \ --min-similarity 0.5 ``` ### End-to-
+end Pipeline For Storing Embeddings Here is an example of an end-to-end
+pipeline for storing embeddings. It takes the following steps: - Get a random
+Wikipedia article - Embed the article - Store the embedding in Qdrant Before
+running the pipeline make sure you have the following installed: ```bash sudo
+apt-get update && sudo apt-get install parallel jq curl ``` Also make sure that
+the `data/articles` and `data/embeddings` directories exist: ```bash mkdir -
+p data/articles data/embeddings ``` Then run the pipeline: ```bash bash
+scripts/run_pipeline.sh ``` #### Parallel Pipeline The script `scripts/
+run_pipeline.sh` can be run in parallel with [GNU Parallel](https://
+www.gnu.org/software/parallel/) to speed up the process. ```bash parallel -j 5
+-n0 bash scripts/run_pipeline.sh ::: {0..10} ``` ## Examples ### Get 10 Random
+Wikipedia Articles ```bash parallel -n0 -j 10 ' curl -L -s "https://
+en.wikipedia.org/api/rest_v1/page/random/summary" | \ jq -r ".title,
+.description, .extract" | \ tee data/articles/$(cat /proc/sys/kernel/random/
+uuid).txt ' ::: {0..10} ``` ### Run Embedder On All Articles ```bash parallel '
+rag-cli embed --ollama-url http://localhost:11434 --file {1} 2>> output.log | \
+jq ".embedding" | \ tee data/embeddings/$(basename {1} .txt) 1> /dev/null ' :::
+$(find data/articles/*.txt) ``` ### Store All Embeddings In Qdrant ```bash
+parallel rag-cli vector-store --qdrant-url http://localhost:6333 --collection-
+name nomic-embed-text-v1.5 2>> output.log ::: $(find data/embeddings/*) ``` ###
+Run RAG Chat On A Query ```bash echo "Who invented the blue LED?" | \ rag-cli
+rag \ --ollama-embedding-url http://localhost:11434 \ --ollama-chat-url http://
+localhost:11435 \ --qdrant-url http://localhost:6333 \ --collection-name nomic-
+embed-text-v1.5 \ --top-k 5 \ --min-similarity 0.5 \ 2>> output.log ``` This
+example obviously requires that the articles similar to the query have been
+embedded and stored in Qdrant. You can do this with the example found in the
+next section. ### End-to-end Pipeline For A Single Article ```bash
+wikipedia_data=$(curl -L -s "https://en.wikipedia.org/api/rest_v1/page/summary/
+Shuji_Nakamura") && \ payload_data=$(jq "{title: .title, description:
+.description, extract: .extract}" <(echo $wikipedia_data)) && \ text_to_embed=$
+(jq -r ".title, .description, .extract" <(echo $wikipedia_data)) && \ echo
+$text_to_embed | \ rag-cli embed --ollama-url http://localhost:11434 | \ jq -
+r ".embedding" | \ rag-cli vector-store \ --qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \ --data "$payload_data" ```
```

### Comparing `rag_cli-0.2.4/pyproject.toml` & `rag_cli-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rag-cli"
-version = "0.2.4"
+version = "0.2.5"
 description = "A project to show good CLI practices with a fully fledged RAG system."
 readme = "README.md"
 license = "GNU GPL v3"
 keywords = ["CLI", "RAG", "LLM", "vector database", "ollama"]
 authors = ["Oliver Kenyon Wilkins <okwilkins@googlemail.com>"]
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3",
```

### Comparing `rag_cli-0.2.4/src/rag_cli/cli.py` & `rag_cli-0.2.5/src/rag_cli/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -87,8 +87,60 @@
         "embedding",
         help="File with embedding to store. Must be a list of floats in the form [0.1, 0.2, ...] (default: stdin)",
         type=argparse.FileType('r'),
         nargs="?",
         default=sys.stdin,
     )
 
+    rag_parser = subparsers.add_parser(
+        "rag",
+        help="Runs the RAG system.",
+    )
+
+    rag_parser.add_argument(
+        "--ollama-embedding-url",
+        help="The URL of the Ollama embedding server.",
+        type=str,
+    )
+
+    rag_parser.add_argument(
+        "--ollama-chat-url",
+        help="The URL of the Ollama chat server.",
+        type=str,
+    )
+
+    rag_parser.add_argument(
+        "--qdrant-url",
+        help="The URL of the Qdrant server.",
+        type=str,
+    )
+
+    rag_parser.add_argument(
+        "--collection-name",
+        help="The name of the collection.",
+        type=str,
+    )
+
+    rag_parser.add_argument(
+        "--top-k",
+        help="The number of similar vectors to return.",
+        type=int,
+        default=5,
+    )
+
+    rag_parser.add_argument(
+        "--min-similarity",
+        help="The minimum similarity to return.",
+        type=float,
+        default=0.5,
+    )
+
+    # Add optional stdin argument
+    rag_parser.add_argument(
+        '--file',
+        nargs='?',
+        type=argparse.FileType('r'),
+        default=sys.stdin,
+        help='Input file to chat with (default: stdin)'
+    )
+
     return parser.parse_args()
```

### Comparing `rag_cli-0.2.4/src/rag_cli/embedder.py` & `rag_cli-0.2.5/src/rag_cli/embedder.py`

 * *Files identical despite different names*

### Comparing `rag_cli-0.2.4/src/rag_cli/vector_store.py` & `rag_cli-0.2.5/src/rag_cli/vector_store.py`

 * *Files identical despite different names*

### Comparing `rag_cli-0.2.4/PKG-INFO` & `rag_cli-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: A project to show good CLI practices with a fully fledged RAG system.
 License: GNU GPL v3
 Keywords: CLI,RAG,LLM,vector database,ollama
 Author: Oliver Kenyon Wilkins
 Author-email: okwilkins@googlemail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -47,15 +47,15 @@
 - Vector store (Qdrant)
 
 ## Usage
 
 ### Docker
 
 If you don't have a running instance of [Qdrant](https://qdrant.tech/) or [Ollama](https://ollama.com/), you can use the provided docker-compose file to start one.
-  
+
 ```bash
 docker-compose up --build -d
 ```
 
 This will start Ollama on `http://localhost:11434` and Qdrant on `http://localhost:6333`.
 
 #### Development
@@ -106,17 +106,42 @@
 cat <INPUT_FILE> | \
 rag-cli vector-store \
 --qdrant-url http://localhost:6333 \
 --collection-name <COLLECTION_NAME> \
 --data '{<JSON_DATA>}'
 ```
 
-### End-to-end Pipeline
+### RAG Chat
+
+```bash
+rag-cli rag \
+--ollama-embedding-url http://localhost:11434 \
+--ollama-chat-url http://localhost:11435 \
+--qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \
+--top-k 5 \
+--min-similarity 0.5
+--file <INPUT_FILE>
+```
+
+You can alternatively use stdin to pass the text:
+
+```bash
+cat <INPUT_FILE> | \
+--ollama-embedding-url http://localhost:11434 \
+--ollama-chat-url http://localhost:11435 \
+--qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \
+--top-k 5 \
+--min-similarity 0.5
+```
 
-Here is an example of an end-to-end pipeline. It takes the following steps:
+### End-to-end Pipeline For Storing Embeddings
+
+Here is an example of an end-to-end pipeline for storing embeddings. It takes the following steps:
 
 - Get a random Wikipedia article
 - Embed the article
 - Store the embedding in Qdrant
 
 Before running the pipeline make sure you have the following installed:
 
@@ -168,17 +193,38 @@
 
 ### Store All Embeddings In Qdrant
 
 ```bash
 parallel rag-cli vector-store --qdrant-url http://localhost:6333 --collection-name nomic-embed-text-v1.5 2>> output.log ::: $(find data/embeddings/*)
 ```
 
+### Run RAG Chat On A Query
+
+```bash
+echo "Who invented the blue LED?" | \
+rag-cli rag \
+--ollama-embedding-url http://localhost:11434 \
+--ollama-chat-url http://localhost:11435 \
+--qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \
+--top-k 5 \
+--min-similarity 0.5 \
+2>> output.log
+```
+
+This example obviously requires that the articles similar to the query have been embedded and stored in Qdrant. You can do this with the example found in the next section.
+
 ### End-to-end Pipeline For A Single Article
 
 ```bash
-curl -L -s "https://en.wikipedia.org/api/rest_v1/page/random/summary" | \
-jq -r ".title, .description, .extract" | \
+wikipedia_data=$(curl -L -s "https://en.wikipedia.org/api/rest_v1/page/summary/Shuji_Nakamura") && \
+payload_data=$(jq "{title: .title, description: .description, extract: .extract}"  <(echo $wikipedia_data)) && \
+text_to_embed=$(jq -r ".title, .description, .extract" <(echo $wikipedia_data)) && \
+echo $text_to_embed | \
 rag-cli embed --ollama-url http://localhost:11434 | \
-jq ".embedding" | \
-rag-cli vector-store --qdrant-url http://localhost:6333 --collection-name nomic-embed-text-v1.5
+jq -r ".embedding" | \
+rag-cli vector-store \
+  --qdrant-url http://localhost:6333 \
+  --collection-name nomic-embed-text-v1.5 \
+  --data "$payload_data"
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rag-cli Version: 0.2.4 Summary: A project to show
+Metadata-Version: 2.1 Name: rag-cli Version: 0.2.5 Summary: A project to show
 good CLI practices with a fully fledged RAG system. License: GNU GPL v3
 Keywords: CLI,RAG,LLM,vector database,ollama Author: Oliver Kenyon Wilkins
 Author-email: okwilkins@googlemail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -33,31 +33,48 @@
 is available: ```bash ollama pull nomic-embed-text:v1.5 ``` ```bash rag-cli
 embed --ollama-url http://localhost:11434 --file ``` You can alternatively use
 stdin to pass the text: ```bash cat | rag-cli embed --ollama-url http://
 localhost:11434 ``` ### Vector store ```bash rag-cli vector-store \ --qdrant-
 url http://localhost:6333 \ --collection-name \ --data '{}' --embedding ``` You
 can alternatively use stdin to pass embeddings: ```bash cat | \ rag-cli vector-
 store \ --qdrant-url http://localhost:6333 \ --collection-name \ --data '{}'
-``` ### End-to-end Pipeline Here is an example of an end-to-end pipeline. It
-takes the following steps: - Get a random Wikipedia article - Embed the article
-- Store the embedding in Qdrant Before running the pipeline make sure you have
-the following installed: ```bash sudo apt-get update && sudo apt-get install
-parallel jq curl ``` Also make sure that the `data/articles` and `data/
-embeddings` directories exist: ```bash mkdir -p data/articles data/embeddings
-``` Then run the pipeline: ```bash bash scripts/run_pipeline.sh ``` ####
-Parallel Pipeline The script `scripts/run_pipeline.sh` can be run in parallel
-with [GNU Parallel](https://www.gnu.org/software/parallel/) to speed up the
-process. ```bash parallel -j 5 -n0 bash scripts/run_pipeline.sh ::: {0..10} ```
-## Examples ### Get 10 Random Wikipedia Articles ```bash parallel -n0 -j 10 '
-curl -L -s "https://en.wikipedia.org/api/rest_v1/page/random/summary" | \ jq -
-r ".title, .description, .extract" | \ tee data/articles/$(cat /proc/sys/
-kernel/random/uuid).txt ' ::: {0..10} ``` ### Run Embedder On All Articles
-```bash parallel ' rag-cli embed --ollama-url http://localhost:11434 --file {1}
-2>> output.log | \ jq ".embedding" | \ tee data/embeddings/$(basename {1} .txt)
-1> /dev/null ' ::: $(find data/articles/*.txt) ``` ### Store All Embeddings In
-Qdrant ```bash parallel rag-cli vector-store --qdrant-url http://localhost:6333
---collection-name nomic-embed-text-v1.5 2>> output.log ::: $(find data/
-embeddings/*) ``` ### End-to-end Pipeline For A Single Article ```bash curl -
-L -s "https://en.wikipedia.org/api/rest_v1/page/random/summary" | \ jq -
-r ".title, .description, .extract" | \ rag-cli embed --ollama-url http://
-localhost:11434 | \ jq ".embedding" | \ rag-cli vector-store --qdrant-url http:
-//localhost:6333 --collection-name nomic-embed-text-v1.5 ```
+``` ### RAG Chat ```bash rag-cli rag \ --ollama-embedding-url http://localhost:
+11434 \ --ollama-chat-url http://localhost:11435 \ --qdrant-url http://
+localhost:6333 \ --collection-name nomic-embed-text-v1.5 \ --top-k 5 \ --min-
+similarity 0.5 --file ``` You can alternatively use stdin to pass the text:
+```bash cat | \ --ollama-embedding-url http://localhost:11434 \ --ollama-chat-
+url http://localhost:11435 \ --qdrant-url http://localhost:6333 \ --collection-
+name nomic-embed-text-v1.5 \ --top-k 5 \ --min-similarity 0.5 ``` ### End-to-
+end Pipeline For Storing Embeddings Here is an example of an end-to-end
+pipeline for storing embeddings. It takes the following steps: - Get a random
+Wikipedia article - Embed the article - Store the embedding in Qdrant Before
+running the pipeline make sure you have the following installed: ```bash sudo
+apt-get update && sudo apt-get install parallel jq curl ``` Also make sure that
+the `data/articles` and `data/embeddings` directories exist: ```bash mkdir -
+p data/articles data/embeddings ``` Then run the pipeline: ```bash bash
+scripts/run_pipeline.sh ``` #### Parallel Pipeline The script `scripts/
+run_pipeline.sh` can be run in parallel with [GNU Parallel](https://
+www.gnu.org/software/parallel/) to speed up the process. ```bash parallel -j 5
+-n0 bash scripts/run_pipeline.sh ::: {0..10} ``` ## Examples ### Get 10 Random
+Wikipedia Articles ```bash parallel -n0 -j 10 ' curl -L -s "https://
+en.wikipedia.org/api/rest_v1/page/random/summary" | \ jq -r ".title,
+.description, .extract" | \ tee data/articles/$(cat /proc/sys/kernel/random/
+uuid).txt ' ::: {0..10} ``` ### Run Embedder On All Articles ```bash parallel '
+rag-cli embed --ollama-url http://localhost:11434 --file {1} 2>> output.log | \
+jq ".embedding" | \ tee data/embeddings/$(basename {1} .txt) 1> /dev/null ' :::
+$(find data/articles/*.txt) ``` ### Store All Embeddings In Qdrant ```bash
+parallel rag-cli vector-store --qdrant-url http://localhost:6333 --collection-
+name nomic-embed-text-v1.5 2>> output.log ::: $(find data/embeddings/*) ``` ###
+Run RAG Chat On A Query ```bash echo "Who invented the blue LED?" | \ rag-cli
+rag \ --ollama-embedding-url http://localhost:11434 \ --ollama-chat-url http://
+localhost:11435 \ --qdrant-url http://localhost:6333 \ --collection-name nomic-
+embed-text-v1.5 \ --top-k 5 \ --min-similarity 0.5 \ 2>> output.log ``` This
+example obviously requires that the articles similar to the query have been
+embedded and stored in Qdrant. You can do this with the example found in the
+next section. ### End-to-end Pipeline For A Single Article ```bash
+wikipedia_data=$(curl -L -s "https://en.wikipedia.org/api/rest_v1/page/summary/
+Shuji_Nakamura") && \ payload_data=$(jq "{title: .title, description:
+.description, extract: .extract}" <(echo $wikipedia_data)) && \ text_to_embed=$
+(jq -r ".title, .description, .extract" <(echo $wikipedia_data)) && \ echo
+$text_to_embed | \ rag-cli embed --ollama-url http://localhost:11434 | \ jq -
+r ".embedding" | \ rag-cli vector-store \ --qdrant-url http://localhost:6333 \
+--collection-name nomic-embed-text-v1.5 \ --data "$payload_data" ```
```

