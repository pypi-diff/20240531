# Comparing `tmp/zeval-0.1.2.tar.gz` & `tmp/zeval-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeval-0.1.2.tar", last modified: Thu May 23 08:16:10 2024, max compression
+gzip compressed data, was "zeval-0.1.4.tar", last modified: Fri May 31 03:15:57 2024, max compression
```

## Comparing `zeval-0.1.2.tar` & `zeval-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,35 @@
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.680909 zeval-0.1.2/
--rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-23 08:16:10.680729 zeval-0.1.2/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-23 08:16:10.680940 zeval-0.1.2/setup.cfg
--rw-r--r--   0 everfly    (501) wheel        (0)      887 2024-05-23 08:14:56.000000 zeval-0.1.2/setup.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.678072 zeval-0.1.2/zeval/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:04:24.000000 zeval-0.1.2/zeval/__init__.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.678839 zeval-0.1.2/zeval/config/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:33.000000 zeval-0.1.2/zeval/config/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)      180 2024-05-10 10:53:55.000000 zeval-0.1.2/zeval/config/model_config.py
--rw-r--r--   0 everfly    (501) wheel        (0)      492 2024-05-20 12:59:22.000000 zeval-0.1.2/zeval/evaluation.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.679962 zeval-0.1.2/zeval/evaluators/
--rw-r--r--   0 everfly    (501) wheel        (0)      211 2024-05-10 10:53:55.000000 zeval-0.1.2/zeval/evaluators/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)     6948 2024-05-22 12:55:23.000000 zeval-0.1.2/zeval/evaluators/answer_relevancy.py
--rw-r--r--   0 everfly    (501) wheel        (0)     4210 2024-05-23 08:14:48.000000 zeval-0.1.2/zeval/evaluators/context_precision.py
--rw-r--r--   0 everfly    (501) wheel        (0)     8173 2024-05-22 13:01:41.000000 zeval-0.1.2/zeval/evaluators/context_recall.py
--rw-r--r--   0 everfly    (501) wheel        (0)     9640 2024-05-20 12:57:21.000000 zeval-0.1.2/zeval/evaluators/faithfulness.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.680278 zeval-0.1.2/zeval/utils/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:26.000000 zeval-0.1.2/zeval/utils/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)     1245 2024-05-19 07:31:36.000000 zeval-0.1.2/zeval/utils/model.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.680535 zeval-0.1.2/zeval.egg-info/
--rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) wheel        (0)       25 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        6 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-31 03:15:57.763375 zeval-0.1.4/
+-rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-31 03:15:57.763161 zeval-0.1.4/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-31 03:15:57.763413 zeval-0.1.4/setup.cfg
+-rw-r--r--   0 everfly    (501) wheel        (0)      887 2024-05-31 03:13:14.000000 zeval-0.1.4/setup.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-31 03:15:57.760487 zeval-0.1.4/tests/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-25 15:11:07.000000 zeval-0.1.4/tests/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)      890 2024-05-30 03:49:29.000000 zeval-0.1.4/tests/test_is_json.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     1393 2024-05-30 03:56:27.000000 zeval-0.1.4/tests/test_json_match.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     1780 2024-05-30 09:11:32.000000 zeval-0.1.4/tests/test_json_schema_match.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     1665 2024-05-30 10:02:50.000000 zeval-0.1.4/tests/test_match.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     2076 2024-05-30 02:43:36.000000 zeval-0.1.4/tests/test_rag.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-31 03:15:57.760670 zeval-0.1.4/zeval/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:04:24.000000 zeval-0.1.4/zeval/__init__.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-31 03:15:57.761427 zeval-0.1.4/zeval/config/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:33.000000 zeval-0.1.4/zeval/config/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)      180 2024-05-10 10:53:55.000000 zeval-0.1.4/zeval/config/model_config.py
+-rw-r--r--   0 everfly    (501) wheel        (0)      590 2024-05-30 02:01:25.000000 zeval-0.1.4/zeval/evaluation.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-31 03:15:57.762392 zeval-0.1.4/zeval/evaluators/
+-rw-r--r--   0 everfly    (501) wheel        (0)      297 2024-05-30 03:59:45.000000 zeval-0.1.4/zeval/evaluators/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     7131 2024-05-30 01:59:54.000000 zeval-0.1.4/zeval/evaluators/answer_relevancy.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     4204 2024-05-30 07:30:22.000000 zeval-0.1.4/zeval/evaluators/context_precision.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     8145 2024-05-30 01:59:45.000000 zeval-0.1.4/zeval/evaluators/context_recall.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     9742 2024-05-30 07:30:29.000000 zeval-0.1.4/zeval/evaluators/faithfulness.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     3965 2024-05-30 09:13:09.000000 zeval-0.1.4/zeval/evaluators/json.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     3862 2024-05-30 03:05:15.000000 zeval-0.1.4/zeval/evaluators/matchness.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-31 03:15:57.762692 zeval-0.1.4/zeval/utils/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:26.000000 zeval-0.1.4/zeval/utils/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     2700 2024-05-30 03:41:17.000000 zeval-0.1.4/zeval/utils/helpers.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     1263 2024-05-25 12:13:24.000000 zeval-0.1.4/zeval/utils/model.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-31 03:15:57.762864 zeval-0.1.4/zeval.egg-info/
+-rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-31 03:15:57.000000 zeval-0.1.4/zeval.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)      674 2024-05-31 03:15:57.000000 zeval-0.1.4/zeval.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-31 03:15:57.000000 zeval-0.1.4/zeval.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)       25 2024-05-31 03:15:57.000000 zeval-0.1.4/zeval.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)       12 2024-05-31 03:15:57.000000 zeval-0.1.4/zeval.egg-info/top_level.txt
```

### Comparing `zeval-0.1.2/PKG-INFO` & `zeval-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeval
-Version: 0.1.2
+Version: 0.1.4
 Summary: A Python library for evaluating RAG outputs of Chinese large language models.
 Home-page: https://github.com/yourgithub/zeval
 Author: everfly
 Author-email: tagriver@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zeval-0.1.2/setup.py` & `zeval-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zeval',
