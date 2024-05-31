# Comparing `tmp/nostr_dvm-0.5.1.tar.gz` & `tmp/nostr_dvm-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.5.1.tar", last modified: Thu May 30 19:17:48 2024, max compression
+gzip compressed data, was "nostr_dvm-0.5.2.tar", last modified: Fri May 31 08:28:47 2024, max compression
```

## Comparing `nostr_dvm-0.5.1.tar` & `nostr_dvm-0.5.2.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.830776 nostr_dvm-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-30 19:17:48.830776 nostr_dvm-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.814776 nostr_dvm-0.5.1/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.814776 nostr_dvm-0.5.1/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.814776 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.814776 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.818776 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.818776 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.818776 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.818776 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.818776 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.818776 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.822776 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39789 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.822776 nostr_dvm-0.5.1/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.826776 nostr_dvm-0.5.1/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14080 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.830776 nostr_dvm-0.5.1/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.830776 nostr_dvm-0.5.1/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.830776 nostr_dvm-0.5.1/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-30 19:17:48.000000 nostr_dvm-0.5.1/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-30 19:17:48.000000 nostr_dvm-0.5.1/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:17:48.000000 nostr_dvm-0.5.1/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 19:17:48.000000 nostr_dvm-0.5.1/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 19:17:48.000000 nostr_dvm-0.5.1/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:17:48.830776 nostr_dvm-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:17:48.830776 nostr_dvm-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-30 19:17:44.000000 nostr_dvm-0.5.1/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.202839 nostr_dvm-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-31 08:28:47.202839 nostr_dvm-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.186839 nostr_dvm-0.5.2/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.186839 nostr_dvm-0.5.2/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.186839 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.186839 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.190839 nostr_dvm-0.5.2/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.198839 nostr_dvm-0.5.2/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.202839 nostr_dvm-0.5.2/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.202839 nostr_dvm-0.5.2/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.202839 nostr_dvm-0.5.2/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-31 08:28:47.000000 nostr_dvm-0.5.2/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-31 08:28:47.000000 nostr_dvm-0.5.2/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:28:47.000000 nostr_dvm-0.5.2/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 08:28:47.000000 nostr_dvm-0.5.2/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 08:28:47.000000 nostr_dvm-0.5.2/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:28:47.202839 nostr_dvm-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:28:47.202839 nostr_dvm-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-31 08:28:41.000000 nostr_dvm-0.5.2/tests/test_events.py
```

### Comparing `nostr_dvm-0.5.1/LICENSE` & `nostr_dvm-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/PKG-INFO` & `nostr_dvm-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.1
+Version: 0.5.2
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.1/README.md` & `nostr_dvm-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.5.2/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/bot.py` & `nostr_dvm-0.5.2/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/dvm.py` & `nostr_dvm-0.5.2/nostr_dvm/dvm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from nostr_dvm.utils.mediasource_utils import input_data_file_duration
 from nostr_dvm.utils.nip88_utils import nip88_has_active_subscription
 from nostr_dvm.utils.nostr_utils import get_event_by_id, get_referenced_event_by_id, send_event, check_and_decrypt_tags
 from nostr_dvm.utils.output_utils import build_status_reaction
 from nostr_dvm.utils.zap_utils import check_bolt11_ln_bits_is_paid, create_bolt11_ln_bits, parse_zap_event_tags, \
     parse_amount_from_bolt11_invoice, zaprequest, pay_bolt11_ln_bits, create_bolt11_lud16
 from nostr_dvm.utils.cashu_utils import redeem_cashu
+from nostr_dvm.utils.print import bcolors
 
 
 class DVM:
     dvm_config: DVMConfig
     admin_config: AdminConfig
     keys: Keys
     client: Client
@@ -43,17 +44,18 @@
 
         signer = NostrSigner.keys(self.keys)
         self.client = Client.with_opts(signer, opts)
 
         self.job_list = []
         self.jobs_on_hold_list = []
         pk = self.keys.public_key()
-
-        print("Nostr DVM public key: " + str(pk.to_bech32()) + " Hex: " + str(pk.to_hex()) + " Supported DVM tasks: " +
-              ', '.join(p.NAME + ":" + p.TASK for p in self.dvm_config.SUPPORTED_DVMS) + "\n")
+        print(bcolors.GREEN + "[" + self.dvm_config.NIP89.NAME + "] " + "Nostr DVM public key: " + str(
+            pk.to_bech32()) + " Hex: " +
+              str(pk.to_hex()) + " Supported DVM tasks: " +
+              ', '.join(p.NAME + ":" + p.TASK for p in self.dvm_config.SUPPORTED_DVMS) + bcolors.ENDC)
 
         for relay in self.dvm_config.RELAY_LIST:
             self.client.add_relay(relay)
         self.client.connect()
 
         zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         kinds = [EventDefinitions.KIND_NIP90_GENERIC]
