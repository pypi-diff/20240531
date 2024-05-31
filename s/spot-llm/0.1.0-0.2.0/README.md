# Comparing `tmp/spot_llm-0.1.0.tar.gz` & `tmp/spot_llm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spot_llm-0.1.0.tar", max compression
+gzip compressed data, was "spot_llm-0.2.0.tar", max compression
```

## Comparing `spot_llm-0.1.0.tar` & `spot_llm-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2107 2024-05-31 01:25:29.411661 spot_llm-0.1.0/README.md
--rw-r--r--   0        0        0      468 2024-05-31 01:25:29.412661 spot_llm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      150 2024-05-31 01:25:29.412661 spot_llm-0.1.0/spot_llm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 01:25:29.442661 spot_llm-0.1.0/spot_llm/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 01:25:29.442661 spot_llm-0.1.0/spot_llm/models/gemma7b.py
--rw-r--r--   0        0        0      886 2024-05-31 01:25:29.412661 spot_llm-0.1.0/spot_llm/models/hf_model.py
--rw-r--r--   0        0        0      223 2024-05-31 01:25:29.413661 spot_llm-0.1.0/spot_llm/models/mistral7b.py
--rw-r--r--   0        0        0      238 2024-05-31 01:25:29.413661 spot_llm-0.1.0/spot_llm/models/opt125.py
--rw-r--r--   0        0        0     1544 2024-05-31 01:25:29.413661 spot_llm-0.1.0/spot_llm/models/spotter.py
--rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 spot_llm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2107 2024-05-31 18:45:19.328686 spot_llm-0.2.0/README.md
+-rw-r--r--   0        0        0      540 2024-05-31 18:45:19.329686 spot_llm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-05-31 18:45:19.329686 spot_llm-0.2.0/spot_llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:45:19.363686 spot_llm-0.2.0/spot_llm/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:45:19.363686 spot_llm-0.2.0/spot_llm/models/gemma7b.py
+-rw-r--r--   0        0        0      978 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/hf_model.py
+-rw-r--r--   0        0        0      223 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/mistral7b.py
+-rw-r--r--   0        0        0      239 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/opt125.py
+-rw-r--r--   0        0        0     1657 2024-05-31 18:45:19.330686 spot_llm-0.2.0/spot_llm/models/spotter.py
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 spot_llm-0.2.0/PKG-INFO
```

### Comparing `spot_llm-0.1.0/README.md` & `spot_llm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spot_llm-0.1.0/spot_llm/models/hf_model.py` & `spot_llm-0.2.0/spot_llm/models/hf_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Optional
 
+import torch
 from torch import Tensor
-from spot_llm.models.spotter import Spotter
 from transformers import AutoTokenizer, AutoModelForCausalLM  # type: ignore
 
+from spot_llm.models.spotter import Spotter
+
 
 class HFSpotter(Spotter):
-    def __init__(
-        self, model_id: str, token: Optional[str] = None, version: str = "0.3"
-    ):
-        self.token = token
-        self.model_id = model_id
+    def __init__(self, model_id: str, token: Optional[str] = None):
+        super().__init__(model_id=model_id, token=token)
 
     def initialize(self) -> None:
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_id, token=self.token)
         self.model = AutoModelForCausalLM.from_pretrained(
-            self.model_id, token=self.token
+            self.model_id, token=self.token, device_map="auto"
         )
 
+    def tokenize(self, text: str) -> Tensor:
+        tokenz = self.tokenizer(
+            text, add_special_tokens=False, return_tensors="pt"
+        ).input_ids
+        return tokenz
+
     def _get_lazy_logits(
         self,
         inputs: Tensor,
     ) -> Tensor:
-
-        return self.model.generate(
-            input_ids=inputs,
-            do_sample=False,
-            temperature=0.0,
-            num_return_sequences=1,
-            max_new_tokens=1,
-        )
+        with torch.no_grad():
+            output = self.model(inputs.to(self.model.device))
+        return output
```

### Comparing `spot_llm-0.1.0/spot_llm/models/spotter.py` & `spot_llm-0.2.0/spot_llm/models/spotter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import numpy as np
-from torch import Tensor
-
-
 from abc import abstractmethod
 from typing import Any, List, Optional, Tuple
 
+import numpy as np
+from torch import Tensor
+
 
 class Spotter:
     def __init__(
         self,
         model_id: str,
         token: Optional[str] = None,
         base_token_count: int = 24,
@@ -24,33 +23,37 @@
     def initialize(self) -> None:
         raise NotImplementedError()
 
     def predict_logits_and_tokenz(self, input_prompt: str) -> Tuple[Tensor, Tensor]:
         tokenz = self.tokenize(input_prompt)
         return self._get_lazy_logits(tokenz), tokenz
 
+    @abstractmethod
     def tokenize(self, text: str) -> Tensor:
-        tokenz = self.tokenizer.encode(text, add_special_tokens=False)
-        return tokenz
+        raise NotImplementedError()
 
     @abstractmethod
     def _get_lazy_logits(
         self,
         inputs: Tensor,
     ) -> Tensor:
         raise NotImplementedError()
 
-    def score(self, text: str) -> float:
+    def score(self, text: str, num_tokens: int = 24) -> float:
 
         outputs, tokenz = self.predict_logits_and_tokenz(text)
 
         output = outputs[0][0]
         rankings: List[int] = []
         for i in range(output.shape[0] - 1):
+            if i < num_tokens:
+                continue
             logit = output[i + 1, :]
             actual_token = tokenz[0, i]
             rankings.append(int((logit > logit[actual_token]).sum().item()))
 
-        return float(np.mean(rankings))
+        if len(rankings) == 0:
+            return -1.0
+        return float(np.mean(rankings) / output.shape[1])
 
     def is_human(self, text: str, treshold: float = 0.1) -> bool:
         return self.score(text) >= treshold
```

### Comparing `spot_llm-0.1.0/PKG-INFO` & `spot_llm-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: spot-llm
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Edouard Yvinec
+Author-email: edouardyvinec@hotmail.fr
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: accelerate (>=0.30.1,<0.31.0)
 Requires-Dist: loadingpy (>=0.1.4,<0.2.0)
```

