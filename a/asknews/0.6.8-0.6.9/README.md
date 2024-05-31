# Comparing `tmp/asknews-0.6.8-py3-none-any.whl.zip` & `tmp/asknews-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 23367 bytes, number of entries: 24
+Zip file size: 23381 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4569 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
 -rw-r--r--  2.0 unx     8716 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
 -rw-r--r--  2.0 unx    13983 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
 -rw-r--r--  2.0 unx    11870 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
 -rw-r--r--  2.0 unx    16134 b- defN 80-Jan-01 00:00 asknews_sdk/client.py
 -rw-r--r--  2.0 unx      677 b- defN 80-Jan-01 00:00 asknews_sdk/dto/__init__.py
 -rw-r--r--  2.0 unx     4040 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     4530 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1306 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
 -rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
--rw-r--r--  2.0 unx     7337 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
+-rw-r--r--  2.0 unx     7354 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1451 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6339 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5396 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1595 b- defN 80-Jan-01 00:00 asknews-0.6.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.8.dist-info/RECORD
-24 files, 94791 bytes uncompressed, 20333 bytes compressed:  78.5%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1595 b- defN 80-Jan-01 00:00 asknews-0.6.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.9.dist-info/RECORD
+24 files, 94808 bytes uncompressed, 20347 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.6.8.dist-info/LICENSE
+Filename: asknews-0.6.9.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.6.8.dist-info/METADATA
+Filename: asknews-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.6.8.dist-info/WHEEL
+Filename: asknews-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.6.8.dist-info/RECORD
+Filename: asknews-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/dto/stories.py

```diff
@@ -60,15 +60,15 @@
     ]
     cluster_probabilities: Annotated[
         Optional[Dict[str, Union[int, float]]], Field({}, title="Cluster Probabilities")
     ]
 
 
 class GraphRelationships(BaseModel):
-    nodes: list[dict[Literal["id", "type"], str]]
+    nodes: list[dict[Literal["id", "type", "detailed_type"], str]]
     edges: list[dict[Literal["from", "to", "label"], str]]
 
 
 class StoryResponseUpdate(BaseModel):
     uuid: Annotated[UUID, Field(title="Uuid")]
     cluster_articles: Annotated[List[Article], Field(title="Cluster Articles")]
     prompt_articles: Annotated[List[Article], Field(title="Prompt Articles")]
```

## Comparing `asknews-0.6.8.dist-info/LICENSE` & `asknews-0.6.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.6.8.dist-info/METADATA` & `asknews-0.6.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python SDK for AskNews
 Home-page: https://github.com/emergentmethods/asknews-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `asknews-0.6.8.dist-info/RECORD` & `asknews-0.6.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 asknews_sdk/client.py,sha256=A7irft6UAXEIA8OTC2-EOfp7HSREiT09WAZ7g53iAVM,16134
 asknews_sdk/dto/__init__.py,sha256=dECq34FclMMDeF8Fq62TTngjillmysK8yht2DTOdqHM,677
 asknews_sdk/dto/base.py,sha256=XMozNP4mCiTubVWeQNGdPEzutHtc_y18lTrEfuLbkv4,4040
 asknews_sdk/dto/chat.py,sha256=U76lXLM27LXAxGeMFzbBp9rr5Wi5epXr3H6-2jyZhfc,4530
 asknews_sdk/dto/error.py,sha256=fAJutRBtFzSLcJuZYgTDZtv7-T3p6WBGqk3ky3K481c,674
 asknews_sdk/dto/news.py,sha256=dbpI_BlXISlhS5FGDGl5noNI8Uj7lsbkALBBolAV0C0,1306
 asknews_sdk/dto/sentiment.py,sha256=8UhtmYw9jxwcZ1aw9300g-UE0WEIdo5JmgWbPLR-58w,596
-asknews_sdk/dto/stories.py,sha256=rjMSy1ciJZH95lMXCBDHXNmKciDg771rtLPRwNaBGNE,7337
+asknews_sdk/dto/stories.py,sha256=5gm0lgJXdj_6TopFuZy6HhkT5SJGf4XhWzeRG2KN2f8,7354
 asknews_sdk/errors.py,sha256=2J6fihHeAL1ny7bdGAoEOazaRibosU3N4IFDBlO9vHk,1451
 asknews_sdk/sdk.py,sha256=EMQeZLuPeAWlV8yLbiefY_C7UuG-1pFDp7GwKJ0rsn4,6339
 asknews_sdk/security.py,sha256=mXVyc4_5KE2j-t5fS3IKewUfmCJZLCPbfcXMJJpLzIk,5396
 asknews_sdk/utils.py,sha256=tM7ga0MZGDA4YheH4dyZ6xxVVexMkzTMz0f6ttP6pwU,1614
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.6.8.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.6.8.dist-info/METADATA,sha256=jYEXvwgKZANpG78zSfCzH_rATJOpnWl9zyRVXuVzM2E,1595
-asknews-0.6.8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.6.8.dist-info/RECORD,,
+asknews-0.6.9.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.6.9.dist-info/METADATA,sha256=ucXVt0AH9myyxePPivy42PIE6zx6pMbu5_PbKanAxk4,1595
+asknews-0.6.9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.6.9.dist-info/RECORD,,
```