@@ -84,15 +86,15 @@
 
         def handle_nip90_job_event(nip90_event):
             # decrypted encrypted events
             nip90_event = check_and_decrypt_tags(nip90_event, self.dvm_config)
             # if event is encrypted, but we can't decrypt it (e.g. because its directed to someone else), return
             if nip90_event is None:
                 return
-            
+
             task_is_free = False
             user_has_active_subscription = False
             cashu = ""
             p_tag_str = ""
 
             for tag in nip90_event.tags():
                 if tag.as_vec()[0] == "cashu":
@@ -100,64 +102,67 @@
                 elif tag.as_vec()[0] == "p":
                     p_tag_str = tag.as_vec()[1]
 
             if p_tag_str != "" and p_tag_str != self.dvm_config.PUBLIC_KEY:
                 print("[" + self.dvm_config.NIP89.NAME + "] No public request, also not addressed to me.")
                 return
 
-
             # check if task is supported by the current DVM
             task_supported, task = check_task_is_supported(nip90_event, client=self.client,
                                                            config=self.dvm_config)
             # if task is supported, continue, else do nothing.
             if task_supported:
                 # fetch or add user contacting the DVM from/to local database
                 user = get_or_add_user(self.dvm_config.DB, nip90_event.author().to_hex(), client=self.client,
                                        config=self.dvm_config, skip_meta=False)
                 # if user is blacklisted for some reason, send an error reaction and return
                 if user.isblacklisted:
                     send_job_status_reaction(nip90_event, "error", client=self.client, dvm_config=self.dvm_config)
                     print("[" + self.dvm_config.NIP89.NAME + "] Request by blacklisted user, skipped")
                     return
 
-                print("[" + self.dvm_config.NIP89.NAME + "] Received new Request: " + task + " from " + user.name)
+                print(bcolors.MAGENTA + "[" + self.dvm_config.NIP89.NAME + "] Received new Request: " + task + " from " + user.name  + bcolors.ENDC)
                 duration = input_data_file_duration(nip90_event, dvm_config=self.dvm_config, client=self.client)
                 amount = get_amount_per_task(task, self.dvm_config, duration)
                 if amount is None:
                     return
 
-
                 # If this is a subscription DVM and the Task is directed to us, check for active subscription
                 if dvm_config.NIP88 is not None and p_tag_str == self.dvm_config.PUBLIC_KEY:
                     send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
-                                             "Checking Subscription Status, please wait..",self.dvm_config)
+                                             "Checking Subscription Status, please wait..", self.dvm_config)
                     # if we stored in the database that the user has an active subscription, we don't need to check it
                     print("User Subscription: " + str(user.subscribed) + " Current time: " + str(
                         Timestamp.now().as_secs()))
                     # if we have an entry in the db that user is subscribed, continue
                     if int(user.subscribed) > int(Timestamp.now().as_secs()):
                         print("User subscribed until: " + str(Timestamp.from_secs(user.subscribed).to_human_datetime()))
                         user_has_active_subscription = True
                         send_job_status_reaction(nip90_event, "subscription-required", True, amount,
                                                  self.client, "User subscripton active until " +
-                                                 Timestamp.from_secs(int(user.subscribed)).to_human_datetime().replace("Z", " ").replace("T", " ") + " GMT", self.dvm_config)
+                                                 Timestamp.from_secs(int(user.subscribed)).to_human_datetime().replace(
+                                                     "Z", " ").replace("T", " ") + " GMT", self.dvm_config)
                     # otherwise we check for an active subscription by checking recipie events
                     else:
                         print("[" + self.dvm_config.NIP89.NAME + "] Checking Subscription status")
                         send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
                                                  "I Don't have information about subscription status, checking on the Nostr. This might take a few seconds",
                                                  self.dvm_config)
 
                         subscription_status = nip88_has_active_subscription(PublicKey.parse(user.npub),
                                                                             self.dvm_config.NIP88.DTAG, self.client,
                                                                             self.dvm_config.PUBLIC_KEY)
 
                         if subscription_status["isActive"]:
                             send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
-                                                     "User subscripton active until " + Timestamp.from_secs(int(subscription_status["validUntil"])).to_human_datetime().replace("Z", " ").replace("T", " ") + " GMT",
+                                                     "User subscripton active until " + Timestamp.from_secs(int(
+                                                         subscription_status[
+                                                             "validUntil"])).to_human_datetime().replace("Z",
+                                                                                                         " ").replace(
+                                                         "T", " ") + " GMT",
                                                      self.dvm_config)
                             print("Checked Recipe: User subscribed until: " + str(
                                 Timestamp.from_secs(int(subscription_status["validUntil"])).to_human_datetime()))
                             user_has_active_subscription = True
                             update_user_subscription(user.npub,
                                                      int(subscription_status["validUntil"]),
                                                      self.client, self.dvm_config)
