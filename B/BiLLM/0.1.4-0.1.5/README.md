# Comparing `tmp/billm-0.1.4.tar.gz` & `tmp/billm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "billm-0.1.4.tar", last modified: Wed May 22 08:36:43 2024, max compression
+gzip compressed data, was "billm-0.1.5.tar", last modified: Fri May 31 08:59:21 2024, max compression
```

## Comparing `billm-0.1.4.tar` & `billm-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1060 2024-03-14 10:50:27.655921 billm-0.1.4/LICENSE
--rw-r--r--   0        0        0     4352 2024-05-22 08:34:53.290584 billm-0.1.4/README.md
--rw-r--r--   0        0        0      486 2024-05-22 08:36:43.224875 billm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      205 2024-05-22 08:35:50.555270 billm-0.1.4/src/billm/__init__.py
--rw-r--r--   0        0        0      267 2024-03-17 05:50:48.094383 billm-0.1.4/src/billm/config.py
--rw-r--r--   0        0        0    14376 2024-05-22 08:34:53.296221 billm-0.1.4/src/billm/configuration_openelm.py
--rw-r--r--   0        0        0    29160 2024-05-22 08:34:53.299901 billm-0.1.4/src/billm/modeling_llama.py
--rw-r--r--   0        0        0    25657 2024-05-22 08:34:53.302473 billm-0.1.4/src/billm/modeling_mistral.py
--rw-r--r--   0        0        0    47882 2024-05-22 08:34:53.306016 billm-0.1.4/src/billm/modeling_openelm.py
--rw-r--r--   0        0        0    25453 2024-05-22 08:34:53.308417 billm-0.1.4/src/billm/modeling_qwen2.py
--rw-r--r--   0        0        0        0 2024-03-17 05:50:48.095776 billm-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-07 03:30:51.086211 billm-0.1.4/tests/test_modeling_llama.py
--rw-r--r--   0        0        0     2728 2024-04-07 03:30:51.087077 billm-0.1.4/tests/test_modeling_mistral.py
--rw-r--r--   0        0        0     2037 2024-05-22 08:34:53.311395 billm-0.1.4/tests/test_modeling_openelm.py
--rw-r--r--   0        0        0     2678 2024-04-07 03:30:51.087923 billm-0.1.4/tests/test_modeling_qwen2.py
--rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 billm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-25 06:59:49.322342 billm-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4429 2024-05-31 08:57:05.734046 billm-0.1.5/README.md
+-rw-r--r--   0        0        0      486 2024-05-31 08:59:21.030078 billm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-05-31 08:58:17.054214 billm-0.1.5/src/billm/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-25 06:59:49.324562 billm-0.1.5/src/billm/config.py
+-rw-r--r--   0        0        0    14376 2024-05-25 06:59:49.324778 billm-0.1.5/src/billm/configuration_openelm.py
+-rw-r--r--   0        0        0    29197 2024-05-31 08:57:05.769760 billm-0.1.5/src/billm/modeling_llama.py
+-rw-r--r--   0        0        0    25697 2024-05-31 08:57:05.794013 billm-0.1.5/src/billm/modeling_mistral.py
+-rw-r--r--   0        0        0    47919 2024-05-31 08:57:05.818981 billm-0.1.5/src/billm/modeling_openelm.py
+-rw-r--r--   0        0        0    25493 2024-05-31 08:57:05.825204 billm-0.1.5/src/billm/modeling_qwen2.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:59:49.326409 billm-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-25 06:59:49.326672 billm-0.1.5/tests/test_modeling_llama.py
+-rw-r--r--   0        0        0     2728 2024-05-25 06:59:49.326825 billm-0.1.5/tests/test_modeling_mistral.py
+-rw-r--r--   0        0        0     2037 2024-05-25 06:59:49.326955 billm-0.1.5/tests/test_modeling_openelm.py
+-rw-r--r--   0        0        0     2678 2024-05-25 06:59:49.327197 billm-0.1.5/tests/test_modeling_qwen2.py
+-rw-r--r--   0        0        0     4762 1970-01-01 00:00:00.000000 billm-0.1.5/PKG-INFO
```

### Comparing `billm-0.1.4/LICENSE` & `billm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `billm-0.1.4/README.md` & `billm-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
 </a>
 <a href="https://pdm-project.org">
     <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="https://pdm-project.org" />
 </a>
 
 
+## Supported Models
+
+- LLaMA
+- Mistral
+- Qwen2
+- OpenELM
+
 ## Usage
 
 1) `python -m pip install -U billm`
 
 2) Specify start index for bi-directional layers via `export BiLLM_START_INDEX={layer_index}`. if not specified, default is 0, i.e., all layers are bi-directional. If set to -1, BiLLM is disabled.
 
 3) Import LLMs from BiLLM and initialize them as usual with transformers.
@@ -99,21 +106,18 @@
 
 token_classifier = pipeline("token-classification", model=model, tokenizer=tokenizer, aggregation_strategy="simple")
 sentence = "I live in Hong Kong. I am a student at Hong Kong PolyU."
 tokens = token_classifier(sentence)
 print(tokens)
 ```
 
