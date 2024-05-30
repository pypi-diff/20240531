# Comparing `tmp/lmnt-1.1.2.tar.gz` & `tmp/lmnt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmnt-1.1.2.tar", last modified: Fri Feb 16 01:21:06 2024, max compression
+gzip compressed data, was "lmnt-1.1.3.tar", last modified: Thu May 30 22:53:12 2024, max compression
```

## Comparing `lmnt-1.1.2.tar` & `lmnt-1.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.553201 lmnt-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.549201 lmnt-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.549201 lmnt-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-16 01:20:58.000000 lmnt-1.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-16 01:20:58.000000 lmnt-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-16 01:20:58.000000 lmnt-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-16 01:20:58.000000 lmnt-1.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-02-16 01:20:58.000000 lmnt-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-02-16 01:21:06.553201 lmnt-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-02-16 01:20:58.000000 lmnt-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.553201 lmnt-1.1.2/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-16 01:20:58.000000 lmnt-1.1.2/demo/.env.example
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-16 01:20:58.000000 lmnt-1.1.2/demo/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-16 01:20:58.000000 lmnt-1.1.2/demo/create_voice.py
--rw-r--r--   0 runner    (1001) docker     (127)   131937 2024-02-16 01:20:58.000000 lmnt-1.1.2/demo/sample-audio-input.mp3
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-02-16 01:20:58.000000 lmnt-1.1.2/demo/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-16 01:20:58.000000 lmnt-1.1.2/demo/synthesize.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-16 01:20:58.000000 lmnt-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 01:21:06.553201 lmnt-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-16 01:20:58.000000 lmnt-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.549201 lmnt-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.553201 lmnt-1.1.2/src/lmnt/
--rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-02-16 01:20:58.000000 lmnt-1.1.2/src/lmnt/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.553201 lmnt-1.1.2/src/lmnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-02-16 01:21:06.000000 lmnt-1.1.2/src/lmnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-16 01:21:06.000000 lmnt-1.1.2/src/lmnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 01:21:06.000000 lmnt-1.1.2/src/lmnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-16 01:21:06.000000 lmnt-1.1.2/src/lmnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-16 01:21:06.000000 lmnt-1.1.2/src/lmnt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.553201 lmnt-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-16 01:20:58.000000 lmnt-1.1.2/test/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    42044 2024-02-16 01:20:58.000000 lmnt-1.1.2/test/filename.wav
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.553201 lmnt-1.1.2/test/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-02-16 01:20:58.000000 lmnt-1.1.2/test/integration/smoke_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 01:21:06.553201 lmnt-1.1.2/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-02-16 01:20:58.000000 lmnt-1.1.2/test/unit/test_speech.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-02-16 01:20:58.000000 lmnt-1.1.2/test/unit/test_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.486051 lmnt-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.482051 lmnt-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.482051 lmnt-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 22:53:08.000000 lmnt-1.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 22:53:08.000000 lmnt-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 22:53:08.000000 lmnt-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-30 22:53:08.000000 lmnt-1.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-30 22:53:08.000000 lmnt-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-30 22:53:12.486051 lmnt-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-30 22:53:08.000000 lmnt-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.486051 lmnt-1.1.3/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 22:53:08.000000 lmnt-1.1.3/demo/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 22:53:08.000000 lmnt-1.1.3/demo/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 22:53:08.000000 lmnt-1.1.3/demo/create_voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131937 2024-05-30 22:53:08.000000 lmnt-1.1.3/demo/sample-audio-input.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-30 22:53:08.000000 lmnt-1.1.3/demo/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-30 22:53:08.000000 lmnt-1.1.3/demo/synthesize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 22:53:08.000000 lmnt-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:53:12.486051 lmnt-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 22:53:08.000000 lmnt-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.482051 lmnt-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.486051 lmnt-1.1.3/src/lmnt/
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-05-30 22:53:08.000000 lmnt-1.1.3/src/lmnt/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.486051 lmnt-1.1.3/src/lmnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-30 22:53:12.000000 lmnt-1.1.3/src/lmnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-30 22:53:12.000000 lmnt-1.1.3/src/lmnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:53:12.000000 lmnt-1.1.3/src/lmnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 22:53:12.000000 lmnt-1.1.3/src/lmnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 22:53:12.000000 lmnt-1.1.3/src/lmnt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.486051 lmnt-1.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 22:53:08.000000 lmnt-1.1.3/test/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    42044 2024-05-30 22:53:08.000000 lmnt-1.1.3/test/filename.wav
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.486051 lmnt-1.1.3/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-05-30 22:53:08.000000 lmnt-1.1.3/test/integration/smoke_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:53:12.486051 lmnt-1.1.3/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-30 22:53:08.000000 lmnt-1.1.3/test/unit/test_speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-30 22:53:08.000000 lmnt-1.1.3/test/unit/test_voice.py
```

### Comparing `lmnt-1.1.2/.github/workflows/publish.yml` & `lmnt-1.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/CHANGELOG.md` & `lmnt-1.1.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/LICENSE` & `lmnt-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/PKG-INFO` & `lmnt-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmnt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python client library for the LMNT API
 Home-page: https://github.com/lmnt-com/lmnt-python
 Author: LMNT, Inc.
 Author-email: feedback@lmnt.com
 License: Apache 2.0
 Keywords: speech tts ai ml genai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lmnt-1.1.2/README.md` & `lmnt-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/demo/create_voice.py` & `lmnt-1.1.3/demo/create_voice.py`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/demo/sample-audio-input.mp3` & `lmnt-1.1.3/demo/sample-audio-input.mp3`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/demo/stream.py` & `lmnt-1.1.3/demo/stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,21 +34,22 @@
     print(content, end='', flush=True)
 
   await conn.finish()
 
 
 async def main(args):
   speech = Speech(os.getenv('LMNT_API_KEY'))