@@ -345,20 +350,20 @@
                                                                  "Someone zapped the result of an exisiting Task. Nice")
                     elif not anon:
                         print("[" + self.dvm_config.NIP89.NAME + "] Note Zap received for DVM balance: " +
                               str(invoice_amount) + " Sats from " + str(user.name))
                     #    update_user_balance(self.dvm_config.DB, sender, invoice_amount, client=self.client,
                     #                        config=self.dvm_config)
 
-                        # a regular note
+                    # a regular note
                 elif not anon and dvm_config.NIP88 is None:
                     print("[" + self.dvm_config.NIP89.NAME + "] Profile Zap received for DVM balance: " +
                           str(invoice_amount) + " Sats from " + str(user.name))
-                   # update_user_balance(self.dvm_config.DB, sender, invoice_amount, client=self.client,
-                   #                     config=self.dvm_config)
+                # update_user_balance(self.dvm_config.DB, sender, invoice_amount, client=self.client,
+                #                     config=self.dvm_config)
 
             except Exception as e:
                 print("[" + self.dvm_config.NIP89.NAME + "] Error during content decryption: " + str(e))
 
         def check_event_has_not_unfinished_job_input(nevent, append, client, dvmconfig):
             task_supported, task = check_task_is_supported(nevent, client, config=dvmconfig)
             if not task_supported:
@@ -468,16 +473,17 @@
                 content = nip04_encrypt(self.keys.secret_key(), PublicKey.from_hex(original_event.author().to_hex()),
                                         content)
 
             reply_event = EventBuilder(Kind(original_event.kind().as_u64() + 1000), str(content), reply_tags).to_event(
                 self.keys)
 
             send_event(reply_event, client=self.client, dvm_config=self.dvm_config)
-            print("[" + self.dvm_config.NIP89.NAME + "] " + str(
-                original_event.kind().as_u64() + 1000) + " Job Response event sent: " + reply_event.as_json())
+
+            print(bcolors.GREEN + "[" + self.dvm_config.NIP89.NAME + "] " + str(
+                original_event.kind().as_u64() + 1000) + " Job Response event sent: " + reply_event.as_json() + bcolors.ENDC)
 
         def send_job_status_reaction(original_event, status, is_paid=True, amount=0, client=None,
                                      content=None,
                                      dvm_config=None, user=None):
 
             task = get_task(original_event, client=client, dvm_config=dvm_config)
             alt_description, reaction = build_status_reaction(status, task, amount, content, dvm_config)
@@ -499,15 +505,14 @@
             if encrypted:
                 encryption_tags.append(p_tag)
                 encryption_tags.append(e_tag)
 
             else:
                 reply_tags.append(p_tag)
 
-
             if status == "success" or status == "error":  #
                 for x in self.job_list:
                     if x.event == original_event:
                         is_paid = x.is_paid
                         amount = x.amount
                         break
 
@@ -568,16 +573,17 @@
 
             else:
                 content = reaction
 
             keys = Keys.parse(dvm_config.PRIVATE_KEY)
             reaction_event = EventBuilder(EventDefinitions.KIND_FEEDBACK, str(content), reply_tags).to_event(keys)
             send_event(reaction_event, client=self.client, dvm_config=self.dvm_config)
-            print("[" + self.dvm_config.NIP89.NAME + "]" + ": Sent Kind " + str(
-                EventDefinitions.KIND_FEEDBACK.as_u64()) + " Reaction: " + status + " " + reaction_event.as_json())
+
+            print(bcolors.YELLOW + "[" + self.dvm_config.NIP89.NAME + "]" + " Sent Kind " + str(
+                EventDefinitions.KIND_FEEDBACK.as_u64()) + " Reaction: " + status + " " + reaction_event.as_json() + bcolors.ENDC)
             return reaction_event.as_json()
 
         def do_work(job_event, amount):
             if ((
                     EventDefinitions.KIND_NIP90_EXTRACT_TEXT.as_u64() <= job_event.kind().as_u64() <= EventDefinitions.KIND_NIP90_GENERIC.as_u64())
                     or job_event.kind().as_u64() == EventDefinitions.KIND_DM.as_u64()):
 
@@ -614,19 +620,21 @@
                             else:  # Some components might have issues with running code in otuside venv.
                                 # We install locally in these cases for now
                                 result = dvm.process(request_form)
                             try:
                                 post_processed = dvm.post_process(result, job_event)
                                 send_nostr_reply_event(post_processed, job_event.as_json())
                             except Exception as e:
