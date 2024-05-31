# Comparing `tmp/llama_summarizer-0.1.tar.gz` & `tmp/llama_summarizer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_summarizer-0.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "llama_summarizer-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `llama_summarizer-0.1.tar` & `llama_summarizer-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     3524 2022-11-09 12:37:21.000000 llama_summarizer-0.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 llama_summarizer-0.1/.gitignore
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 llama_summarizer-0.1/CMakeLists.txt
--rw-r--r--   0        0        0    11358 2022-11-09 12:37:21.000000 llama_summarizer-0.1/LICENSE
--rw-r--r--   0        0        0      729 2022-11-09 12:37:21.000000 llama_summarizer-0.1/README.md
--rw-r--r--   0        0        0      452 2022-11-09 12:37:21.000000 llama_summarizer-0.1/ci/linux-aarch64/Dockerfile
--rw-r--r--   0        0        0      450 2022-11-09 12:37:21.000000 llama_summarizer-0.1/ci/linux-x86_64/Dockerfile
--rw-r--r--   0        0        0      739 2022-11-09 12:37:21.000000 llama_summarizer-0.1/ci/osx-deps.sh
--rwxr-xr-x   0        0        0      465 2022-11-09 12:37:21.000000 llama_summarizer-0.1/ext-installer/install.sh
--rwxr-xr-x   0        0        0       86 2022-11-09 12:37:21.000000 llama_summarizer-0.1/ext-installer/launcher.sh
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 llama_summarizer-0.1/ext-installer/summarize.json
--rw-r--r--   0        0        0     1103 2022-11-09 12:37:21.000000 llama_summarizer-0.1/extension/background.js
--rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 llama_summarizer-0.1/extension/load.js
--rw-r--r--   0        0        0      708 2022-11-09 12:37:21.000000 llama_summarizer-0.1/extension/manifest.json
--rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 llama_summarizer-0.1/extension/progress.html
--rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 llama_summarizer-0.1/extension/progress.js
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 llama_summarizer-0.1/extension/summary.html
--rw-r--r--   0        0        0      598 2022-11-09 12:37:21.000000 llama_summarizer-0.1/pyproject.toml
--rw-r--r--   0        0        0      158 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/__init__.py
--rw-r--r--   0        0        0     9643 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/audio_decode.c
--rw-r--r--   0        0        0     3667 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/chatgpt.py
--rw-r--r--   0        0        0     3813 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/cli.py
--rw-r--r--   0        0        0     2375 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/extension.py
--rw-r--r--   0        0        0     2299 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/huggingchat.py
--rw-r--r--   0        0        0    13184 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/summarizer.py
--rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 llama_summarizer-0.1/summarizer/template.html
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 llama_summarizer-0.1/PKG-INFO
+-rw-r--r--   0        0        0     3524 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0    11358 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/LICENSE
+-rw-r--r--   0        0        0      729 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/README.md
+-rw-r--r--   0        0        0      452 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/ci/linux-aarch64/Dockerfile
+-rw-r--r--   0        0        0      450 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/ci/linux-x86_64/Dockerfile
+-rw-r--r--   0        0        0      739 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/ci/osx-deps.sh
+-rwxr-xr-x   0        0        0     1239 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/ext-installer/install.py
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/ext-installer/summarize.json
+-rw-r--r--   0        0        0     1103 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/extension/background.js
+-rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/extension/load.js
+-rw-r--r--   0        0        0      708 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/extension/manifest.json
+-rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/extension/progress.html
+-rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/extension/progress.js
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/extension/summary.html
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      158 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/__init__.py
+-rw-r--r--   0        0        0     9693 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/audio_decode.c
+-rw-r--r--   0        0        0     3667 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/chatgpt.py
+-rw-r--r--   0        0        0     3830 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/cli.py
+-rw-r--r--   0        0        0     2392 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/extension.py
+-rw-r--r--   0        0        0     2299 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/huggingchat.py
+-rw-r--r--   0        0        0    13184 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/summarizer.py
+-rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/summarizer/template.html
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 llama_summarizer-0.1.1/PKG-INFO
```

### Comparing `llama_summarizer-0.1/.github/workflows/wheels.yml` & `llama_summarizer-0.1.1/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/CMakeLists.txt` & `llama_summarizer-0.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/LICENSE` & `llama_summarizer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/README.md` & `llama_summarizer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/ci/osx-deps.sh` & `llama_summarizer-0.1.1/ci/osx-deps.sh`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/extension/background.js` & `llama_summarizer-0.1.1/extension/background.js`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/extension/manifest.json` & `llama_summarizer-0.1.1/extension/manifest.json`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/extension/progress.html` & `llama_summarizer-0.1.1/extension/progress.html`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/extension/progress.js` & `llama_summarizer-0.1.1/extension/progress.js`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/pyproject.toml` & `llama_summarizer-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core[pyproject]>=0.5.1"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "llama-summarizer"
-version = "0.1"
+version = "0.1.1"
 requires-python = ">=3.11"
 dependencies = [
   "Jinja2>=3.1.3",
   "llama_cpp_python>=0.2.64",
   "requests>=2.31.0",
   "yt-dlp>=2024.4.9",
   "huggingface_hub>=0.22.1",
```

### Comparing `llama_summarizer-0.1/summarizer/audio_decode.c` & `llama_summarizer-0.1.1/summarizer/audio_decode.c`

 * *Files 3% similar despite different names*