-  conn = await speech.synthesize_streaming(VOICE_ID, return_extras=False)
+  conn = await speech.synthesize_streaming(VOICE_ID, return_extras=False, language=args.language)
 
   t1 = asyncio.create_task(reader_task(conn))
   t2 = asyncio.create_task(writer_task(conn, args.prompt))
 
   await t1
   await t2
   await speech.close()
 
 
 if __name__ == '__main__':
   parser = ArgumentParser()
   parser.add_argument('prompt', default=DEFAULT_PROMPT, nargs='?')
+  parser.add_argument('-l', '--language', required=False, default='en', help='Language code')
   asyncio.run(main(parser.parse_args()))
```

### Comparing `lmnt-1.1.2/demo/synthesize.py` & `lmnt-1.1.3/demo/synthesize.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     print(voices)
 
     # Get your account information.
     account = await s.account_info()
     print(account)
 
     # Synthesize text to speech.
-    synthesize = await s.synthesize(text=args.text, voice=args.voice)
+    synthesize = await s.synthesize(text=args.text, voice=args.voice, language=args.language)
     with open('output.mp3', 'wb') as f:
       f.write(synthesize['audio'])
     print('Done.')
 
 if __name__ == '__main__':
   parser = argparse.ArgumentParser(description='Synthesize text to speech using LMNT API')
   parser.add_argument('-t', '--text', required=False, default='This is a test of the LMNT API.', help='Text to synthesize')
   parser.add_argument('-v', '--voice', required=False, default='lily', help='Voice to use')
+  parser.add_argument('-l', '--language', required=False, default='en', help='Language code')
   args = parser.parse_args()
   asyncio.run(main(args))
```

### Comparing `lmnt-1.1.2/pyproject.toml` & `lmnt-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/setup.py` & `lmnt-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/src/lmnt/api.py` & `lmnt-1.1.3/src/lmnt/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -311,17 +311,19 @@
     Parameters:
     - `text` (str): The text to synthesize.
     - `voice` (str): The voice id to use for synthesis.
 
     Optional parameters:
     - `seed` (int): The seed used to specify a different take. Defaults to random.
     - `format` (str): The audio format to use for synthesis. Defaults to `mp3`.
