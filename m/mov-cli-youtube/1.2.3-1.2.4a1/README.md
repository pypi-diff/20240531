# Comparing `tmp/mov_cli_youtube-1.2.3.tar.gz` & `tmp/mov_cli_youtube-1.2.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_youtube-1.2.3.tar", last modified: Fri May 17 13:42:44 2024, max compression
+gzip compressed data, was "mov_cli_youtube-1.2.4a1.tar", last modified: Fri May 31 19:07:34 2024, max compression
```

## Comparing `mov_cli_youtube-1.2.3.tar` & `mov_cli_youtube-1.2.4a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/LICENSE
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2930 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      613 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/README.md
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/mov_cli_youtube/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      650 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/mov_cli_youtube/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2731 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/mov_cli_youtube/pytube.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4203 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/mov_cli_youtube/yt_dlp.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2930 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      306 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)      100 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)       16 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1298 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/pyproject.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-31 19:07:34.151444 mov_cli_youtube-1.2.4a1/
+-rwxr-xr-x   0 ananas    (1000) ananas    (1000)     1085 2024-05-28 22:29:40.000000 mov_cli_youtube-1.2.4a1/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2960 2024-05-31 19:07:34.151444 mov_cli_youtube-1.2.4a1/PKG-INFO
+-rwxr-xr-x   0 ananas    (1000) ananas    (1000)      647 2024-05-28 22:29:40.000000 mov_cli_youtube-1.2.4a1/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-31 19:07:34.151444 mov_cli_youtube-1.2.4a1/mov_cli_youtube/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      652 2024-05-31 19:07:26.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3170 2024-05-31 19:07:26.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube/pytube.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4714 2024-05-31 17:26:04.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube/yt_dlp.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-31 19:07:34.151444 mov_cli_youtube-1.2.4a1/mov_cli_youtube.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2960 2024-05-31 19:07:34.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube.egg-info/PKG-INFO
+-rwxr-xr-x   0 ananas    (1000) ananas    (1000)      306 2024-05-31 19:07:34.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ananas    (1000) ananas    (1000)        1 2024-05-31 19:07:34.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ananas    (1000) ananas    (1000)      100 2024-05-31 19:07:34.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube.egg-info/requires.txt
+-rwxr-xr-x   0 ananas    (1000) ananas    (1000)       16 2024-05-31 19:07:34.000000 mov_cli_youtube-1.2.4a1/mov_cli_youtube.egg-info/top_level.txt
+-rwxr-xr-x   0 ananas    (1000) ananas    (1000)     1401 2024-05-31 07:53:09.000000 mov_cli_youtube-1.2.4a1/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-31 19:07:34.151444 mov_cli_youtube-1.2.4a1/setup.cfg
```

### Comparing `mov_cli_youtube-1.2.3/PKG-INFO` & `mov_cli_youtube-1.2.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.3
+Version: 1.2.4a1
 Summary: A mov-cli v4 plugin for watching youtube.
-Author-email: Goldy <goldy@devgoldy.xyz>
+Author-email: Goldy <goldy@devgoldy.xyz>, Ananas <ananas@ananas.moe>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mov_cli_youtube-1.2.3/README.md` & `mov_cli_youtube-1.2.4a1/README.md`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-<div align="center">
-
-  # mov-cli-youtube
-  <sub>A mov-cli v4 plugin for watching youtube.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
-
-</div>
-
-## Installation 🛠️
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-youtube
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-youtube = "mov-cli-youtube"
-```
-
-## Usage 🖱️
-```sh
-mov-cli -s youtube nyan cat
-```
-
-### Audio Only 🔉
-```sh
-mov-cli -s youtube nyan cat -- --audio
-```
+<div align="center">
+
+  # mov-cli-youtube
+  <sub>A mov-cli v4 plugin for watching youtube.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
+
+</div>
+
+## Installation 🛠️
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-youtube
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+youtube = "mov-cli-youtube"
+```
+
+## Usage 🖱️
+```sh
+mov-cli -s youtube nyan cat
+```
+
+### Audio Only 🔉
+```sh
+mov-cli -s youtube nyan cat -- --audio
+```
```

### Comparing `mov_cli_youtube-1.2.3/mov_cli_youtube/__init__.py` & `mov_cli_youtube-1.2.4a1/mov_cli_youtube/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         "IOS.DEFAULT": PyTubeScraper, 
 
         "yt-dlp": YTDlpScraper, 
         "pytube": PyTubeScraper, 
     }
 }
 