+### Sentence Embeddings
 
-## Supported Models
+refer to AnglE: https://github.com/SeanLee97/AnglE
 
-- LLaMA
-- Mistral
-- Qwen2
-- OpenELM
 
 ## Citation
 
 If you use this toolkit in your work, please cite the following paper:
 
 1) For sentence embeddings modeling:
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 # BiLLM Tool for converting LLMs from uni-directional to bi-directional for
 tasks like classification and sentence embeddings. Compatible with ð¤
 transformers. _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_1_0_._0_1_2_0_8_]_[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/
 _2_3_1_1_._0_5_2_9_6_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_:_/_/_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_]_[_h_t_t_p_s_:_/_/
-_p_d_m_-_p_r_o_j_e_c_t_._o_r_g_]## Usage 1) `python -m pip install -U billm` 2) Specify start
-index for bi-directional layers via `export BiLLM_START_INDEX={layer_index}`.
-if not specified, default is 0, i.e., all layers are bi-directional. If set to
--1, BiLLM is disabled. 3) Import LLMs from BiLLM and initialize them as usual
-with transformers. ```diff - from transformers import ( - LLamaModel, -
+_p_d_m_-_p_r_o_j_e_c_t_._o_r_g_]## Supported Models - LLaMA - Mistral - Qwen2 - OpenELM ##
+Usage 1) `python -m pip install -U billm` 2) Specify start index for bi-
+directional layers via `export BiLLM_START_INDEX={layer_index}`. if not
+specified, default is 0, i.e., all layers are bi-directional. If set to -1,
+BiLLM is disabled. 3) Import LLMs from BiLLM and initialize them as usual with
+transformers. ```diff - from transformers import ( - LLamaModel, -
 LLamaForCausalLM, - LLamaForSequenceClassification, - MistralModel, -
 MistralForCausalLM, - MistralForSequenceClassification - Qwen2Model, -
 Qwen2ForCausalLM, - Qwen2ForSequenceClassification - ) + from billm import ( +
 LLamaModel, + LLamaForCausalLM, + LLamaForSequenceClassification, +
 LLamaForTokenClassification, + MistralModel, + MistralForCausalLM, +
 MistralForSequenceClassification, + MistralForTokenClassification, +
 Qwen2Model, + Qwen2ForCausalLM, + Qwen2ForSequenceClassification, +
@@ -29,19 +30,19 @@
 MistralForTokenClassification.from_pretrained
 ( peft_config.base_model_name_or_path, num_labels=len(label2id),
 id2label=id2label, label2id=label2id ) model = PeftModel.from_pretrained(model,
 model_id) # merge and unload is necessary for inference model =
 model.merge_and_unload() token_classifier = pipeline("token-classification",
 model=model, tokenizer=tokenizer, aggregation_strategy="simple") sentence = "I
 live in Hong Kong. I am a student at Hong Kong PolyU." tokens =
-token_classifier(sentence) print(tokens) ``` ## Supported Models - LLaMA -
-Mistral - Qwen2 - OpenELM ## Citation If you use this toolkit in your work,
-please cite the following paper: 1) For sentence embeddings modeling: ```bibtex
-@inproceedings{li2024bellm, title = "BeLLM: Backward Dependency Enhanced Large
-Language Model for Sentence Embeddings", author = "Li, Xianming and Li, Jing",
-booktitle = "Proceedings of the 2024 Conference of the North American Chapter
-of the Association for Computational Linguistics", year = "2024", publisher =
-"Association for Computational Linguistics" } ``` 2) For other tasks: ```bibtex
-@article{li2023label, title={Label supervised llama finetuning}, author={Li,
-Zongxi and Li, Xianming and Liu, Yuzhang and Xie, Haoran and Li, Jing and Wang,
-Fu-lee and Li, Qing and Zhong, Xiaoqin}, journal={arXiv preprint arXiv:
-2310.01208}, year={2023} } ```
+token_classifier(sentence) print(tokens) ``` ### Sentence Embeddings refer to
+AnglE: https://github.com/SeanLee97/AnglE ## Citation If you use this toolkit
+in your work, please cite the following paper: 1) For sentence embeddings
+modeling: ```bibtex @inproceedings{li2024bellm, title = "BeLLM: Backward
+Dependency Enhanced Large Language Model for Sentence Embeddings", author =
+"Li, Xianming and Li, Jing", booktitle = "Proceedings of the 2024 Conference of
+the North American Chapter of the Association for Computational Linguistics",
+year = "2024", publisher = "Association for Computational Linguistics" } ``` 2)
+For other tasks: ```bibtex @article{li2023label, title={Label supervised llama
+finetuning}, author={Li, Zongxi and Li, Xianming and Liu, Yuzhang and Xie,
+Haoran and Li, Jing and Wang, Fu-lee and Li, Qing and Zhong, Xiaoqin}, journal=
+{arXiv preprint arXiv:2310.01208}, year={2023} } ```
```

### Comparing `billm-0.1.4/src/billm/configuration_openelm.py` & `billm-0.1.5/src/billm/configuration_openelm.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.4/src/billm/modeling_llama.py` & `billm-0.1.5/src/billm/modeling_llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         if position_ids is None:
             position_ids = cache_position.unsqueeze(0)
 
         causal_mask = self._update_causal_mask(
             attention_mask, inputs_embeds, cache_position, past_seen_tokens + inputs_embeds.shape[1]
         )