+    - `sample_rate` (int): 8000, 16000, or 24000 – the desired output sample rate. Defaults to 24000 for all formats except `mulaw` which defaults to 8000.
     - `speed` (float): Floating point value between 0.25 (slow) and 2.0 (fast); Defaults to 1.0
     - `return_durations` (bool): If `True`, the response will include word durations detail. Defaults to `False`.
     - `return_seed` (bool): If `True`, the response will include the seed used for synthesis. Defaults to `False`.
+    - `language` (str): The desired language of the synthesized speech. Two letter ISO 639-1 code. Defaults to `en`.
     - `length` (int): The desired target length of the output speech in seconds. Maximum 300.0 (5 minutes)
 
     Deprecated parameters:
     - `durations` (bool): If `True`, the response will include word durations detail. Defaults to `False`. Deprecated in favor of `return_durations`.
 
     Returns an object with the following keys:
     - `audio`: The binary audio file.
@@ -347,23 +349,26 @@
     if 'seed' in kwargs:
       form_data.add_field('seed', kwargs.get('seed'))
     form_data.add_field('format', kwargs.get('format', 'mp3'))
     form_data.add_field('speed', kwargs.get('speed', 1.0))
     length = kwargs.get('length', None)
     if length is not None:
       form_data.add_field('length', length)
+    if 'sample_rate' in kwargs:
+      form_data.add_field('sample_rate', kwargs.get('sample_rate'))
     if 'quality' in kwargs:
       form_data.add_field('quality', kwargs.get('quality'))
     return_durations = kwargs.get('durations', False)
     if 'return_durations' in kwargs:  # return_durations takes precedence over durations
       return_durations = kwargs['return_durations']
     if return_durations is True:
       form_data.add_field('return_durations', 'true')
     return_seed = kwargs.get('return_seed', False)
-
+    if 'language' in kwargs:
+      form_data.add_field('language', kwargs.get('language'))
     async with self._session.post(url, data=form_data, headers=self._build_headers()) as resp:
       await self._handle_response_errors(resp, 'Speech.synthesize')
       response_data = await resp.json()
       synthesis_result = {}
       synthesis_result['audio'] = base64.b64decode(response_data['audio'])
       if return_durations:
         synthesis_result['durations'] = response_data['durations']
@@ -377,14 +382,15 @@
 
     Parameters:
     - `format` (str): `mp3`, `raw`, or `ulaw` – the desired output format. Defaults to `mp3`.
     - `sample_rate` (int): 8000, 16000, or 24000 – the desired output sample rate. Defaults to 24000.
     - `voice` (str): The voice id to use for this connection.
     - `speed` (float): The speed to use for synthesis. Defaults to 1.0.
     - `return_extras` (bool): If `True`, the response will include word durations detail. Defaults to `False`.
+    - `language` (str): The desired language of the synthesized speech. Two letter ISO 639-1 code. Defaults to `en`.
 
     Returns:
     - `StreamingSynthesisConnection`: The streaming connection object.
     """
     if not voice:
       raise ValueError('[Speech.synthesize_streaming] `voice` must not be None.')
 
@@ -399,14 +405,16 @@
     if 'sample_rate' in kwargs:
       init_msg['sample_rate'] = kwargs['sample_rate']
     if 'speed' in kwargs:
       init_msg['speed'] = kwargs['speed']
     if 'expressive' in kwargs:
       init_msg['expressive'] = kwargs['expressive']
     init_msg['send_extras'] = return_extras
+    if 'language' in kwargs:
+      init_msg['language'] = kwargs['language']
     ws = await self._session.ws_connect(f'{self._base_url}{_SYNTHESIZE_STREAMING_ENDPOINT}')
     await ws.send_str(json.dumps(init_msg))
     return StreamingSynthesisConnection(ws, return_extras)
 
   async def account_info(self):
     """
     Returns details about your account.