-    version='0.1.2',
+    version='0.1.4',
     author='everfly',
     author_email='tagriver@gmail.com',
     description='A Python library for evaluating RAG outputs of Chinese large language models.',
     # long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourgithub/zeval',
     packages=find_packages(),
```

### Comparing `zeval-0.1.2/zeval/evaluators/answer_relevancy.py` & `zeval-0.1.4/zeval/evaluators/answer_relevancy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from zeval.utils.model import ModelCaller
 from typing import Any, Callable, Dict
 from datasets import Dataset
 import logging
-import time, json, os 
-import numpy as np
 import re, json, logging
-from openai import OpenAI
 logging.basicConfig(level=logging.INFO)
 
 class AnswerRelevancy:
     name = 'answer_relevancy'
 
     PROMPTS = {
         'en': {
             'QUESTION_TEMPLATE': """
-Generate a question for the given answer.
-Answer:
-The PSLV-C56 mission is scheduled to launch on Sunday, July 30, 2023, at 6:30 AM IST / 1:00 AM UTC. It will be launched from the Satish Dhawan Space Centre in Sriharikota, Andhra Pradesh, India.
-Question:
-What is the scheduled launch date and time for the PSLV-C56 mission? Where will it be launched from?
+Generate question for the given answer.
+Answer:\nThe PSLV-C56 mission is scheduled to be launched on Sunday, 30 July 2023 at 06:30 IST / 01:00 UTC. It will be launched from the Satish Dhawan Space Centre, Sriharikota, Andhra Pradesh, India 
+Question: When is the scheduled launch date and time for the PSLV-C56 mission, and where will it be launched from?
 
-Answer: {answer}
+Answer:{answer}
 Question:
 """,
             'CORRELATION_PROMPT_TEMPLATE': """
 Task: Estimate the correlation between the two given strings. In your evaluation, consider not only direct connections but also indirect and subtle associations.
 For example, if 'bridge' appears in the first string and 'water' in the second, consider the compound term 'water bridge.' Similarly, for 'book' and 'wisdom,' consider phrases like 'books are keys to wisdom.'
 You should use the following scoring scale from 0.00 to 1.00 to assess correlation, where:
 0.00 means no correlation at all.
@@ -47,15 +42,15 @@
 
 The question I generated is:
 {gen_question}
 
 The original question provided by the user is:
 {question}
 
-By calculating the cosine similarity, the derived answer relevance score is: {result}
+By analyzing the meaning of the two questions, the derived answer relevance score is: {result}
 """
         },
         'zh': {
             'QUESTION_TEMPLATE': """
 为给定的答案生成问题。
 答案：
 PSLV-C56任务预定于2023年7月30日星期日IST上午6:30 / UTC凌晨1:00发射。它将从位于印度安得拉邦斯里赫里戈塔的萨蒂什·达瓦恩航天中心发射。
@@ -89,34 +84,39 @@
 
 我由此生成的问题是：
 {gen_question}
 
 用户原来的问题是：
 {question}
 
-通过计算余弦相似度，由此得出的回答相似度得分是：{result}
+通过分析两个问题的语义，我给出的回答相似度得分是：{result}
 """
         }
     }
+    
+    PRE_ANSWER = {
+        'en': 'Final answer:',
+        'zh': '最终答案：'
+    }
 
     def __init__(self, lang='zh'):
         self.language = lang
 
     def get_prompt(self, key):
         return self.PROMPTS[self.language][key]
 