-                                print(e)
+                                print(bcolors.RED + "[" + self.dvm_config.NIP89.NAME + "] Error: " + str(e) + bcolors.ENDC)
                                 send_job_status_reaction(job_event, "error", content=str(e),
                                                          dvm_config=self.dvm_config)
                     except Exception as e:
-                        print(e)
+                        print(
+                            bcolors.RED + "[" + self.dvm_config.NIP89.NAME + "] Error: " + str(e) + bcolors.ENDC)
+
                         # we could send the exception here to the user, but maybe that's not a good idea after all.
                         send_job_status_reaction(job_event, "error", content=result,
                                                  dvm_config=self.dvm_config)
                         # Zapping back the user on error
                         if amount > 0 and self.dvm_config.LNBITS_ADMIN_KEY != "":
                             user = get_or_add_user(self.dvm_config.DB, job_event.author().to_hex(),
                                                    client=self.client, config=self.dvm_config)
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.5.2/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,21 +119,21 @@
         "Process the data and return the result"
         pass
 
     def post_process(self, result, event):
         """Post-process the data and return the result Use default function, if not overwritten"""
         return post_process_result(result, event)
 
-    @staticmethod
-    def set_options(request_form):
-        print("Setting options...")
+    def set_options(self, request_form):
+
+        print("[" + self.dvm_config.NIP89.NAME + "] " + "Setting options...")
         opts = []
         if request_form.get("options"):
             opts = json.loads(request_form["options"])
-            print(opts)
+            print("[" + self.dvm_config.NIP89.NAME + "] " + str(opts))
         return dict(opts)
 
     @staticmethod
     def process_args():
         import argparse
         parser = argparse.ArgumentParser()
         parser.add_argument('--request', dest='request')
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/subscription.py` & `nostr_dvm-0.5.2/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/advanced_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             "relay": relay
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         cli = Client.with_opts(signer, opts)
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         userkeys = []
         for user in options["users"]:
             tag = Tag.parse(user)
             user = tag.as_vec()[1]
             user = str(user).lstrip("@")
             if str(user).startswith('npub'):
                 userkey = PublicKey.from_bech32(user)
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,14 @@
                 self.db_since = int(self.options.get("db_since"))
             if self.options.get("logger"):
                 self.logger = bool(self.options.get("logger"))
 
             if self.logger:
                 init_logger(LogLevel.DEBUG)
 
-
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
@@ -72,15 +71,14 @@
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
                     return False
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
-        print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
         search = ""
         max_results = 100
 
