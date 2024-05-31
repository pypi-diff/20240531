# Comparing `tmp/generalagent-0.2.8.tar.gz` & `tmp/generalagent-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalagent-0.2.8.tar", max compression
+gzip compressed data, was "generalagent-0.2.9.tar", max compression
```

## Comparing `generalagent-0.2.8.tar` & `generalagent-0.2.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0       92 2024-01-10 06:08:20.294775 generalagent-0.2.8/GeneralAgent/__init__.py
--rw-r--r--   0        0        0      338 2024-02-01 08:24:41.370558 generalagent-0.2.8/GeneralAgent/agent/__init__.py
--rw-r--r--   0        0        0     2865 2024-03-12 05:09:42.317861 generalagent-0.2.8/GeneralAgent/agent/abs_agent.py
--rw-r--r--   0        0        0     9071 2024-03-12 05:08:38.380927 generalagent-0.2.8/GeneralAgent/agent/normal_agent.py
--rw-r--r--   0        0        0     1348 2023-12-20 13:11:57.130304 generalagent-0.2.8/GeneralAgent/cli.py
--rw-r--r--   0        0        0        0 2024-01-10 06:08:20.296275 generalagent-0.2.8/GeneralAgent/function_searcher/__init__.py
--rw-r--r--   0        0        0     2280 2024-01-19 03:58:46.245778 generalagent-0.2.8/GeneralAgent/function_searcher/function_searcher.py
--rw-r--r--   0        0        0      618 2024-01-10 06:08:20.296866 generalagent-0.2.8/GeneralAgent/interpreter/__init__.py
--rw-r--r--   0        0        0     1405 2023-12-20 13:11:57.131045 generalagent-0.2.8/GeneralAgent/interpreter/applescript_interpreter.py
--rw-r--r--   0        0        0     3209 2023-12-20 13:11:57.131296 generalagent-0.2.8/GeneralAgent/interpreter/embedding_retrieve_interpreter.py
--rw-r--r--   0        0        0     4647 2023-12-20 13:11:57.131506 generalagent-0.2.8/GeneralAgent/interpreter/file_interpreter.py
--rw-r--r--   0        0        0     2799 2024-01-04 02:04:50.012763 generalagent-0.2.8/GeneralAgent/interpreter/interpreter.py
--rw-r--r--   0        0        0     2243 2024-01-08 08:40:00.101417 generalagent-0.2.8/GeneralAgent/interpreter/link_retrieve_interpreter.py
--rw-r--r--   0        0        0     7619 2024-03-14 07:20:36.100510 generalagent-0.2.8/GeneralAgent/interpreter/python_interpreter.py
--rw-r--r--   0        0        0     2085 2024-03-12 02:28:04.988819 generalagent-0.2.8/GeneralAgent/interpreter/role_interpreter.py
--rw-r--r--   0        0        0     1304 2023-12-20 13:11:57.133328 generalagent-0.2.8/GeneralAgent/interpreter/shell_interpreter.py
--rw-r--r--   0        0        0     1668 2024-01-04 02:04:41.665472 generalagent-0.2.8/GeneralAgent/interpreter/ui_interpreter.py
--rw-r--r--   0        0        0      156 2024-01-10 06:08:20.297735 generalagent-0.2.8/GeneralAgent/memory/__init__.py
--rw-r--r--   0        0        0     4554 2024-01-10 06:08:20.298143 generalagent-0.2.8/GeneralAgent/memory/link_memory.py
--rw-r--r--   0        0        0     2844 2024-01-10 06:08:20.298531 generalagent-0.2.8/GeneralAgent/memory/normal_memory.py
--rw-r--r--   0        0        0     7723 2024-01-10 06:08:20.298772 generalagent-0.2.8/GeneralAgent/memory/stack_memory.py
--rw-r--r--   0        0        0       28 2023-11-28 03:34:58.141227 generalagent-0.2.8/GeneralAgent/pytest.ini
--rw-r--r--   0        0        0      526 2023-11-20 09:19:54.599123 generalagent-0.2.8/GeneralAgent/requirements.txt
--rw-r--r--   0        0        0     3614 2024-03-13 08:18:44.493735 generalagent-0.2.8/GeneralAgent/skills/__init__.py
--rw-r--r--   0        0        0    13046 2024-01-10 06:08:20.299305 generalagent-0.2.8/GeneralAgent/skills/agent_builder_2.py
--rw-r--r--   0        0        0     4139 2023-12-21 10:41:10.246412 generalagent-0.2.8/GeneralAgent/skills/agents.py
--rw-r--r--   0        0        0      754 2023-11-08 03:05:34.056233 generalagent-0.2.8/GeneralAgent/skills/ai_draw_prompt_gen.py
--rw-r--r--   0        0        0     2211 2024-01-19 05:48:12.001695 generalagent-0.2.8/GeneralAgent/skills/ai_tools.py
--rw-r--r--   0        0        0    24317 2024-01-10 06:08:20.299994 generalagent-0.2.8/GeneralAgent/skills/application_builder.py
--rw-r--r--   0        0        0     3057 2024-01-30 12:49:10.117681 generalagent-0.2.8/GeneralAgent/skills/applications.py
--rw-r--r--   0        0        0     4628 2023-11-26 15:15:57.709933 generalagent-0.2.8/GeneralAgent/skills/build_web.py
--rw-r--r--   0        0        0      979 2023-12-01 14:32:37.053345 generalagent-0.2.8/GeneralAgent/skills/concatenate_videos/concatenate_videos.py
--rw-r--r--   0        0        0   216787 2023-12-01 14:30:29.378783 generalagent-0.2.8/GeneralAgent/skills/concatenate_videos/f63bfaae7b0e.mp4
--rw-r--r--   0        0        0     1495 2023-12-25 03:37:33.842196 generalagent-0.2.8/GeneralAgent/skills/download_file.py
--rw-r--r--   0        0        0     1764 2023-11-26 15:16:39.451045 generalagent-0.2.8/GeneralAgent/skills/file_operation.py
--rw-r--r--   0        0        0    16295 2024-02-22 07:11:45.729571 generalagent-0.2.8/GeneralAgent/skills/llm_inference.py
--rw-r--r--   0        0        0     4026 2023-12-20 13:11:57.135505 generalagent-0.2.8/GeneralAgent/skills/markdown_to_ppt/bid_plan.md
--rw-r--r--   0        0        0     3183 2023-12-20 13:11:57.135839 generalagent-0.2.8/GeneralAgent/skills/markdown_to_ppt/markdown_to_ppt.py
--rw-r--r--   0        0        0     4946 2024-01-10 06:08:20.301312 generalagent-0.2.8/GeneralAgent/skills/memory_utils.py
--rw-r--r--   0        0        0     2382 2023-12-02 06:14:00.874028 generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/merge_video_audio.py
--rw-r--r--   0        0        0  3840078 2023-12-01 07:24:08.962442 generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/music.wav
--rw-r--r--   0        0        0   133920 2023-12-01 07:22:01.878983 generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/narration.mp3
--rw-r--r--   0        0        0      237 2023-12-01 08:04:02.083062 generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/tmp_audio.mp3
--rw-r--r--   0        0        0   248535 2023-12-01 07:17:44.560401 generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/video.mp4
--rw-r--r--   0        0        0     1316 2023-12-01 04:07:04.632327 generalagent-0.2.8/GeneralAgent/skills/musicgen/generate_music.py
--rw-r--r--   0        0        0     4982 2024-03-01 05:26:24.789591 generalagent-0.2.8/GeneralAgent/skills/python_envs.py
--rw-r--r--   0        0        0     2677 2024-01-10 06:08:20.301818 generalagent-0.2.8/GeneralAgent/skills/replicate_api.py
--rw-r--r--   0        0        0      970 2023-11-01 07:12:13.390767 generalagent-0.2.8/GeneralAgent/skills/split_text.py
--rw-r--r--   0        0        0    89301 2023-11-09 03:28:53.719455 generalagent-0.2.8/GeneralAgent/skills/stable_video_diffusion/dab774a452f3.jpg
--rw-r--r--   0        0        0     2222 2023-12-01 15:06:04.566769 generalagent-0.2.8/GeneralAgent/skills/stable_video_diffusion/stable_video_diffusion.py
--rw-r--r--   0        0        0      575 2023-08-28 03:15:56.578103 generalagent-0.2.8/GeneralAgent/skills/text_is_english.py
--rw-r--r--   0        0        0     2772 2024-01-10 06:08:20.302093 generalagent-0.2.8/GeneralAgent/skills/text_translation.py
--rw-r--r--   0        0        0      970 2023-10-24 00:40:33.817982 generalagent-0.2.8/GeneralAgent/skills/token_count.py
--rw-r--r--   0        0        0      653 2023-10-24 15:26:16.577709 generalagent-0.2.8/GeneralAgent/skills/unique_name.py
--rw-r--r--   0        0        0     6289 2024-01-10 06:08:20.302383 generalagent-0.2.8/GeneralAgent/skills/web_tools.py
--rw-r--r--   0        0        0     3043 2023-12-22 16:01:22.700532 generalagent-0.2.8/GeneralAgent/skills/web_tools_advance.py
--rw-r--r--   0        0        0     4462 2024-02-18 07:33:34.128386 generalagent-0.2.8/GeneralAgent/utils.py
--rw-r--r--   0        0        0    11338 2023-12-25 06:05:09.537613 generalagent-0.2.8/LICENSE
--rw-r--r--   0        0        0     4160 2024-01-28 12:18:12.506561 generalagent-0.2.8/README.md
--rw-r--r--   0        0        0     1294 2024-03-14 07:21:54.854377 generalagent-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6021 1970-01-01 00:00:00.000000 generalagent-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       92 2024-01-10 06:08:20.294775 generalagent-0.2.9/GeneralAgent/__init__.py
+-rw-r--r--   0        0        0      338 2024-02-01 08:24:41.370558 generalagent-0.2.9/GeneralAgent/agent/__init__.py
+-rw-r--r--   0        0        0     2865 2024-03-12 05:09:42.317861 generalagent-0.2.9/GeneralAgent/agent/abs_agent.py
+-rw-r--r--   0        0        0     9252 2024-03-18 01:38:12.949838 generalagent-0.2.9/GeneralAgent/agent/normal_agent.py
+-rw-r--r--   0        0        0     1348 2023-12-20 13:11:57.130304 generalagent-0.2.9/GeneralAgent/cli.py
+-rw-r--r--   0        0        0        0 2024-01-10 06:08:20.296275 generalagent-0.2.9/GeneralAgent/function_searcher/__init__.py
+-rw-r--r--   0        0        0     2280 2024-01-19 03:58:46.245778 generalagent-0.2.9/GeneralAgent/function_searcher/function_searcher.py
+-rw-r--r--   0        0        0      618 2024-01-10 06:08:20.296866 generalagent-0.2.9/GeneralAgent/interpreter/__init__.py
+-rw-r--r--   0        0        0     1405 2023-12-20 13:11:57.131045 generalagent-0.2.9/GeneralAgent/interpreter/applescript_interpreter.py
+-rw-r--r--   0        0        0     3209 2023-12-20 13:11:57.131296 generalagent-0.2.9/GeneralAgent/interpreter/embedding_retrieve_interpreter.py
+-rw-r--r--   0        0        0     4647 2023-12-20 13:11:57.131506 generalagent-0.2.9/GeneralAgent/interpreter/file_interpreter.py
+-rw-r--r--   0        0        0     2799 2024-01-04 02:04:50.012763 generalagent-0.2.9/GeneralAgent/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2243 2024-01-08 08:40:00.101417 generalagent-0.2.9/GeneralAgent/interpreter/link_retrieve_interpreter.py
+-rw-r--r--   0        0        0     7619 2024-03-14 07:20:36.100510 generalagent-0.2.9/GeneralAgent/interpreter/python_interpreter.py
+-rw-r--r--   0        0        0     2085 2024-03-12 02:28:04.988819 generalagent-0.2.9/GeneralAgent/interpreter/role_interpreter.py
+-rw-r--r--   0        0        0     1304 2023-12-20 13:11:57.133328 generalagent-0.2.9/GeneralAgent/interpreter/shell_interpreter.py
+-rw-r--r--   0        0        0     1668 2024-01-04 02:04:41.665472 generalagent-0.2.9/GeneralAgent/interpreter/ui_interpreter.py
+-rw-r--r--   0        0        0      156 2024-01-10 06:08:20.297735 generalagent-0.2.9/GeneralAgent/memory/__init__.py
+-rw-r--r--   0        0        0     4554 2024-01-10 06:08:20.298143 generalagent-0.2.9/GeneralAgent/memory/link_memory.py
+-rw-r--r--   0        0        0     2844 2024-01-10 06:08:20.298531 generalagent-0.2.9/GeneralAgent/memory/normal_memory.py
+-rw-r--r--   0        0        0     7723 2024-01-10 06:08:20.298772 generalagent-0.2.9/GeneralAgent/memory/stack_memory.py
+-rw-r--r--   0        0        0       28 2023-11-28 03:34:58.141227 generalagent-0.2.9/GeneralAgent/pytest.ini
+-rw-r--r--   0        0        0      526 2023-11-20 09:19:54.599123 generalagent-0.2.9/GeneralAgent/requirements.txt
+-rw-r--r--   0        0        0     3614 2024-03-13 08:18:44.493735 generalagent-0.2.9/GeneralAgent/skills/__init__.py
+-rw-r--r--   0        0        0    13046 2024-01-10 06:08:20.299305 generalagent-0.2.9/GeneralAgent/skills/agent_builder_2.py
+-rw-r--r--   0        0        0     4139 2023-12-21 10:41:10.246412 generalagent-0.2.9/GeneralAgent/skills/agents.py
+-rw-r--r--   0        0        0      754 2023-11-08 03:05:34.056233 generalagent-0.2.9/GeneralAgent/skills/ai_draw_prompt_gen.py
+-rw-r--r--   0        0        0     2211 2024-01-19 05:48:12.001695 generalagent-0.2.9/GeneralAgent/skills/ai_tools.py
+-rw-r--r--   0        0        0    24317 2024-01-10 06:08:20.299994 generalagent-0.2.9/GeneralAgent/skills/application_builder.py
+-rw-r--r--   0        0        0     3057 2024-01-30 12:49:10.117681 generalagent-0.2.9/GeneralAgent/skills/applications.py
+-rw-r--r--   0        0        0     4628 2023-11-26 15:15:57.709933 generalagent-0.2.9/GeneralAgent/skills/build_web.py
+-rw-r--r--   0        0        0      979 2023-12-01 14:32:37.053345 generalagent-0.2.9/GeneralAgent/skills/concatenate_videos/concatenate_videos.py
+-rw-r--r--   0        0        0   216787 2023-12-01 14:30:29.378783 generalagent-0.2.9/GeneralAgent/skills/concatenate_videos/f63bfaae7b0e.mp4
+-rw-r--r--   0        0        0     1495 2023-12-25 03:37:33.842196 generalagent-0.2.9/GeneralAgent/skills/download_file.py
+-rw-r--r--   0        0        0     1764 2023-11-26 15:16:39.451045 generalagent-0.2.9/GeneralAgent/skills/file_operation.py
+-rw-r--r--   0        0        0    16295 2024-02-22 07:11:45.729571 generalagent-0.2.9/GeneralAgent/skills/llm_inference.py
+-rw-r--r--   0        0        0     4026 2023-12-20 13:11:57.135505 generalagent-0.2.9/GeneralAgent/skills/markdown_to_ppt/bid_plan.md
+-rw-r--r--   0        0        0     3183 2023-12-20 13:11:57.135839 generalagent-0.2.9/GeneralAgent/skills/markdown_to_ppt/markdown_to_ppt.py
+-rw-r--r--   0        0        0     4946 2024-01-10 06:08:20.301312 generalagent-0.2.9/GeneralAgent/skills/memory_utils.py
+-rw-r--r--   0        0        0     2382 2023-12-02 06:14:00.874028 generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/merge_video_audio.py
+-rw-r--r--   0        0        0  3840078 2023-12-01 07:24:08.962442 generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/music.wav
+-rw-r--r--   0        0        0   133920 2023-12-01 07:22:01.878983 generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/narration.mp3
+-rw-r--r--   0        0        0      237 2023-12-01 08:04:02.083062 generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/tmp_audio.mp3
+-rw-r--r--   0        0        0   248535 2023-12-01 07:17:44.560401 generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/video.mp4
+-rw-r--r--   0        0        0     1316 2023-12-01 04:07:04.632327 generalagent-0.2.9/GeneralAgent/skills/musicgen/generate_music.py
+-rw-r--r--   0        0        0     4982 2024-03-01 05:26:24.789591 generalagent-0.2.9/GeneralAgent/skills/python_envs.py
+-rw-r--r--   0        0        0     2677 2024-01-10 06:08:20.301818 generalagent-0.2.9/GeneralAgent/skills/replicate_api.py
+-rw-r--r--   0        0        0      970 2023-11-01 07:12:13.390767 generalagent-0.2.9/GeneralAgent/skills/split_text.py
+-rw-r--r--   0        0        0    89301 2023-11-09 03:28:53.719455 generalagent-0.2.9/GeneralAgent/skills/stable_video_diffusion/dab774a452f3.jpg
+-rw-r--r--   0        0        0     2222 2023-12-01 15:06:04.566769 generalagent-0.2.9/GeneralAgent/skills/stable_video_diffusion/stable_video_diffusion.py
+-rw-r--r--   0        0        0      575 2023-08-28 03:15:56.578103 generalagent-0.2.9/GeneralAgent/skills/text_is_english.py
+-rw-r--r--   0        0        0     2772 2024-01-10 06:08:20.302093 generalagent-0.2.9/GeneralAgent/skills/text_translation.py
+-rw-r--r--   0        0        0      970 2023-10-24 00:40:33.817982 generalagent-0.2.9/GeneralAgent/skills/token_count.py
+-rw-r--r--   0        0        0      653 2023-10-24 15:26:16.577709 generalagent-0.2.9/GeneralAgent/skills/unique_name.py
+-rw-r--r--   0        0        0     6289 2024-01-10 06:08:20.302383 generalagent-0.2.9/GeneralAgent/skills/web_tools.py
+-rw-r--r--   0        0        0     3043 2023-12-22 16:01:22.700532 generalagent-0.2.9/GeneralAgent/skills/web_tools_advance.py
+-rw-r--r--   0        0        0     4462 2024-02-18 07:33:34.128386 generalagent-0.2.9/GeneralAgent/utils.py
+-rw-r--r--   0        0        0    11338 2023-12-25 06:05:09.537613 generalagent-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4160 2024-01-28 12:18:12.506561 generalagent-0.2.9/README.md
+-rw-r--r--   0        0        0     1294 2024-03-18 01:53:19.463083 generalagent-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6021 1970-01-01 00:00:00.000000 generalagent-0.2.9/PKG-INFO
```

### Comparing `generalagent-0.2.8/GeneralAgent/agent/abs_agent.py` & `generalagent-0.2.9/GeneralAgent/agent/abs_agent.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/agent/normal_agent.py` & `generalagent-0.2.9/GeneralAgent/agent/normal_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,25 +48,29 @@
         bash_interpreter = ShellInterpreter(workspace)
         applescript_interpreter = AppleScriptInterpreter()
         file_interpreter = FileInterpreter()
         agent.interpreters = [role_interpreter, retrieve_interperter, python_interpreter, bash_interpreter, applescript_interpreter, file_interpreter]
         return agent
 
     @classmethod