```

### Comparing `lmnt-1.1.2/src/lmnt.egg-info/PKG-INFO` & `lmnt-1.1.3/src/lmnt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmnt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python client library for the LMNT API
 Home-page: https://github.com/lmnt-com/lmnt-python
 Author: LMNT, Inc.
 Author-email: feedback@lmnt.com
 License: Apache 2.0
 Keywords: speech tts ai ml genai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lmnt-1.1.2/src/lmnt.egg-info/SOURCES.txt` & `lmnt-1.1.3/src/lmnt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/test/filename.wav` & `lmnt-1.1.3/test/filename.wav`

 * *Files identical despite different names*

### Comparing `lmnt-1.1.2/test/integration/smoke_test.py` & `lmnt-1.1.3/test/integration/smoke_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,28 @@
   assert 'durations' not in result
   assert 'seed' not in result
   assert len(result['audio']) > 0
   assert isinstance(result['audio'], bytes)
 
 
 @pytest.mark.asyncio
+async def test_synthesize__non_en_language(api: Speech):
+  voice = 'lily'
+  text = 'Example Text'
+  language = 'pt'
+  result = await api.synthesize(text=text, voice=voice, language=language)
+  assert result is not None
+  assert 'audio' in result
+  assert 'durations' not in result
+  assert 'seed' not in result
+  assert len(result['audio']) > 0
+  assert isinstance(result['audio'], bytes)
+
+
+@pytest.mark.asyncio
 async def test_synthesize_with_empty_voice(api: Speech):
   voice = ''
   text = 'Example Text'
   with pytest.raises(Exception):
     await api.synthesize(text=text, voice=voice)
```

### Comparing `lmnt-1.1.2/test/unit/test_speech.py` & `lmnt-1.1.3/test/unit/test_speech.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,27 @@
   api._session.post.return_value.__aenter__.return_value.status = 200
 
   synthesis_result = await api.synthesize(text, voice, return_durations=True, return_seed=True)
   assert synthesis_result == {'audio': base64.b64decode(mock_response['audio']), 'durations': mock_response['durations'], 'seed': mock_response['seed']}
 
 
 @pytest.mark.asyncio
+async def test_synthesize__non_en_language(api):
+  text = 'Hello, world!'
+  voice = 'Voice1'
+  language = 'pt'
+  mock_response = {'audio': MOCK_AUDIO, 'durations': [], 'seed': 'random_seed'}
+  api._session.post.return_value.__aenter__.return_value.json = AsyncMock(return_value=mock_response)
+  api._session.post.return_value.__aenter__.return_value.status = 200
+
+  synthesis_result = await api.synthesize(text, voice, language=language)
+  assert synthesis_result == {'audio': base64.b64decode(mock_response['audio'])}
+
+
+@pytest.mark.asyncio
 async def test_synthesize_no_text(api):
   with pytest.raises(AssertionError):
     await api.synthesize(None, 'Voice1')
 
 
 @pytest.mark.asyncio
 async def test_synthesize_no_voice(api):
@@ -109,29 +122,31 @@
 
 @pytest.mark.asyncio
 async def test_synthesize_streaming(api):
   voice = 'Voice1'
   speed = 1.5
   expressive = 0.8
   return_extras = True
+  language = 'pt'
 
   mock_ws = AsyncMock()
   api._session = AsyncMock()
   api._session.ws_connect.return_value = mock_ws
 
-  connection = await api.synthesize_streaming(voice, return_extras=return_extras, speed=speed, expressive=expressive)
+  connection = await api.synthesize_streaming(voice, return_extras=return_extras, speed=speed, expressive=expressive, language=language)
 
   assert isinstance(connection, StreamingSynthesisConnection)
   api._session.ws_connect.assert_called_once_with(f'{api._base_url}{_SYNTHESIZE_STREAMING_ENDPOINT}')
   mock_ws.send_str.assert_called_once_with(json.dumps({
       'X-API-Key': api._api_key,
       'voice': voice,
       'speed': speed,
       'expressive': expressive,
-      'send_extras': return_extras
+      'send_extras': return_extras,
+      'language': language
   }))
 
 
 @pytest.mark.asyncio
 async def test_synthesize_streaming_defaults(api):
   voice = 'Voice1'
```

### Comparing `lmnt-1.1.2/test/unit/test_voice.py` & `lmnt-1.1.3/test/unit/test_voice.py`

 * *Files identical despite different names*