-__version__ = "1.2.3"
+__version__ = "1.2.4a1"
```

### Comparing `mov_cli_youtube-1.2.3/mov_cli_youtube/pytube.py` & `mov_cli_youtube-1.2.4a1/mov_cli_youtube/pytube.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import List, Optional, Dict, Generator, Any
+    from typing import List, Optional, Generator, Any
 
     from mov_cli import Config
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
 import os
 import sys
 from pytubefix import YouTube, Search
 
 from mov_cli.scraper import Scraper
 from mov_cli.utils import EpisodeSelector
 from mov_cli import Single, Metadata, MetadataType, ExtraMetadata
 
+from mov_cli.media import Quality
+from mov_cli.utils import get_temp_directory, what_platform
+
 __all__ = ("PyTubeScraper",)
 
 class PyTubeScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         super().__init__(config, http_client, options)
 
-    def search(self, query: str, limit: int = None) -> Generator[Metadata, Any, None]:
+    def search(self, query: str, limit: Optional[int] = None) -> Generator[Metadata, Any, None]:
         search_query = Search(query)
         search_results: List[YouTube] = search_query.videos
 
         max_videos = 20 if limit is None else limit
 
         # suppress pytube's stupid errors from getting to the console and ruining fzf output.
         sys.stderr = open(os.devnull, "w")
@@ -34,48 +37,59 @@
         for index, video in enumerate(search_results):
             if (index + 1) == len(search_results) and not (index + 1) >= max_videos:
                 search_query.get_next_results()
 
             yield Metadata(
                 id = video.watch_url, 
                 title = f"{video.title} ~ {video.author}", 
-                type = MetadataType.MOVIE, 
+                type = MetadataType.SINGLE, 
                 year = str(video.publish_date.year),
                 extra_func = lambda: self.__scrape_extra(video)
             )
 
         # restore the console.
         sys.stderr = sys.__stderr__
 
     def scrape(self, metadata: Metadata, _: EpisodeSelector) -> Single:
         audio_only: bool = self.options.get("audio", False)
+        subtitle = None
 
         watch_url = metadata.id
         video = YouTube(watch_url)
 
         if audio_only:
             url = video.streams.get_audio_only().url
 
-        elif self.config.resolution is not None:
-            url = video.streams.get_by_resolution(f"{self.config.resolution}p").url
+        elif not self.config.resolution == Quality.AUTO:
+            url = video.streams.get_by_resolution(self.config.resolution.apply_p()).url
 
             if url is None:
                 url = video.streams.get_highest_resolution().url
 
         else:
             url = video.streams.get_highest_resolution().url
+    
+        for caption in video.captions:
+            if caption.code.startswith(self.config.language.iso639_1):
+                platform = what_platform()
+
+                temp = get_temp_directory(platform).joinpath(video.video_id)
+
+                with temp.open("w", encoding = "utf-8") as f:
+                    f.write(
+                        caption.generate_srt_captions()
+                    )
+                
+                subtitle = temp
 
         return Single(
             url = url, 
             title = metadata.title, 
-            year = metadata.year
+            year = metadata.year,
+            subtitles = subtitle
         )
 
-    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[None, int]:
-        # Returning None as search does not return any metadata of type series.
-        return {None: 1}
-
     def __scrape_extra(self, key: YouTube) -> ExtraMetadata:
         return ExtraMetadata(
             description = key.description,
             image_url = key.thumbnail_url,
         )
```

### Comparing `mov_cli_youtube-1.2.3/mov_cli_youtube/yt_dlp.py` & `mov_cli_youtube-1.2.4a1/mov_cli_youtube/yt_dlp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Optional, Dict, Generator, Any, List, Tuple
+    from typing import Optional, Generator, Any, List, Tuple
 
     from mov_cli import Config
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
 import yt_dlp
 
@@ -48,14 +48,15 @@
                 )
 
     def scrape(
         self, 
         metadata: Metadata, 
         _: EpisodeSelector
     ) -> Single:
+        subtitle = None
 
         watch_url = metadata.id
 
         yt_options = {
             "format": "best", 
             "nocheckcertificate": True, 
             "geo_bypass": True, 
@@ -69,25 +70,34 @@
 
             if self.options.get("audio", False):
                 url = self.__get_best_stream(info, audio = True)
             else:
                 url = self.__get_best_stream(info, video = True)
                 audio_url = self.__get_best_stream(info, audio = True)
 
+            for lang_code, caption_data in info.get("automatic_captions", {}).items():
+                if lang_code == self.config.language.iso639_1:
+                    for caption in caption_data:
+                        if caption.get("ext") == "vtt":
+                            subtitle = caption.get("url")
+
+            for lang_code, caption_data in info.get("subtitles", {}).items():
+                if lang_code.startswith(self.config.language.iso639_1):
+                    for caption in caption_data:
+                        if caption.get("ext") == "vtt":
+                            subtitle = caption.get("url")
+
         return Single(
             url = url, 
             audio_url = audio_url, 
             title = metadata.title, 
-            year = metadata.year
+            year = metadata.year,
+            subtitles = subtitle
         )
 
-    def scrape_episodes(self, _: Metadata) -> Dict[None, int]:
-        # Returning None as search does not return any metadata of type series.
-        return {None: 1}
-
     def __get_best_stream(self, ytdlp_info: dict, video: bool = False, audio: bool = False) -> str:
         """Returns the best stream respecting the parameters given."""
         stream_formats_to_sort: List[Tuple[int, str]] = []
 
         for stream_format in ytdlp_info["formats"]:
 
             if video is True and stream_format["video_ext"] == "none":
```

### Comparing `mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/PKG-INFO` & `mov_cli_youtube-1.2.4a1/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.3
+Version: 1.2.4a1
 Summary: A mov-cli v4 plugin for watching youtube.
-Author-email: Goldy <goldy@devgoldy.xyz>
+Author-email: Goldy <goldy@devgoldy.xyz>, Ananas <ananas@ananas.moe>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mov_cli_youtube-1.2.3/pyproject.toml` & `mov_cli_youtube-1.2.4a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-[project]
-name = "mov-cli-youtube"
-description = "A mov-cli v4 plugin for watching youtube."
-authors = [
-    {name = "Goldy", email = "goldy@devgoldy.xyz"}
-]
-readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.8"
-license = { file = "LICENSE" }
-keywords = [
-    "amazing mov-cli plugin"
-]
-classifiers = [
-	'Operating System :: Microsoft :: Windows :: Windows 11',
-    'Operating System :: Microsoft :: Windows :: Windows 10',
-    'Operating System :: POSIX :: Linux',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-	'Programming Language :: Python :: 3.11'
-]
-dependencies = [
-    "requests",
-    "importlib-metadata; python_version<'3.8'",
-
-    "pytubefix",
-    "yt-dlp>=2024.4.9"
-]
-
-dynamic = ["version"]
-
-[project.optional-dependencies]
-dev = [
-    "ruff",
-    "build"
-]
-
-[project.urls]
-GitHub = "https://github.com/mov-cli/mov-cli-youtube"
-BugTracker = "https://github.com/mov-cli/mov-cli-youtube/issues"
-
-[tool.setuptools.dynamic]
-version = { attr = "mov_cli_youtube.__version__" }
-
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
+[project]
+name = "mov-cli-youtube"
+description = "A mov-cli v4 plugin for watching youtube."
+authors = [
+    {name = "Goldy", email = "goldy@devgoldy.xyz"},
+    {name = "Ananas", email = "ananas@ananas.moe"}
+]
+readme = {file = "README.md", content-type = "text/markdown"}
+requires-python = ">=3.8"
+license = { file = "LICENSE" }
+keywords = [
+    "amazing mov-cli plugin"
+]
+classifiers = [
+	'Operating System :: Microsoft :: Windows :: Windows 11',
+    'Operating System :: Microsoft :: Windows :: Windows 10',
+    'Operating System :: POSIX :: Linux',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+	'Programming Language :: Python :: 3.11'
+]
+dependencies = [
+    "requests",
+    "importlib-metadata; python_version<'3.8'",
+
+    "pytubefix",
+    "yt-dlp>=2024.4.9"
+]
+
+dynamic = ["version"]
+
+[project.optional-dependencies]
+dev = [
+    "ruff",
+    "build"
+]
+
+[project.urls]
+GitHub = "https://github.com/mov-cli/mov-cli-youtube"
+BugTracker = "https://github.com/mov-cli/mov-cli-youtube/issues"
+
+[tool.setuptools.dynamic]
+version = { attr = "mov_cli_youtube.__version__" }
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
 include = ["mov_cli_youtube*"]
```