@@ -107,42 +105,41 @@
             return self.result
 
     def calculate_result(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
-        options = DVMTaskInterface.set_options(request_form)
-
+        options = self.set_options(request_form)
 
         database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().database(database).build()
 
-
         # Negentropy reconciliation
         # Query events from database
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         since = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
         events = cli.database().query([filter1])
+        print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
+
         ns.finallist = {}
         for event in events:
             if event.created_at().as_secs() > timestamp_hour_ago:
                 filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST,
                                        definitions.EventDefinitions.KIND_REACTION,
                                        definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
                 reactions = cli.database().query([filt])
                 if len(reactions) >= self.min_reactions:
                     ns.finallist[event.id().to_hex()] = len(reactions)
 
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
-            # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
             e_tag = Tag.parse(["e", entry[0]])
             result_list.append(e_tag.as_vec())
 
         return json.dumps(result_list)
 
     def post_process(self, result, event):
         """Overwrite the interface function to return a social client readable format, if requested"""
@@ -163,15 +160,15 @@
                 if self.dvm_config.UPDATE_DATABASE:
                     self.sync_db()
                 self.last_schedule = Timestamp.now().as_secs()
                 if not self.personalized:
                     try:
                         self.result = self.calculate_result(self.request_form)
                     except Exception as e:
-                        print("EXCEPTION: "+ e)
+                        print("EXCEPTION: " + str(e))
                 return 1
 
     def sync_db(self):
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
@@ -187,29 +184,30 @@
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
                                   definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(
+        print("[" + self.dvm_config.NIP89.NAME + "] Syncing notes of the last " + str(
             self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
-        database.delete(Filter().until(Timestamp.from_secs(
-            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesnt get too full.
+        filter_delete = Filter().until(Timestamp.from_secs(Timestamp.now().as_secs() - self.db_since))
+        database.delete(filter_delete)  # Clear old events so db doesn't get too full.
 
         print(
-            "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
+            "[" + self.dvm_config.NIP89.NAME + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, options,  cost=0, update_rate=180,  processing_msg=None, update_db=True):
+def build_example(name, identifier, admin_config, options, cost=0, update_rate=180, processing_msg=None,
+                  update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 10 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
@@ -240,22 +238,23 @@
         }
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    #admin_config.UPDATE_PROFILE = False
-    #admin_config.REBROADCAST_NIP89 = False
+    # admin_config.UPDATE_PROFILE = False
+    # admin_config.REBROADCAST_NIP89 = False
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           admin_config=admin_config, options=options)
 
 
-def build_example_subscription(name, identifier, admin_config, options, update_rate=180, processing_msg=None, update_db=True):
+def build_example_subscription(name, identifier, admin_config, options, update_rate=180, processing_msg=None,
+                               update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 3 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
@@ -297,17 +296,17 @@
     nip88config.AMOUNT_DAILY = 100
     nip88config.AMOUNT_MONTHLY = 2000
     nip88config.CONTENT = "Subscribe to the DVM for unlimited use during your subscription"
     nip88config.PERK1DESC = "Unlimited requests"
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
-    #admin_config.UPDATE_PROFILE = False
-    #admin_config.REBROADCAST_NIP89 = False
-    #admin_config.REBROADCAST_NIP88 = False
+    # admin_config.UPDATE_PROFILE = False
+    # admin_config.REBROADCAST_NIP89 = False
+    # admin_config.REBROADCAST_NIP88 = False
 
     # admin_config.FETCH_NIP88 = True
     # admin_config.EVENTID = ""
     # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           nip88config=nip88config, options=options,
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
             if self.options.get("db_since"):
                 self.db_since = int(self.options.get("db_since"))
             if self.options.get("logger"):
                 self.logger = bool(self.options.get("logger"))
 
             if self.logger:
                 init_logger(LogLevel.DEBUG)
-        print("UPDATEDB: " + str(self.dvm_config.UPDATE_DATABASE))
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
@@ -72,15 +71,14 @@
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
                     return False
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
-        print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
         max_results = 200
 
         for tag in event.tags():
@@ -106,26 +104,28 @@
             return self.result
 
     def calculate_result(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().database(database).build()
 
         # Negentropy reconciliation
         # Query events from database
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         since = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
         events = cli.database().query([filter1])
+        print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
+
         ns.finallist = {}
         for event in events:
             if event.created_at().as_secs() > timestamp_hour_ago:
                 filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP]).event(event.id()).since(since)
                 reactions = cli.database().query([filt])
                 invoice_amount = 0
                 haspreimage = False
@@ -194,23 +194,23 @@
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
                                   definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(
+        print("[" + self.dvm_config.NIP89.NAME + "] Syncing notes of the last " + str(
             self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
-        database.delete(Filter().until(Timestamp.from_secs(
-            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesnt get too full.
+        filter_delete = Filter().until(Timestamp.from_secs(Timestamp.now().as_secs() - self.db_since))
+        database.delete(filter_delete)  # Clear old events so db doesn't get too full.
 
         print(
-            "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
+            "[" + self.dvm_config.NIP89.NAME + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config, options, cost=0, update_rate=180, processing_msg=None,
                   update_db=True):
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
                     return False
         return True
 
     def create_request_from_nostr_event(self, event: Event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
-        print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
         user = event.author().to_hex()
         max_results = 100
 
@@ -91,15 +90,15 @@
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         relaylimits = RelayLimits.disable()
         opts = (
             Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)).relay_limits(
                 relaylimits))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
@@ -139,14 +138,15 @@
             for tag in best_entry.tags():
                 if tag.as_vec()[0] == "p":
                     following = PublicKey.parse(tag.as_vec()[1])
                     followings.append(following)
 
             filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).authors(followings).since(since)
             events = cli.database().query([filter1])
+            print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
 
             ns.finallist = {}
             for event in events:
                 # if event.created_at().as_secs() > timestamp_since:
                 filt = Filter().kinds(
                     [EventDefinitions.KIND_ZAP, EventDefinitions.KIND_REACTION, EventDefinitions.KIND_REPOST,
                      EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
@@ -203,23 +203,22 @@
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
                                   definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(
+        print("[" + self.dvm_config.NIP89.NAME + "] Syncing notes of the last " + str(
             self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
-        database.delete(Filter().until(Timestamp.from_secs(
-            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesnt get too full.
-
+        filter_delete = Filter().until(Timestamp.from_secs(Timestamp.now().as_secs() - self.db_since))
+        database.delete(filter_delete)  # Clear old events so db doesn't get too full.
         print(
-            "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
+            "[" + self.dvm_config.NIP89.NAME + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config, options, cost=0, update_rate=300, processing_msg=None,
                   update_db=True):
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,14 @@
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
                     return False
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
-        print(self.dvm_config.PRIVATE_KEY)
-
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
         max_results = 200
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
@@ -131,36 +129,26 @@
         return result
 
     def calculate_result(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
-        options = DVMTaskInterface.set_options(request_form)
-
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
-        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
-        keys = Keys.parse(sk.to_hex())
-        signer = NostrSigner.keys(keys)
+        options = self.set_options(request_form)
 
         database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().database(database).build()
-
-        # cli.add_relay("wss://relay.damus.io")
-        # cli.connect()
-
-        # Negentropy reconciliation
-        # Query events from database
         timestamp_since = Timestamp.now().as_secs() - self.db_since
         since = Timestamp.from_secs(timestamp_since)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
 
         events = cli.database().query([filter1])
-        print(len(events))
+        print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
+
         ns.final_list = {}
 
         for event in events:
             if all(ele in event.content().lower() for ele in self.must_list):
                 if any(ele in event.content().lower() for ele in self.search_list):
                     if not any(ele in event.content().lower() for ele in self.avoid_list):
 
@@ -193,43 +181,42 @@
                     if not self.personalized:
                         self.result = self.calculate_result(self.request_form)
                 except Exception as e:
                     print(e)
                 return 1
 
     def sync_db(self):
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         cli.add_relay("wss://nostr.oxtr.dev")
         cli.add_relay("wss://nostr21.com")
-
         cli.connect()
 
         timestamp_since = Timestamp.now().as_secs() - self.db_since
         since = Timestamp.from_secs(timestamp_since)
 
         filter1 = Filter().kinds([EventDefinitions.KIND_NOTE, EventDefinitions.KIND_REACTION, EventDefinitions.KIND_ZAP,
                                   EventDefinitions.KIND_LONGFORM]).since(since)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(
+        print("[" + self.dvm_config.NIP89.NAME + "] Syncing notes of the last " + str(
             self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
-        database.delete(Filter().until(Timestamp.from_secs(
-            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesn't get too full.
+        filter_delete = Filter().until(Timestamp.from_secs(Timestamp.now().as_secs() - self.db_since))
+        database.delete(filter_delete)  # Clear old events so db doesn't get too full.
 
         print(
-            "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
+            "[" + self.dvm_config.NIP89.NAME + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config, options, image, description, update_rate=600, cost=0,
                   processing_msg=None, update_db=True):
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/convert_media.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             "filepath": filepath
         }
 
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         url = upload_media_to_hoster(options["filepath"])
 
         return url
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             "max_results": max_results,
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
         database = NostrDatabase.sqlite("db/nostr_profiles.db")
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             cli.add_relay(relay)
         # add nostr band, too.
         ropts = RelayOptions().ping(False)
         cli.add_relay_with_opts("wss://nostr.band", ropts)
 
         cli.connect()
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         step = 20
 
         pubkeys = []
         for user in options["users"]:
             pubkeys.append(PublicKey.parse(user))
 
         # if we don't add users, e.g. by a wot, we check all our followers.
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         for relay in self.dvm_config.RELAY_LIST:
             cli.add_relay(relay)
         ropts = RelayOptions().ping(False)
         cli.add_relay_with_opts("wss://nostr.band", ropts)
 
         cli.connect()
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         step = 20
 
         followers_filter = Filter().author(PublicKey.parse(options["user"])).kind(Kind(3))
         followers = cli.get_events_of([followers_filter], timedelta(seconds=5))
 
 
         if len(followers) > 0:
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             cli.add_relay(relay)
         #add nostr band, too.
         ropts = RelayOptions().ping(False)
         cli.add_relay_with_opts("wss://nostr.band", ropts)
 
         cli.connect()
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         step = 20
 
         followers_filter = Filter().author(PublicKey.from_hex(options["user"])).kind(Kind(3))
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
 
         if len(followers) > 0:
             result_list = []
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         options = {
             "max_results": max_results,
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         import requests
 
         url = "https://api.nostr.band/v0/trending/notes"
         try:
             response = requests.get(url)
             response_json = response.json()
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         try:
-            options = DVMTaskInterface.set_options(request_form)
+            options = self.set_options(request_form)
 
             from openai import OpenAI
             client = OpenAI()
             print("Job " + request_form['jobID'] + " sent to OpenAI API..")
 
             response = client.images.generate(
                 model=options['model'],
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         try:
-            options = DVMTaskInterface.set_options(request_form)
+            options = self.set_options(request_form)
 
             import replicate
             width = int(options["size"].split("x")[0])
             height = int(options["size"].split("x")[1])
             output = replicate.run(
                 "stability-ai/sdxl:39ed52f2a78e934b3ba6e2a89f5b1c712de7dfea535525255b1aa35c5565e08b",
                 input={"prompt": options["prompt"],
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         return request_form
 
     def process(self, request_form):
         try:
             import mlx.core as mx
             from nostr_dvm.backends.mlx.modules.stable_diffusion import StableDiffusion
-            options = DVMTaskInterface.set_options(request_form)
+            options = self.set_options(request_form)
 
             sd = StableDiffusion()
             cfg_weight = 7.5
             batchsize = 1
             n_rows = 1
             steps = 50
             n_images = options["number"]
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/search_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             "max_results": max_results,
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
         database = NostrDatabase.sqlite(self.db_name)
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         try:
             cookies = sign.loadCookiesFromDir(
                 cookie_path_dir)  # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
         except:
             cookies = sign.login()
             sign.saveCookiesToDir(cookie_path_dir)
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         try:
             chatbot = hugchat.ChatBot(cookies=cookies.get_dict())  # or cookie_path="usercookies/<email>.json"
             query_result = chatbot.query("Summarize the following notes: " + str(options["prompt"]))
             print(query_result["text"])  # or query_result.text or query_result["text"]
             return str(query_result["text"]).lstrip()
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         return request_form
 
     def process(self, request_form):
         from openai import OpenAI
         temp_open_ai_api_key = os.environ["OPENAI_API_KEY"]
         os.environ["OPENAI_API_KEY"] = os.getenv("UNLEASHED_API_KEY")
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         try:
             client = OpenAI(
                 base_url='https://unleashed.chat/api/v1',
             )
 
             print('Models:\n')
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/textextraction_google.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     def process(self, request_form):
         import speech_recognition as sr
         if self.options.get("api_key"):
             api_key = self.options['api_key']
         else:
             api_key = None
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         # Speech recognition instance
         asr = sr.Recognizer()
         with sr.AudioFile(options["filepath"]) as source:
             audio = asr.record(source)  # read the entire audio file
 
         try:
             # Use Google Web Speech API to recognize speech from audio data
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         return request_form
 
     def process(self, request_form):
         from pypdf import PdfReader
         from pathlib import Path
         import requests
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         try:
             file_path = Path('temp.pdf')
             response = requests.get(options["url"])
             file_path.write_bytes(response.content)
             reader = PdfReader(file_path)
             number_of_pages = len(reader.pages)
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             cookies = sign.loadCookiesFromDir(
                 cookie_path_dir)  # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
         except:
             cookies = sign.login()
             sign.saveCookiesToDir(cookie_path_dir)
 
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         try:
             chatbot = hugchat.ChatBot(cookies=cookies.get_dict())  # or cookie_path="usercookies/<email>.json"
             query_result = chatbot.query(options["prompt"])
             print(query_result["text"])  # or query_result.text or query_result["text"]
             return str(query_result["text"]).lstrip()
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         from litellm import completion
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         try:
             if options["model"].startswith("ollama"):
                 response = completion(
                     model=options["model"],
                     messages=[{"content": options["prompt"], "role": "user"}],
                     api_base=options["server"],
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         return request_form
 
     def process(self, request_form):
         from openai import OpenAI
         temp_open_ai_api_key = os.environ["OPENAI_API_KEY"]
         os.environ["OPENAI_API_KEY"] = os.getenv("UNLEASHED_API_KEY")
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
 
         try:
             client = OpenAI(
                 base_url='https://unleashed.chat/api/v1',
             )
 
             print('Models:\n')
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/texttospeech.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         import torch
         from TTS.api import TTS
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         device = "cuda" if torch.cuda.is_available() else "cpu"
         # else "mps" if torch.backends.mps.is_available() \
 
         print(TTS().list_models())
         try:
             # model = "tts_models/deu/fairseq/vits"
             # model = "tts_models/multilingual/multi-dataset/your_tts"
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/translation_google.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from translatepy.translators.google import GoogleTranslate
 
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         gtranslate = GoogleTranslate()
         length = len(options["text"])
 
         step = 0
         translated_text = ""
         if length > 4999:
             while step + 5000 < length:
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             "text": text,
             "language": translation_lang
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
-        options = DVMTaskInterface.set_options(request_form)
+        options = self.set_options(request_form)
         request = {
             "q": options["text"],
             "source": "auto",
             "target": options["language"]
         }
         if options["libre_api_key"] != "":
             request["api_key"] = options["libre_api_key"]
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         try:
-            options = DVMTaskInterface.set_options(request_form)
+            options = self.set_options(request_form)
             print(options["url"])
             response = requests.get(options["url"])
             image = Image.open(BytesIO(response.content)).convert("RGB")
             image.save("./outputs/input.jpg")
 
             import replicate
             output = replicate.run(
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.5.2/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/nip88_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,16 @@
         tags.append(perk_tag)
 
     keys = Keys.parse(dvm_config.NIP89.PK)
     content = dvm_config.NIP88.CONTENT
     event = EventBuilder(EventDefinitions.KIND_NIP88_TIER_EVENT, content, tags).to_event(keys)
     annotier_id = send_event(event, client=client, dvm_config=dvm_config)
 
-    print("Announced NIP 88 Tier for " + dvm_config.NIP89.NAME)
+    print("[" + dvm_config.NAME + "] Announced NIP 88 Tier for " + dvm_config.NIP89.NAME)
+
     return annotier_id
 
     # Relay and payment-verification
 
 
 # ["r", "wss://my-subscribers-only-relay.com"],
 # ["p", "<payment-verifier-pubkey>"],
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/nip89_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import dotenv
 from nostr_sdk import Tag, Keys, EventBuilder, Filter, Alphabet, PublicKey, Client, EventId, SingleLetterTag, Kind
 
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.nostr_utils import send_event
+from nostr_dvm.utils.print import bcolors
 
 
 class NIP89Config:
     DTAG: str = ""
     NAME: str = ""
     KIND: int = None
     PK: str = ""
@@ -27,15 +28,17 @@
 def nip89_announce_tasks(dvm_config, client):
     k_tag = Tag.parse(["k", str(dvm_config.NIP89.KIND.as_u64())])
     d_tag = Tag.parse(["d", dvm_config.NIP89.DTAG])
     keys = Keys.parse(dvm_config.NIP89.PK)
     content = dvm_config.NIP89.CONTENT
     event = EventBuilder(EventDefinitions.KIND_ANNOUNCEMENT, content, [k_tag, d_tag]).to_event(keys)
     send_event(event, client=client, dvm_config=dvm_config)
-    print("Announced NIP 89 for " + dvm_config.NIP89.NAME)
+
+    print(bcolors.BLUE + "[" + dvm_config.NIP89.NAME + "] Announced NIP 89 for " + dvm_config.NIP89.NAME + bcolors.ENDC)
+
 
 
 def fetch_nip89_parameters_for_deletion(keys, eventid, client, dvmconfig, pow=False):
     idfilter = Filter().id(EventId.from_hex(eventid)).limit(1)
     nip89events = client.get_events_of([idfilter], timedelta(seconds=dvmconfig.RELAY_TIMEOUT))
     d_tag = ""
     if len(nip89events) == 0:
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/nostr_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,16 +207,15 @@
             .set_name(name) \
             .set_display_name(name) \
             .set_about(about) \
             .set_picture(image) \
             .set_lud16(lud16) \
             .set_nip05(lud16)
         # .set_banner("https://example.com/banner.png") \
-
-        print(f"Setting profile metadata for {keys.public_key().to_bech32()}...")
+        print("[" + dvm_config.NIP89.NAME + "] Setting profile metadata for " + keys.public_key().to_bech32() + "...")
         print(metadata.as_json())
         client.set_metadata(metadata)
 
 
 def check_and_set_private_key(identifier):
     if not os.getenv("DVM_PRIVATE_KEY_" + identifier.upper()):
         pk = Keys.generate().secret_key().to_hex()
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.5.2/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.5.2/nostr_dvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.1
+Version: 0.5.2
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.1/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.5.2/nostr_dvm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -85,13 +85,14 @@
 nostr_dvm/utils/external_dvm_utils.py
 nostr_dvm/utils/mediasource_utils.py
 nostr_dvm/utils/nip88_utils.py
 nostr_dvm/utils/nip89_utils.py
 nostr_dvm/utils/nostr_utils.py
 nostr_dvm/utils/nwc_tools.py
 nostr_dvm/utils/output_utils.py
+nostr_dvm/utils/print.py
 nostr_dvm/utils/subscription_utils.py
 nostr_dvm/utils/zap_utils.py
 nostr_dvm/utils/scrapper/__init__.py
 nostr_dvm/utils/scrapper/media_scrapper.py
 tests/test_dvm_client.py
 tests/test_events.py
```

### Comparing `nostr_dvm-0.5.1/setup.py` & `nostr_dvm-0.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.1'
+VERSION = '0.5.2'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
     author="Believethehype",
     author_email="believethehypeonnostr@proton.me",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(include=['nostr_dvm', 'nostr_dvm.*']),
-#nostr-sdk==0.13.0a2.dev0
+
     install_requires=["nostr-sdk==0.12.0",
                       "bech32",
                       "pycryptodome==3.20.0",
                       "python-dotenv==1.0.0",
                       "emoji==2.8.0",
                       "eva-decord==0.6.1",
                       "ffmpegio==0.8.5",
```

### Comparing `nostr_dvm-0.5.1/tests/test_dvm_client.py` & `nostr_dvm-0.5.2/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.1/tests/test_events.py` & `nostr_dvm-0.5.2/tests/test_events.py`

 * *Files identical despite different names*