-        bi_attention_mask = torch.zeros_like(causal_mask)
+        bi_attention_mask = torch.zeros_like(causal_mask) if causal_mask is not None else None
 
         # embed positions
         hidden_states = inputs_embeds
 
         # decoder layers
         all_hidden_states = () if output_hidden_states else None
         all_self_attns = () if output_attentions else None
```

### Comparing `billm-0.1.4/src/billm/modeling_mistral.py` & `billm-0.1.5/src/billm/modeling_mistral.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             attention_mask = _prepare_4d_causal_attention_mask(
                 attention_mask,
                 (batch_size, seq_length),
                 inputs_embeds,
                 past_key_values_length,
                 sliding_window=self.config.sliding_window,
             )
-        bi_attention_mask = torch.zeros_like(attention_mask)
+        bi_attention_mask = torch.zeros_like(attention_mask) if attention_mask is not None else None
 
         hidden_states = inputs_embeds
 
         # decoder layers
         all_hidden_states = () if output_hidden_states else None
         all_self_attns = () if output_attentions else None
         next_decoder_cache = None
```

### Comparing `billm-0.1.4/src/billm/modeling_openelm.py` & `billm-0.1.5/src/billm/modeling_openelm.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,15 +654,15 @@
                 device=inputs_embeds.device,
             )
 
         if position_ids is None:
             position_ids = cache_position.unsqueeze(0)
 
         causal_mask = self._update_causal_mask(attention_mask, inputs_embeds)
-        bi_attention_mask = torch.zeros_like(causal_mask)
+        bi_attention_mask = torch.zeros_like(causal_mask) if causal_mask is not None else None
 
         # embed positions
         hidden_states = inputs_embeds
 
         # decoder layers
         all_hidden_states = () if output_hidden_states else None
         all_self_attns = () if output_attentions else None