-    def with_functions(cls, functions, role_prompt=None, workspace = './', model_type='smart', variables=None):
+    def with_functions(cls, functions, system_prompt=None, role_prompt=None, workspace = './', model_type='smart', variables=None):
         """
         agent with functions
         @functions: list, [function1, function2, ...]
+        @system_prompt: str, system prompt
         @role_prompt: str, role prompt
         @workspace: str, workspace path
         @model_type: str, 'smart', 'normal', or 'long'
         @variables: dict, embed variables to python interpreter, like {'a': a, 'variable_name': variable_value}, then Agent can use the variables in python interpreter like `variable_name`
         """
         agent = cls(workspace)
-        role_interpreter = RoleInterpreter()
+        if system_prompt is not None:
+            role_interpreter = RoleInterpreter()
+        else:
+            role_interpreter = RoleInterpreter(system_prompt)
         python_interpreter = PythonInterpreter(agent, serialize_path=f'{workspace}/code.bin')
         python_interpreter.function_tools = functions
         agent.interpreters = [role_interpreter, python_interpreter]
         agent.model_type = model_type
         if role_prompt is not None:
             agent.add_role_prompt(role_prompt)
         if variables is not None:
```

### Comparing `generalagent-0.2.8/GeneralAgent/cli.py` & `generalagent-0.2.9/GeneralAgent/cli.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/function_searcher/function_searcher.py` & `generalagent-0.2.9/GeneralAgent/function_searcher/function_searcher.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/__init__.py` & `generalagent-0.2.9/GeneralAgent/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/applescript_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/applescript_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/embedding_retrieve_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/embedding_retrieve_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/file_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/file_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/link_retrieve_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/link_retrieve_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/python_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/role_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/role_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/shell_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/shell_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/interpreter/ui_interpreter.py` & `generalagent-0.2.9/GeneralAgent/interpreter/ui_interpreter.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/memory/link_memory.py` & `generalagent-0.2.9/GeneralAgent/memory/link_memory.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/memory/normal_memory.py` & `generalagent-0.2.9/GeneralAgent/memory/normal_memory.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/memory/stack_memory.py` & `generalagent-0.2.9/GeneralAgent/memory/stack_memory.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/requirements.txt` & `generalagent-0.2.9/GeneralAgent/requirements.txt`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/__init__.py` & `generalagent-0.2.9/GeneralAgent/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/agent_builder_2.py` & `generalagent-0.2.9/GeneralAgent/skills/agent_builder_2.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/agents.py` & `generalagent-0.2.9/GeneralAgent/skills/agents.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/ai_draw_prompt_gen.py` & `generalagent-0.2.9/GeneralAgent/skills/ai_draw_prompt_gen.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/ai_tools.py` & `generalagent-0.2.9/GeneralAgent/skills/ai_tools.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/application_builder.py` & `generalagent-0.2.9/GeneralAgent/skills/application_builder.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/applications.py` & `generalagent-0.2.9/GeneralAgent/skills/applications.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/build_web.py` & `generalagent-0.2.9/GeneralAgent/skills/build_web.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/concatenate_videos/concatenate_videos.py` & `generalagent-0.2.9/GeneralAgent/skills/concatenate_videos/concatenate_videos.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/concatenate_videos/f63bfaae7b0e.mp4` & `generalagent-0.2.9/GeneralAgent/skills/concatenate_videos/f63bfaae7b0e.mp4`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/download_file.py` & `generalagent-0.2.9/GeneralAgent/skills/download_file.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/file_operation.py` & `generalagent-0.2.9/GeneralAgent/skills/file_operation.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/llm_inference.py` & `generalagent-0.2.9/GeneralAgent/skills/llm_inference.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/markdown_to_ppt/bid_plan.md` & `generalagent-0.2.9/GeneralAgent/skills/markdown_to_ppt/bid_plan.md`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/markdown_to_ppt/markdown_to_ppt.py` & `generalagent-0.2.9/GeneralAgent/skills/markdown_to_ppt/markdown_to_ppt.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/memory_utils.py` & `generalagent-0.2.9/GeneralAgent/skills/memory_utils.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/merge_video_audio.py` & `generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/merge_video_audio.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/music.wav` & `generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/music.wav`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/narration.mp3` & `generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/narration.mp3`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/merge_video_audio/video.mp4` & `generalagent-0.2.9/GeneralAgent/skills/merge_video_audio/video.mp4`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/musicgen/generate_music.py` & `generalagent-0.2.9/GeneralAgent/skills/musicgen/generate_music.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/python_envs.py` & `generalagent-0.2.9/GeneralAgent/skills/python_envs.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/replicate_api.py` & `generalagent-0.2.9/GeneralAgent/skills/replicate_api.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/split_text.py` & `generalagent-0.2.9/GeneralAgent/skills/split_text.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/stable_video_diffusion/dab774a452f3.jpg` & `generalagent-0.2.9/GeneralAgent/skills/stable_video_diffusion/dab774a452f3.jpg`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/stable_video_diffusion/stable_video_diffusion.py` & `generalagent-0.2.9/GeneralAgent/skills/stable_video_diffusion/stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/text_is_english.py` & `generalagent-0.2.9/GeneralAgent/skills/text_is_english.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/text_translation.py` & `generalagent-0.2.9/GeneralAgent/skills/text_translation.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/token_count.py` & `generalagent-0.2.9/GeneralAgent/skills/token_count.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/unique_name.py` & `generalagent-0.2.9/GeneralAgent/skills/unique_name.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/web_tools.py` & `generalagent-0.2.9/GeneralAgent/skills/web_tools.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/skills/web_tools_advance.py` & `generalagent-0.2.9/GeneralAgent/skills/web_tools_advance.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/GeneralAgent/utils.py` & `generalagent-0.2.9/GeneralAgent/utils.py`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/LICENSE` & `generalagent-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/README.md` & `generalagent-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `generalagent-0.2.8/pyproject.toml` & `generalagent-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "GeneralAgent"
-version = "0.2.8"
+version = "0.2.9"
 description = "General Agent: From LLM to Agent"
 authors = ["Chen Li <lichenarthurdata@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/CosmosShadow/GeneralAgent"
 packages = [
     { include = "GeneralAgent" },
```

### Comparing `generalagent-0.2.8/PKG-INFO` & `generalagent-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeneralAgent
-Version: 0.2.8
+Version: 0.2.9
 Summary: General Agent: From LLM to Agent
 Home-page: https://github.com/CosmosShadow/GeneralAgent
 License: Apache 2.0
 Author: Chen Li
 Author-email: lichenarthurdata@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