-    def score(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
+    def eval(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
         if dataset is None:
             params = {}
         if sample_kwargs is None:
             sample_kwargs = {}
 
         question = dataset["question"]
         answer = dataset["answer"]
-        context = dataset["context"]
+        context = '\n'.join(dataset["context"])
 
         question_prompt = self.get_prompt('QUESTION_TEMPLATE').format(answer=answer)
         if isinstance(question_prompt, str):
             messages = [{"role": "user", "content": question_prompt}]
 
         gen_question_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
         gen_question = ModelCaller.parse_response(self, gen_question_response)
@@ -135,28 +135,31 @@
         correlation_response.completion = correlation_result
 
         result_score = self.extract_score(correlation_result)
 
         reasoning = self.get_prompt('REASONING_MESSAGE').format(answer=answer, gen_question=gen_question, question=question, result=result_score)
 
         responses = [gen_question_response, correlation_response]
-        return result_score, reasoning, responses
+        eval_result = {"score": result_score, "reasoning": reasoning, "responses": responses}
+
+        return eval_result
 
-    @staticmethod
-    def extract_score(response_content: str) -> float:
+    def extract_score(self, response_content: str) -> float:
         """
         Extracts the similarity score from the content of a GPT model's response.
 
         Args:
             response_content: The content of a GPT model's response.
 
         Returns:
             The similarity score as a float. If no score could be extracted, returns 0.0.
         """
         try:
-            match = re.search(r"最终答案[:：]\s*\[(.+?)]", response_content).group(1)
+            pre_answer = self.PRE_ANSWER[self.language]  
+            match = re.search(f"{pre_answer}\s*\[(.+?)]", response_content).group(1)
             score = float(match)
             logging.debug(f"response_content: {response_content}, score: {score}")
-        except AttributeError:
+        except AttributeError as e:
+            print(e)
             score = 0.0
             logging.warning("Answer not found in response, score set to 0, will autofail validation scoring.")
-        return score
+        return score
```

### Comparing `zeval-0.1.2/zeval/evaluators/context_precision.py` & `zeval-0.1.4/zeval/evaluators/context_precision.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 from zeval.utils.model import ModelCaller
 from typing import Any, Callable, Dict
 from datasets import Dataset
 import logging
-import time, json
+import json
 logging.basicConfig(level=logging.INFO)
 
 class ContextPrecision:
     name = 'context_precision'
 
     PROMPTS = {
         'en': {
             'CONTEXT_PRECISION_TEMPLATE': """\
-Given a question and a context, verify whether the information in the given context helps answer the question. Return a "Yes" or "No" answer.
-Question:
-{question}
-Context:
+Given a question and a context, verify if the information in the given context is useful in answering the question. Return a Yes/No answer.
+question: {question}
+context:
 {context}
-Answer:
+answer:
 """,
             'REASONING_MESSAGE': """
 My reasoning process is as follows:
 I will go through each context, verify whether the information in the given context helps answer the question, and return a "Yes" or "No" answer, which I will convert to True or False accordingly.
 
 Here are my judgments for each context:
 {judges}
 
 Then, by calculating the cumulative precision of all the correct responses (True) up to that point, the average precision score is: {result}
 """
         },
         'zh': {
             'CONTEXT_PRECISION_TEMPLATE': """\
 给定一个问题和一个上下文，验证给定的上下文中的信息是否有助于回答这个问题。返回一个“Yes”或“No”的答案。
-问题：
-{question}
+问题：{question}
 上下文：
 {context}
 答案：
 """,
             'REASONING_MESSAGE': """
 我的推理过程如下：
 我会遍历每个上下文信息，验证给定的上下文中的信息是否有助于回答这个问题。返回一个“Yes”或“No”的答案，并将其转化为True或False的相应。
@@ -51,49 +49,48 @@
 
     def __init__(self, lang='zh'):
         self.language = lang
 
     def get_prompt(self, key):
         return self.PROMPTS[self.language][key]
 
-    def score(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
+    def eval(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
         if dataset is None:
             params = {}
         if sample_kwargs is None:
             sample_kwargs = {}
 
         question = dataset["question"]
-        context = dataset["context"][0]
-
+        context = dataset["context"]
+        
         """
-        根据问题和上下文计算上下文精确度。
+        Compute context precision based on the question and context.
         """
         determine_results, determine_responses = self.determine_usefulness(question, context, sample_kwargs)
 
         result_score = self.calculate_average_precision(determine_results)
 
         string_results = [str(result) for result in determine_results]
         judges = ",".join(string_results)
 
         reasoning = self.get_prompt('REASONING_MESSAGE').format(judges=judges, result=result_score)
-        print("reasoning: ", reasoning)
-        return result_score, reasoning, determine_responses
+        eval_result = {"score": result_score, "reasoning": reasoning, "responses": determine_responses}
+        return eval_result
 
     def determine_usefulness(self, question: str, contexts: list[str], sample_kwargs: dict = None) -> list[bool]:
         determine_responses = []
         determine_results = []
         for context in contexts:
-            start_time = time.time()  # 开始计时
             determine_prompt = self.get_prompt('CONTEXT_PRECISION_TEMPLATE').format(question=question, context=context)
             if isinstance(determine_prompt, str):
                 messages = [{"role": "user", "content": determine_prompt}]
 
             determine_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
             determine_result = ModelCaller.parse_response(self, determine_response)
-
+            
             determine_response.elapsed_time = elapsed_time
             determine_response.prompt = json.dumps(determine_prompt)
             determine_response.completion = determine_result
 
             determine_results.append("Yes" in determine_result)
             determine_responses.append(determine_response)
```

### Comparing `zeval-0.1.2/zeval/evaluators/context_recall.py` & `zeval-0.1.4/zeval/evaluators/context_recall.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from zeval.utils.model import ModelCaller
 from typing import Any, Callable, Dict
 from datasets import Dataset
 import logging
-import time, json
+import json
 logging.basicConfig(level=logging.INFO)
 
 class ContextRecall:
     name = 'context_recall'
 
     PROMPTS = {
         'en': {
             'CONTEXT_RECALL_RA': """
-Given a context and an answer, analyze each sentence of the answer to determine if the sentence can be attributed to the given context. Think through the steps and reason before concluding.
+Given a context, and an answer, analyze each sentence in the answer and classify if the sentence can be attributed to the given context or not.
+Think in steps and reason before coming to conclusion.
 
-Context: Einstein (March 14, 1879 – April 18, 1955) was a theoretical physicist born in Germany who is widely regarded as one of the greatest and most influential scientists of all time. His most famous achievement is developing the theory of relativity, and he also made significant contributions to quantum mechanics. As a result, he was a central figure in the revolution of modern physics in the early 20th century that reshaped our understanding of the natural sciences. His equation E=mc², which arises from relativity, is known as "the world's most famous equation." He received the Nobel Prize in Physics in 1921 for his contributions to theoretical physics, particularly the discovery of the law of the photoelectric effect, a crucial step in the development of quantum theory. His work is also known for its influence on the philosophy of science. In a survey of top physicists conducted by Physics World magazine in 1999, Einstein was voted the greatest physicist of all time. His intellectual achievements and originality have made the word "Einstein" synonymous with "genius."
-Answer: Einstein was born on March 14, 1879, and was a German-born theoretical physicist who is widely regarded as one of the greatest and most influential scientists of all time. He received the Nobel Prize in Physics in 1921 for his contributions to theoretical physics. He published four papers in 1905. Einstein moved to Switzerland in 1895.
-Classification:
-1. Einstein was born on March 14, 1879, and was a German-born theoretical physicist who is widely regarded as one of the greatest and most influential scientists of all time. Einstein's birth date is explicitly mentioned in the context. Therefore, [Attribution]
-2. He received the Nobel Prize in Physics in 1921 for his contributions to theoretical physics. This exact sentence is in the given context. Therefore, [Attribution]
-3. He published four papers in 1905. This is not mentioned in the given context. Therefore, [No Attribution]
-4. Einstein moved to Switzerland in 1895. There is no evidence to support this in the given context. Therefore, [No Attribution]
-
-Context: {context}
-Answer: {ideal}
-Classification:
+context: Albert Einstein (14 March 1879 – 18 April 1955) was a German-born theoretical physicist,widely held to be one of the greatest and most influential scientists of all time. Best known for developing the theory of relativity, he also made important contributions to quantum mechanics, and was thus a central figure in the revolutionary reshaping of the scientific understanding of nature that modern physics accomplished in the first decades of the twentieth century. His mass–energy equivalence formula E = mc2, which arises from relativity theory, has been called "the world's most famous equation". He received the 1921 Nobel Prize in Physics "for his services to theoretical physics, and especially for his discovery of the law of the photoelectric effect", a pivotal step in the development of quantum theory. His work is also known for its influence on the philosophy of science. In a 1999 poll of 130 leading physicists worldwide by the British journal Physics World, Einstein was ranked the greatest physicist of all time. His intellectual achievements and originality have made Einstein synonymous with genius.
+answer: Albert Einstein born in 14 March 1879 was  German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time. He received the 1921 Nobel Prize in Physics "for his services to theoretical physics. He published 4 papers in 1905.  Einstein moved to Switzerland in 1895 
+classification
+1. Albert Einstein born in 14 March 1879 was  German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time. The date of birth of Einstein is mentioned clearly in the context. So [Attributed]
+2. He received the 1921 Nobel Prize in Physics "for his services to theoretical physics. The exact sentence is present in the given context. So [Attributed]
+3. He published 4 papers in 1905. There is no mention about papers he wrote in given the context. So [Not Attributed]
+4. Einstein moved to Switzerland in 1895. There is not supporting evidence for this in the given the context. So [Not Attributed]
+
+context:{context}
+answer:{ideal}
+classification:
 """,
             'REASONING_MESSAGE': """
 My reasoning process is as follows:
 First, I analyze each sentence of the ideal answer to determine if it can be attributed to the given context.
 
 Ideal answer: {ideal}
 Context: {context}
@@ -47,84 +48,88 @@
 答案：爱因斯坦出生于1879年3月14日，是一位德国出生的理论物理学家，被广泛认为是有史以来最伟大和最具影响力的科学家之一。他因“对理论物理的贡献”获得了1921年诺贝尔物理学奖。他在1905年发表了4篇论文。爱因斯坦于1895年搬到了瑞士。
 分类：
 1. 爱因斯坦出生于1879年3月14日，是一位德国出生的理论物理学家，被广泛认为是有史以来最伟大和最具影响力的科学家之一。爱因斯坦的出生日期在上下文中有明确提及。因此[归因]
 2. 他因“对理论物理的贡献”获得了1921年诺贝尔物理学奖。给定上下文中有这个确切的句子。因此[归因]
 3. 他在1905年发表了4篇论文。在给定的上下文中没有提到他写的论文。因此[未归因]
 4. 爱因斯坦于1895年搬到了瑞士。在给定的上下文中没有支持这一点的证据。因此[未归因]
 
-上下文：{context}
+上下文：
+{context}
 答案：{ideal}
 分类：
 """,
             'REASONING_MESSAGE': """
 我的推理过程如下：
 首先，我分析理想答案(ideal)中的每个句子，判断该句子是否能归因于给定的上下文(Context)。
 
 理想答案：{ideal}
-上下文：{context}
+上下文：
+{context}
 
 以下是我的分类：
 {statements}
 
 然后，我根据归因的句子数量计算得分，得出的得分是：{final_score}
 """
         }
     }
+    
+    ATTRIBUTE_WORDS = {
+        'en': {
+            'yes': '[Attributed]',
+            'no': '[No Attributed]'
+        },
+        'zh': {
+            'yes': '[归因]',
+            'no': '[未归因]'
+        }
+    }
 
     def __init__(self, lang='zh'):
         self.language = lang
 
     def get_prompt(self, key):
         return self.PROMPTS[self.language][key]
 
-    def score(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
+    def eval(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
         if dataset is None:
             params = {}
         if sample_kwargs is None:
             sample_kwargs = {}
 
-        question = dataset["question"]
-        context = dataset["context"][0]
-        ideal = dataset["ideal"][0]
-        print("ideal:", ideal)
+        context = dataset["context"]
+        ideal = dataset["ideal"]
 
         gt = "\n".join(ideal) if isinstance(ideal, list) else ideal
         ctx = "\n".join(context) if isinstance(context, list) else context
+        
         classification, attribute_response = self.classify_context_recall(ctx, gt, sample_kwargs)
-        print("classification:", classification)
-        print("response:", attribute_response)
-
         result_score = self.calculate_score(classification)
 
         responses = [attribute_response]
         reasoning = self.get_prompt('REASONING_MESSAGE').format(ideal=gt, context=ctx, statements="\n".join(classification), final_score=result_score)
+        eval_result = {"score": result_score, "reasoning": reasoning, "responses": responses}
 
-        return result_score, reasoning, responses
+        return eval_result
 
     def classify_context_recall(self, context: str, ideal: str, sample_kwargs: dict = None) -> list[str]:
-        # 使用 CONTEXT_RECALL_RA 模板
         prompt = self.get_prompt('CONTEXT_RECALL_RA').format(context=context, ideal=ideal)
-
-        # 创建 PromptFn 实例
         if isinstance(prompt, str):
             messages = [{"role": "user", "content": prompt}]
-
         attribute_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
         attribute_answer = ModelCaller.parse_response(self, attribute_response)
-
         attribute_response.elapsed_time = elapsed_time
         attribute_response.prompt = json.dumps(prompt)
         attribute_response.completion = attribute_answer
 
         classification = []
+        attributed = self.ATTRIBUTE_WORDS[self.language]['yes']
         for line in attribute_answer.split('\n'):
-            if '[归因]' in line or '[未归因]' in line or '[Attribution]' in line or '[No Attribution]' in line:
+            if attributed in line or attributed in line:
                 classification.append(line.strip())
 
         return classification, attribute_response
 
     def calculate_score(self, classification: list[str]) -> float:
-        verdict_token_zh = "[归因]"
-        verdict_token_en = "[Attribution]"
-        numerator = sum(verdict_token_zh in sentence or verdict_token_en in sentence for sentence in classification)
+        numerator = sum(self.ATTRIBUTE_WORDS[self.language]['yes'] in sentence for sentence in classification)
         denominator = len(classification)
         return numerator / denominator if denominator > 0 else 0
```

### Comparing `zeval-0.1.2/zeval/evaluators/faithfulness.py` & `zeval-0.1.4/zeval/evaluators/faithfulness.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 from zeval.utils.model import ModelCaller
 from typing import Any, Callable, Dict
 from datasets import Dataset
 import logging
-import time, json
+import json
 logging.basicConfig(level=logging.INFO)
 
 class Faithfulness:
     name = 'faithfulness'
 
     PROMPTS = {
         'en': {
             'LONG_FORM_ANSWER_PROMPT': """\
-Given a question and an answer, create one or more statements from each sentence of the given answer.
-Question: Who is Albert Einstein and what is he most famous for?
-Answer: He was a theoretical physicist born in Germany who is widely regarded as one of the greatest and most influential physicists of all time. He is best known for developing the theory of relativity, and he also made significant contributions to the development of the theory of quantum mechanics.
-Statements:
+Given a question and answer, create one or more statements from each sentence in the given answer.
+question: Who was Albert Einstein and what is he best known for?
+answer: He was a German-born theoretical physicist, widely acknowledged to be one of the greatest and most influential physicists of all time. He was best known for developing the theory of relativity, he also made important contributions to the development of the theory of quantum mechanics.
+statements:
 Albert Einstein was born in Germany.
-Albert Einstein is known for his theory of relativity.
-Question: Cadmium chloride is slightly soluble in which chemical substance?
-Answer: Alcohol.
-Statements:
-Cadmium chloride is slightly soluble in alcohol.
-Question: Are Shahul and Jithin of the same nationality?
-Answer: They are from different countries.
-Statements:
-Shahul and Jithin are from different countries.
-Question: {question}
-Answer: {answer}
-Statements:
+Albert Einstein was best known for his theory of relativity.
+question: Cadmium Chloride is slightly soluble in this chemical, it is also called what?
+answer: alcohol
+statements:
+Cadmium Chloride is slightly soluble in alcohol.
+question: Were Shahul and Jithin of the same nationality?
+answer: They were from different countries.
+statements:
+Shahul and Jithin were from different countries.
+question:{question}
+answer: {answer}
+statements:
 """,
             'NLI_STATEMENTS_MESSAGE': """
-Prompt: Natural Language Inference
-Consider the given context and the following statements, then determine whether these statements are supported by the information in the context. Provide a brief explanation for each statement before concluding (yes/no). Provide the final judgment for each statement in the specified format at the end. Do not deviate from the specified format.
+Prompt: Natural language inference
+Consider the given context and following statements, then determine whether they are supported by the information present in the context.Provide a brief explanation for each statement before arriving at the verdict (Yes/No). Provide a final verdict for each statement in order at the end in the given format. Do not deviate from the specified format.
 
 Context:
-John is a student at XYZ University. He is pursuing a degree in Computer Science. He has enrolled in several courses this semester, including Data Structures, Algorithms, and Database Management. John is a diligent student who spends a lot of time studying and completing assignments. He often stays late at the library working on his projects.
-Statements:
-1. John majors in Biology.
+John is a student at XYZ University. He is pursuing a degree in Computer Science. He is enrolled in several courses this semester, including Data Structures, Algorithms, and Database Management. John is a diligent student and spends a significant amount of time studying and completing assignments. He often stays late in the library to work on his projects.
+statements:
+1. John is majoring in Biology.
 2. John is taking a course on Artificial Intelligence.
 3. John is a dedicated student.
 4. John has a part-time job.
 5. John is interested in computer programming.
 
 Answer:
-1. John majors in Biology.
-Explanation: It is clearly mentioned that John is majoring in Computer Science. There is no information indicating he is majoring in Biology. Verdict: No.
+1. John is majoring in Biology.
+Explanation: John's major is explicitly mentioned as Computer Science. There is no information suggesting he is majoring in Biology.  Verdict: No.
 2. John is taking a course on Artificial Intelligence.
-Explanation: The context mentions the courses John is currently enrolled in, but does not mention Artificial Intelligence. Hence, we cannot infer that John is taking a course on Artificial Intelligence. Verdict: No.
+Explanation: The context mentions the courses John is currently enrolled in, and Artificial Intelligence is not mentioned. Therefore, it cannot be deduced that John is taking a course on AI. Verdict: No.
 3. John is a dedicated student.
-Explanation: The context states that he spends a lot of time studying and completing assignments. Additionally, it mentions that he often stays late at the library working on his projects, implying his dedication. Verdict: Yes.
+Explanation: The prompt states that he spends a significant amount of time studying and completing assignments. Additionally, it mentions that he often stays late in the library to work on his projects, which implies dedication. Verdict: Yes.
 4. John has a part-time job.
-Explanation: The context does not provide information about John having a part-time job. Hence, we cannot infer that John has a part-time job. Verdict: No.
+Explanation: There is no information given in the context about John having a part-time job. Therefore, it cannot be deduced that John has a part-time job.  Verdict: No.
 5. John is interested in computer programming.
-Explanation: The context mentions that John is pursuing a degree in Computer Science, which implies his interest in computer programming. Verdict: Yes.
-Final judgment for each statement: No. No. Yes. No. Yes.
-Context:
+Explanation: The context states that John is pursuing a degree in Computer Science, which implies an interest in computer programming. Verdict: Yes.
+Final verdict for each statement in order: No. No. Yes. No. Yes.
+context:
 {context}
-Statements:
+statements:
 {statements}
 Answer:
 """,
             'REASONING_MESSAGE': """
 My reasoning process is as follows:
 First, I created the following statements from each sentence of the given answer:
 {statements}
@@ -83,15 +83,15 @@
 问题：Shahul和Jithin是同一国籍吗？
 答案：他们来自不同的国家。
 陈述：
 Shahul和Jithin来自不同的国家。
 问题：{question}
 答案：{answer}
 陈述：
-""",  # noqa: E501
+""",
             'NLI_STATEMENTS_MESSAGE': """
 提示：自然语言推理
 考虑给定的背景和以下陈述，然后确定这些陈述是否得到了上下文中的信息支持。在得出结论（是/否）之前，为每个陈述提供简要说明。在最后以指定格式为每个陈述提供最终裁决。不要偏离指定格式。
 
 上下文：
 约翰是XYZ大学的学生。他正在攻读计算机科学学位。他这学期注册了几门课程，包括数据结构、算法和数据库管理。约翰是一个勤奋的学生，花大量时间学习和完成作业。他经常待在图书馆里晚上工作在他的项目上。
 陈述：
@@ -99,24 +99,24 @@
 2.约翰正在上一门关于人工智能的课程。
 3.约翰是一个专注的学生。
 4.约翰有一份兼职工作。
 5.约翰对计算机编程感兴趣。
 
 答案：
 1.约翰主修生物学。
-解释：明确提到约翰的专业是计算机科学。没有信息表明他主修生物学。 裁决：否。
+解释：明确提到约翰的专业是计算机科学。没有信息表明他主修生物学。 裁决：No.
 2.约翰正在上一门关于人工智能的课程。
-解释：上下文提到约翰当前注册的课程，而没有提到人工智能。因此，不能推断约翰正在上人工智能课程。裁决：否。
+解释：上下文提到约翰当前注册的课程，而没有提到人工智能。因此，不能推断约翰正在上人工智能课程。裁决：No.
 3.约翰是一个专注的学生。
-解释：提示中提到他花大量时间学习和完成作业。此外，还提到他经常待在图书馆里晚上工作在他的项目上，这暗示了他的专注。裁决：是。
+解释：提示中提到他花大量时间学习和完成作业。此外，还提到他经常待在图书馆里晚上工作在他的项目上，这暗示了他的专注。裁决：Yes.
 4.约翰有一份兼职工作。
-解释：上下文中没有提供约翰有兼职工作的信息。因此，不能推断约翰有兼职工作。裁决：否。
+解释：上下文中没有提供约翰有兼职工作的信息。因此，不能推断约翰有兼职工作。裁决：No.
 5.约翰对计算机编程感兴趣。
-解释：上下文提到约翰正在攻读计算机科学学位，这暗示了他对计算机编程的兴趣。裁决：是。
-每个陈述的最终裁决顺序：否。否。是。否。是。
+解释：上下文提到约翰正在攻读计算机科学学位，这暗示了他对计算机编程的兴趣。裁决：No.
+每个陈述的最终裁决顺序：No. No. Yes. No. No.
 上下文：
 {context}
 陈述：
 {statements}
 答案：
 """,
             'REASONING_MESSAGE': """
@@ -124,81 +124,80 @@
 首先，我从给定答案的每个句子中创建以下的陈述：
 {statements}
 然后，我考虑了上下文信息，并对每个陈述进行了自然语言推理。最后，我得出了每个陈述的最终裁决。
 {final_statement}
 """
         }
     }
+    
+    PRE_ANSWER = {
+        'en': 'Final verdict for each statement in order:',
+        'zh': '每个陈述的最终裁决顺序：'
+    }
 
     def __init__(self, lang='zh'):
         self.language = lang
         
     def get_prompt(self, key):
         return self.PROMPTS[self.language][key]
 
-    def score(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
+    def eval(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
         if dataset is None:
             params = {}
         if sample_kwargs is None:
             sample_kwargs = {}
 
         question = dataset["question"]
         answer = dataset["answer"]
-        context = dataset["context"][0]
+        context = "\n".join(dataset["context"])
 
         human_prompt = self.get_prompt('LONG_FORM_ANSWER_PROMPT').format(question=question, answer=answer)
-
+        
         messages = [
             {"content": human_prompt, "role": "user"},
         ]
-
         statements_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
+        
         statements = ModelCaller.parse_response(self, statements_response)
 
         statements_response.elapsed_time = elapsed_time
         statements_response.prompt = json.dumps(human_prompt)
         statements_response.completion = statements
 
         nli_prompt = self.get_prompt('NLI_STATEMENTS_MESSAGE').format(context=context, statements=statements)
-
+        
         messages = [
             {"content": nli_prompt, "role": "user"},
         ]
-
-        logging.info("messages: %s", messages)
-
         nli_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
+                
         final_statement = ModelCaller.parse_response(self, nli_response)
         nli_response.elapsed_time = elapsed_time
         nli_response.prompt = json.dumps(nli_prompt)
         nli_response.completion = final_statement
-
-        result = self.analyze_nli_response(final_statement)
+        
+        result_score = self.analyze_nli_response(nli_response.completion)
 
         responses = [statements_response, nli_response]
         reasoning = self.get_prompt('REASONING_MESSAGE').format(statements=statements, final_statement=final_statement)
+        
+        eval_result = {"score": result_score, "reasoning": reasoning, "responses": responses}
 
-        return result, reasoning, responses
+        return eval_result
 
     def analyze_nli_response(self, final_statement):
-        # 从模型响应中获得最终陈述
         if not final_statement:
             return 0.0
-        # 计算得分
-        pre_answer = "每个陈述的最终裁决顺序："
+        pre_answer = self.PRE_ANSWER[self.language]
         if pre_answer in final_statement:
             final_statement = final_statement[final_statement.find(pre_answer) + len(pre_answer):]
-            final_statement = final_statement.strip().split("。")
+            final_statement = final_statement.strip().split(".")
             final_statement = list(filter(None, final_statement))
 
-            print(final_statement)
             score = sum(
-                0 if "是" in answer else 1
+                0 if "Yes" in answer else 1
                 for answer in final_statement
             )
             score = score / len(final_statement)
-
-            print("raw score: ", score)
         else:
             score = 0.0
-
         return 1 - score
```

### Comparing `zeval-0.1.2/zeval/utils/model.py` & `zeval-0.1.4/zeval/utils/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # zeval/zeval/utils/model_caller.py
 import litellm
 from litellm import completion
-from unionllm import UnionLLM
+from unionllm import UnionLLM, unionchat
 import time
 
 class ModelCaller:
     def __init__(self, config):
         self.config = config
 
     def call(self, **params):
-        # 更新或合并额外参数，避免重复
+        # merge the parameters
         effective_params = {**params}
-        start_time = time.time() # 开始计时
+        start_time = time.time()
 
         try:
-            self.client = UnionLLM(**params)
-            response = self.client.completion(**effective_params)
+            # self.client = UnionLLM(**params)
+            # response = self.client.completion(**effective_params)
+            response = unionchat(**effective_params)
         except:
             try:
-                # 去掉不需要的参数provider
+                # remove the provider key from the parameters for litellm
                 effective_params.pop('provider', None)
-                response = litellm.completion(**effective_params)
+                response = completion(**effective_params)
             except Exception as e:
                 return False, str(e)
           
-        end_time = time.time() # 结束计时
-        elapsed_time = end_time - start_time # 计算经过的时间
+        end_time = time.time()
+        elapsed_time = end_time - start_time
         return response, elapsed_time
             
     def parse_response(self, response):
         try:
-            # 从模型响应中获得最终陈述
+            # get the final statement from the model response
             choices = response.choices
             final_statement = choices[0].message.content 
             return final_statement
         except Exception as e:
             return False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zeval-0.1.2/zeval.egg-info/PKG-INFO` & `zeval-0.1.4/zeval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeval
-Version: 0.1.2
+Version: 0.1.4
 Summary: A Python library for evaluating RAG outputs of Chinese large language models.
 Home-page: https://github.com/yourgithub/zeval
 Author: everfly
 Author-email: tagriver@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