```diff
@@ -197,26 +197,27 @@
     }
     err = avformat_find_stream_info(fmt_ctx, NULL);
     if (err < 0) {
         str_err = format_error("getting stream info", err);
         goto out_close_input;
     }
 
-    if (fmt_ctx->nb_streams != 1) {
-        asprintf(&str_err, "invalid number of streams: %d", fmt_ctx->nb_streams);
-        goto out_close_input;
+    int stream_id = -1;
+    for (int i = 0; i < fmt_ctx->nb_streams; i++) {
+        if (fmt_ctx->streams[i]->codecpar->codec_type == AVMEDIA_TYPE_AUDIO) {
+            stream_id = i;
+            break;
+        }
     }
-
-    AVCodecParameters *codec_params = fmt_ctx->streams[0]->codecpar;
-    enum AVMediaType codec_type = codec_params->codec_type;
-    if (codec_type != AVMEDIA_TYPE_AUDIO) {
-        asprintf(&str_err, "invalid stream type: %s", av_get_media_type_string(codec_type));
+    if (stream_id == -1) {
+        str_err = strdup("Unable to find the audio stream");
         goto out_close_input;
     }
 
+    AVCodecParameters *codec_params = fmt_ctx->streams[stream_id]->codecpar;
     AVCodec *decoder = avcodec_find_decoder(codec_params->codec_id);
     if (!decoder) {
         asprintf(&str_err, "can't find decoder for codec: %s", avcodec_get_name(codec_params->codec_id));
         goto out_close_input;
     }
     AVCodecContext *dec_ctx = avcodec_alloc_context3(decoder);
     err = avcodec_parameters_to_context(dec_ctx, codec_params);
@@ -226,15 +227,15 @@
     }
     err = avcodec_open2(dec_ctx, decoder, NULL);
     if (err < 0) {
         str_err = format_error("opening decoder", err);
         goto out_free_dec_ctx;
     }
     char *graph_err;
-    struct filter filter = create_filter_graph(fmt_ctx->streams[0]->time_base, dec_ctx, &graph_err);
+    struct filter filter = create_filter_graph(fmt_ctx->streams[stream_id]->time_base, dec_ctx, &graph_err);
     if (graph_err != NULL) {
         asprintf(&str_err, "creating filter graph: %s", graph_err);
         free(graph_err);
         goto out_free_dec_ctx;
     }
 
     AVPacket *packet = av_packet_alloc();
@@ -242,14 +243,17 @@
     AVFrame *filt_frame = av_frame_alloc();
     struct buffer buffer = {
         .data = malloc(block_size * sizeof(float)),
         .ptr = 0,
         .size = block_size
     };
     while ((err = av_read_frame(fmt_ctx, packet)) == 0) {
+        if (packet->stream_index != stream_id) {
+            continue;
+        }
         err = avcodec_send_packet(dec_ctx, packet);
         if (err < 0) {
             str_err = format_error("sending packet to decoder", err);
             goto loop_end;
         }
         str_err = receive_and_filter(frame, filt_frame, dec_ctx, &filter, &buffer, callback);
       loop_end:
```

### Comparing `llama_summarizer-0.1/summarizer/chatgpt.py` & `llama_summarizer-0.1.1/summarizer/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/summarizer/cli.py` & `llama_summarizer-0.1.1/summarizer/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     args.openai_api_key = api_key
     kwargs = {k: v for (k, v) in vars(args).items() if v is not None}
     progress = ProgressHooks()
     result = process_video(progress, **kwargs)
     progress.close()
     filename = os.path.join(OUT_DIR, f'{result.video_id}.html')
     os.makedirs(OUT_DIR, exist_ok = True)
-    with open(filename, 'w') as out:
-        out.write(result.summary)
+    with open(filename, 'wb') as out:
+        out.write(result.summary.encode('utf-8'))
     for opener in ['open', 'xdg-open']:
         if shutil.which(opener) is not None:
             os.execlp(opener, opener, filename)
             return
     if shutil.which('cmd') is not None:
         os.execlp('cmd', 'cmd', '/c', filename)
     print(f'Unable to open the file automatically, the output was written to {filename}')
```

### Comparing `llama_summarizer-0.1/summarizer/extension.py` & `llama_summarizer-0.1.1/summarizer/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     api_key = os.environ.get('OPENAI_API_KEY', api_key)
     config['openai_api_key'] = api_key
     result = process_video(
         ProgressHooks(ctx), video_url=msg['url'], **config
     )
     filename = f'{OUT_DIR}/{result.video_id}.html'
     os.makedirs(OUT_DIR, exist_ok = True)
-    with open(filename, 'w') as out:
-        out.write(result.summary)
+    with open(filename, 'wb') as out:
+        out.write(result.summary.encode('utf-8'))
     output({
         'msg': 'complete',
         'id': result.video_id,
         'ctx': ctx
     })
 
 def load(msg):
```

### Comparing `llama_summarizer-0.1/summarizer/huggingchat.py` & `llama_summarizer-0.1.1/summarizer/huggingchat.py`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/summarizer/summarizer.py` & `llama_summarizer-0.1.1/summarizer/summarizer.py`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/summarizer/template.html` & `llama_summarizer-0.1.1/summarizer/template.html`

 * *Files identical despite different names*

### Comparing `llama_summarizer-0.1/PKG-INFO` & `llama_summarizer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-summarizer
-Version: 0.1
+Version: 0.1.1
 Requires-Python: >=3.11
 Requires-Dist: Jinja2>=3.1.3
 Requires-Dist: llama_cpp_python>=0.2.64
 Requires-Dist: requests>=2.31.0
 Requires-Dist: yt-dlp>=2024.4.9
 Requires-Dist: huggingface_hub>=0.22.1
 Requires-Dist: whisper-cpp-python-smr>=0.1
```