```

### Comparing `billm-0.1.4/src/billm/modeling_qwen2.py` & `billm-0.1.5/src/billm/modeling_qwen2.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             attention_mask = _prepare_4d_causal_attention_mask(
                 attention_mask,
                 (batch_size, seq_length),
                 inputs_embeds,
                 past_key_values_length,
                 sliding_window=self.config.sliding_window,
             )
-        bi_attention_mask = torch.zeros_like(attention_mask)
+        bi_attention_mask = torch.zeros_like(attention_mask) if attention_mask is not None else None
 
         hidden_states = inputs_embeds
 
         # decoder layers
         all_hidden_states = () if output_hidden_states else None
         all_self_attns = () if output_attentions else None
         next_decoder_cache = None
```

### Comparing `billm-0.1.4/tests/test_modeling_llama.py` & `billm-0.1.5/tests/test_modeling_llama.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.4/tests/test_modeling_mistral.py` & `billm-0.1.5/tests/test_modeling_mistral.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.4/tests/test_modeling_openelm.py` & `billm-0.1.5/tests/test_modeling_openelm.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.4/tests/test_modeling_qwen2.py` & `billm-0.1.5/tests/test_modeling_qwen2.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.4/PKG-INFO` & `billm-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiLLM
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool for converting LLMs from uni-directional to bi-directional for tasks like classification and sentence embeddings.
 Author-Email: Sean Lee <xmlee97@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: transformers>=4.38.2
 Description-Content-Type: text/markdown
 
@@ -27,14 +27,21 @@
     <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
 </a>
 <a href="https://pdm-project.org">
     <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="https://pdm-project.org" />
 </a>
 
 
+## Supported Models
+
+- LLaMA
+- Mistral
+- Qwen2
+- OpenELM
+
 ## Usage
 
 1) `python -m pip install -U billm`
 
 2) Specify start index for bi-directional layers via `export BiLLM_START_INDEX={layer_index}`. if not specified, default is 0, i.e., all layers are bi-directional. If set to -1, BiLLM is disabled.
 
 3) Import LLMs from BiLLM and initialize them as usual with transformers.
@@ -109,21 +116,18 @@
 
 token_classifier = pipeline("token-classification", model=model, tokenizer=tokenizer, aggregation_strategy="simple")
 sentence = "I live in Hong Kong. I am a student at Hong Kong PolyU."
 tokens = token_classifier(sentence)
 print(tokens)
 ```
 
+### Sentence Embeddings
 
-## Supported Models
+refer to AnglE: https://github.com/SeanLee97/AnglE
 
-- LLaMA
-- Mistral
-- Qwen2
-- OpenELM
 
 ## Citation
 
 If you use this toolkit in your work, please cite the following paper:
 
 1) For sentence embeddings modeling:
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: BiLLM Version: 0.1.4 Summary: Tool for converting
+Metadata-Version: 2.1 Name: BiLLM Version: 0.1.5 Summary: Tool for converting
 LLMs from uni-directional to bi-directional for tasks like classification and
 sentence embeddings. Author-Email: Sean Lee
 gmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist:
 transformers>=4.38.2 Description-Content-Type: text/markdown # BiLLM Tool for
 converting LLMs from uni-directional to bi-directional for tasks like
 classification and sentence embeddings. Compatible with ð¤ transformers.
 _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_1_0_._0_1_2_0_8_]_[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_1_1_._0_5_2_9_6_]_[_P_y_P_I
 _v_e_r_s_i_o_n_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_:_/_/_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_]_[_h_t_t_p_s_:_/_/_p_d_m_-
-_p_r_o_j_e_c_t_._o_r_g_]## Usage 1) `python -m pip install -U billm` 2) Specify start index
-for bi-directional layers via `export BiLLM_START_INDEX={layer_index}`. if not
-specified, default is 0, i.e., all layers are bi-directional. If set to -1,
-BiLLM is disabled. 3) Import LLMs from BiLLM and initialize them as usual with
-transformers. ```diff - from transformers import ( - LLamaModel, -
-LLamaForCausalLM, - LLamaForSequenceClassification, - MistralModel, -
-MistralForCausalLM, - MistralForSequenceClassification - Qwen2Model, -
-Qwen2ForCausalLM, - Qwen2ForSequenceClassification - ) + from billm import ( +
-LLamaModel, + LLamaForCausalLM, + LLamaForSequenceClassification, +
+_p_r_o_j_e_c_t_._o_r_g_]## Supported Models - LLaMA - Mistral - Qwen2 - OpenELM ## Usage 1)
+`python -m pip install -U billm` 2) Specify start index for bi-directional
+layers via `export BiLLM_START_INDEX={layer_index}`. if not specified, default
+is 0, i.e., all layers are bi-directional. If set to -1, BiLLM is disabled. 3)
+Import LLMs from BiLLM and initialize them as usual with transformers. ```diff
+- from transformers import ( - LLamaModel, - LLamaForCausalLM, -
+LLamaForSequenceClassification, - MistralModel, - MistralForCausalLM, -
+MistralForSequenceClassification - Qwen2Model, - Qwen2ForCausalLM, -
+Qwen2ForSequenceClassification - ) + from billm import ( + LLamaModel, +
+LLamaForCausalLM, + LLamaForSequenceClassification, +
 LLamaForTokenClassification, + MistralModel, + MistralForCausalLM, +
 MistralForSequenceClassification, + MistralForTokenClassification, +
 Qwen2Model, + Qwen2ForCausalLM, + Qwen2ForSequenceClassification, +
 Qwen2ForTokenClassification + OpenELMModel, + OpenELMForCausalLM, +
 OpenELMForSequenceClassification, + OpenELMForTokenClassification + ) ``` ##
 Examples ### NER **training:** ```bash $ cd examples $ WANDB_MODE=disabled
 BiLLM_START_INDEX=0 CUDA_VISIBLE_DEVICES=3 python billm_ner.py \ --
@@ -34,19 +35,19 @@
 MistralForTokenClassification.from_pretrained
 ( peft_config.base_model_name_or_path, num_labels=len(label2id),
 id2label=id2label, label2id=label2id ) model = PeftModel.from_pretrained(model,
 model_id) # merge and unload is necessary for inference model =
 model.merge_and_unload() token_classifier = pipeline("token-classification",
 model=model, tokenizer=tokenizer, aggregation_strategy="simple") sentence = "I
 live in Hong Kong. I am a student at Hong Kong PolyU." tokens =
-token_classifier(sentence) print(tokens) ``` ## Supported Models - LLaMA -
-Mistral - Qwen2 - OpenELM ## Citation If you use this toolkit in your work,
-please cite the following paper: 1) For sentence embeddings modeling: ```bibtex
-@inproceedings{li2024bellm, title = "BeLLM: Backward Dependency Enhanced Large
-Language Model for Sentence Embeddings", author = "Li, Xianming and Li, Jing",
-booktitle = "Proceedings of the 2024 Conference of the North American Chapter
-of the Association for Computational Linguistics", year = "2024", publisher =
-"Association for Computational Linguistics" } ``` 2) For other tasks: ```bibtex
-@article{li2023label, title={Label supervised llama finetuning}, author={Li,
-Zongxi and Li, Xianming and Liu, Yuzhang and Xie, Haoran and Li, Jing and Wang,
-Fu-lee and Li, Qing and Zhong, Xiaoqin}, journal={arXiv preprint arXiv:
-2310.01208}, year={2023} } ```
+token_classifier(sentence) print(tokens) ``` ### Sentence Embeddings refer to
+AnglE: https://github.com/SeanLee97/AnglE ## Citation If you use this toolkit
+in your work, please cite the following paper: 1) For sentence embeddings
+modeling: ```bibtex @inproceedings{li2024bellm, title = "BeLLM: Backward
+Dependency Enhanced Large Language Model for Sentence Embeddings", author =
+"Li, Xianming and Li, Jing", booktitle = "Proceedings of the 2024 Conference of
+the North American Chapter of the Association for Computational Linguistics",
+year = "2024", publisher = "Association for Computational Linguistics" } ``` 2)
+For other tasks: ```bibtex @article{li2023label, title={Label supervised llama
+finetuning}, author={Li, Zongxi and Li, Xianming and Liu, Yuzhang and Xie,
+Haoran and Li, Jing and Wang, Fu-lee and Li, Qing and Zhong, Xiaoqin}, journal=
+{arXiv preprint arXiv:2310.01208}, year={2023} } ```
```

