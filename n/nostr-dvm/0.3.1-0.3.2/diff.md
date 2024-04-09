# Comparing `tmp/nostr-dvm-0.3.1.tar.gz` & `tmp/nostr-dvm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr-dvm-0.3.1.tar", last modified: Wed Apr  3 21:58:17 2024, max compression
+gzip compressed data, was "nostr-dvm-0.3.2.tar", last modified: Tue Apr  9 13:41:35 2024, max compression
```

## Comparing `nostr-dvm-0.3.1.tar` & `nostr-dvm-0.3.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36516 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39387 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.479745 nostr-dvm-0.3.1/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.479745 nostr-dvm-0.3.1/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36516 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39387 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22893 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.941900 nostr-dvm-0.3.2/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.941900 nostr-dvm-0.3.2/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.941900 nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/tests/test_events.py
```

### Comparing `nostr-dvm-0.3.1/LICENSE` & `nostr-dvm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/PKG-INFO` & `nostr-dvm-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.1
+Version: 0.3.2
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr-dvm-0.3.1/README.md` & `nostr-dvm-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/utils.py` & `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/bot.py` & `nostr-dvm-0.3.2/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/dvm.py` & `nostr-dvm-0.3.2/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr-dvm-0.3.2/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/subscription.py` & `nostr-dvm-0.3.2/nostr_dvm/subscription.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,388 +1,439 @@
 import json
+import math
 import os
 import signal
 import time
 from datetime import timedelta
 
-from nostr_sdk import (
-    Keys, Client, Timestamp, Filter, nip04_decrypt, HandleNotification, EventBuilder,
-    PublicKey, Options, Tag, Event, nip04_encrypt, NostrSigner, EventId, Kind
-)
+from nostr_sdk import (Keys, Client, Timestamp, Filter, nip04_decrypt, HandleNotification, EventBuilder, PublicKey,
+                       Options, Tag, Event, nip04_encrypt, NostrSigner, EventId, Nip19Event, nip44_decrypt, Kind)
 
 from nostr_dvm.utils.database_utils import fetch_user_metadata
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.nip88_utils import nip88_has_active_subscription
 from nostr_dvm.utils.nip89_utils import NIP89Config
 from nostr_dvm.utils.nostr_utils import send_event
 from nostr_dvm.utils.nwc_tools import nwc_zap
-from nostr_dvm.utils.subscription_utils import (
-    create_subscription_sql_table, add_to_subscription_sql_table, get_from_subscription_sql_table,
-    update_subscription_sql_table, get_all_subscriptions_from_sql_table, delete_from_subscription_sql_table
-)
+from nostr_dvm.utils.subscription_utils import create_subscription_sql_table, add_to_subscription_sql_table, \
+    get_from_subscription_sql_table, update_subscription_sql_table, get_all_subscriptions_from_sql_table, \
+    delete_from_subscription_sql_table
 from nostr_dvm.utils.zap_utils import create_bolt11_lud16, zaprequest
 
 
 class Subscription:
+    job_list: list
+
+    # This is a simple list just to keep track which events we created and manage, so we don't pay for other requests
     def __init__(self, dvm_config, admin_config=None):
         self.NAME = "Subscription Handler"
-        dvm_config.DB = "db/subscriptions.db"
+        dvm_config.DB = "db/" + "subscriptions" + ".db"
         self.dvm_config = dvm_config
         nip89config = NIP89Config()
         nip89config.NAME = self.NAME
         self.dvm_config.NIP89 = nip89config
         self.admin_config = admin_config
         self.keys = Keys.parse(dvm_config.PRIVATE_KEY)
         wait_for_send = False
         skip_disconnected_relays = True
         opts = (Options().wait_for_send(wait_for_send).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
                 .skip_disconnected_relays(skip_disconnected_relays))
         signer = NostrSigner.keys(self.keys)
         self.client = Client.with_opts(signer, opts)
 
-        public_key = self.keys.public_key()
+        pk = self.keys.public_key()
 
         self.job_list = []
 
-        print(f"Nostr Subscription Handler public key: {public_key.to_bech32()} Hex: {public_key.to_hex()}\n")
+        print("Nostr Subscription Handler public key: " + str(pk.to_bech32()) + " Hex: " + str(
+            pk.to_hex()) + "\n")
 
         for relay in self.dvm_config.RELAY_LIST:
             self.client.add_relay(relay)
         self.client.connect()
 
-        zap_filter = Filter().pubkey(public_key).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
+        zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         cancel_subscription_filter = Filter().kinds([EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT]).since(
             Timestamp.now())
         authors = []
         if admin_config is not None:
             for key in admin_config.USERNPUBS:
                 authors.append(PublicKey.parse(key))
-        dvm_filter = Filter().authors(authors).pubkey(public_key).kinds([EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION]).since(Timestamp.now())
+        dvm_filter = Filter().authors(authors).pubkey(pk).kinds([EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION]).since(
+            Timestamp.now())
 
         self.client.subscribe([zap_filter, dvm_filter, cancel_subscription_filter], None)
 
         create_subscription_sql_table(dvm_config.DB)
 
-        self.client.handle_notifications(self.NotificationHandler(self))
+        class NotificationHandler(HandleNotification):
+            client = self.client
+            dvm_config = self.dvm_config
+            keys = self.keys
+
+            def handle(self, relay_url, subscription_id, nostr_event: Event):
+                if nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION.as_u64():
+                    handle_nwc_request(nostr_event)
+                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT.as_u64():
+                    handle_cancel(nostr_event)
+
+            def handle_msg(self, relay_url, msg):
+                return
+
+        def handle_cancel(nostr_event):
+            print(nostr_event.as_json())
+            sender = nostr_event.author().to_hex()
+            kind7001eventid = ""
+            recipient = ""
+            if sender == self.keys.public_key().to_hex():
+                return
+
+            for tag in nostr_event.tags():
+                if tag.as_vec()[0] == "p":
+                    recipient = tag.as_vec()[1]
+                elif tag.as_vec()[0] == "e":
+                    kind7001eventid = tag.as_vec()[1]
+
+            if kind7001eventid != "":
+                subscription = get_from_subscription_sql_table(dvm_config.DB, kind7001eventid)
+
+                if subscription is not None:
+                    update_subscription_sql_table(dvm_config.DB, kind7001eventid, recipient,
+                                                  subscription.subscriber, subscription.nwc, subscription.cadence,
+                                                  subscription.amount, subscription.unit, subscription.begin,
+                                                  subscription.end,
+                                                  subscription.tier_dtag, subscription.zaps, subscription.recipe,
+                                                  False, Timestamp.now().as_secs(), subscription.tier)
+
+        # send_status_canceled(kind7001eventid, nostr_event) # TODO, waiting for spec
+
+        def infer_subscription_end_time(start, cadence):
+            end = start
+            if cadence == "daily":
+                end = start + 60 * 60 * 24
+            elif cadence == "weekly":
+                end = start + 60 * 60 * 24 * 7
+            elif cadence == "monthly":
+                # TODO check days of month -.-
+                end = start + 60 * 60 * 24 * 31
+            elif cadence == "yearly":
+                # TODO check extra day every 4 years
+                end = start + 60 * 60 * 24 * 356
+            return end
+
+        def send_status_success(original_event, domain):
+
+            e_tag = Tag.parse(["e", original_event.id().to_hex()])
+            p_tag = Tag.parse(["p", original_event.author().to_hex()])
+            status_tag = Tag.parse(["status", "success", "Job has been scheduled, you can manage it on " + domain])
+            reply_tags = [status_tag]
+            encryption_tags = []
+
+            encrypted_tag = Tag.parse(["encrypted"])
+            encryption_tags.append(encrypted_tag)
+            encryption_tags.append(p_tag)
+            encryption_tags.append(e_tag)
+
+            str_tags = []
+            for element in reply_tags:
+                str_tags.append(element.as_vec())
+
+            content = json.dumps(str_tags)
+            content = nip04_encrypt(self.keys.secret_key(), PublicKey.from_hex(original_event.author().to_hex()),
+                                    content)
+            reply_tags = encryption_tags
+
+            keys = Keys.parse(dvm_config.PRIVATE_KEY)
+            reaction_event = EventBuilder(EventDefinitions.KIND_FEEDBACK, str(content), reply_tags).to_event(keys)
+            send_event(reaction_event, client=self.client, dvm_config=self.dvm_config)
+            print("[" + self.dvm_config.NIP89.NAME + "]" + ": Sent Kind " + str(
+                EventDefinitions.KIND_FEEDBACK.as_u64()) + " Reaction: " + "success" + " " + reaction_event.as_json())
+
+        def pay_zap_split(nwc, overall_amount, zaps, tier, unit="msats"):
+            overallsplit = 0
+
+            for zap in zaps:
+                print(zap)
+                overallsplit += int(zap[3])
+
+            print(overallsplit)
+            zapped_amount = 0
+            for zap in zaps:
+                if zap[1] == "":
+                    zap[1] = Keys.parse(self.dvm_config.PRIVATE_KEY).public_key().to_hex()
+
+                name, nip05, lud16 = fetch_user_metadata(zap[1], self.client)
+                splitted_amount = math.floor(
+                    (int(zap[3]) / overallsplit) * int(overall_amount) / 1000)
+                # invoice = create_bolt11_lud16(lud16, splitted_amount)
+                # TODO add details about DVM in message
+
+                invoice = zaprequest(lud16, splitted_amount, tier, None,
+                                     PublicKey.parse(zap[1]), self.keys, DVMConfig.RELAY_LIST)
+                print(invoice)
+                if invoice is not None:
+                    nwc_event_id = nwc_zap(nwc, invoice, self.keys, zap[2])
+                    if nwc_event_id is None:
+                        print("error zapping " + lud16)
+                    else:
+                        zapped_amount = zapped_amount + (splitted_amount * 1000)
+                        print(str(zapped_amount) + "/" + str(overall_amount))
 
-        try:
-            while True:
-                time.sleep(60.0)
-                self.check_subscriptions()
+            if zapped_amount < overall_amount * 0.8:  # TODO how do we handle failed zaps for some addresses? we are ok with 80% for now
+                success = False
+            else:
+                success = True
+                # if no active subscription exists OR the subscription ended, pay
 
-        except KeyboardInterrupt:
-            print('Stay weird!')
-            os.kill(os.getpid(), signal.SIGTERM)
+            return success
 
-    def check_subscriptions(self):
-        subscriptions = get_all_subscriptions_from_sql_table(self.dvm_config.DB)
+        def make_subscription_zap_recipe(event7001, recipient, subscriber, start, end, tier_dtag):
+            message = "payed by subscription service"
+            pTag = Tag.parse(["p", recipient])
+            PTag = Tag.parse(["P", subscriber])
+            eTag = Tag.parse(["e", event7001])
+            validTag = Tag.parse(["valid", str(start), str(end)])
+            tierTag = Tag.parse(["tier", tier_dtag])
+            alttag = Tag.parse(["alt", "This is a NIP90 DVM Subscription Payment Recipe"])
+
+            tags = [pTag, PTag, eTag, validTag, tierTag, alttag]
+
+            event = EventBuilder(EventDefinitions.KIND_NIP88_PAYMENT_RECIPE,
+                                 message, tags).to_event(self.keys)
+
+            dvmconfig = DVMConfig()
+            signer = NostrSigner.keys(self.keys)
+            client = Client(signer)
+            for relay in dvmconfig.RELAY_LIST:
+                client.add_relay(relay)
+            client.connect()
+            recipeid = client.send_event(event)
+            recipe = recipeid.to_hex()
+            return recipe
+
+        def handle_nwc_request(nostr_event):
+            print(nostr_event.as_json())
+            sender = nostr_event.author().to_hex()
+            if sender == self.keys.public_key().to_hex():
+                return
 
-        for subscription in subscriptions:
-            if subscription.active:
-                if subscription.end < Timestamp.now().as_secs():
-                    self.handle_subscription_renewal(subscription)
-            else:
-                self.handle_expired_subscription(subscription)
+            try:
+                decrypted_text = nip04_decrypt(self.keys.secret_key(), nostr_event.author(), nostr_event.content())
+                try:
+                    jsonevent = json.loads(decrypted_text)
+                    for entry in jsonevent:
+                        if entry[1] == "nwc":
+                            nwc = entry[2]
+                        elif entry[1] == "p":
+                            subscriber = entry[2]
+
+                    subscriptionfilter = Filter().kind(EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT).author(
+                        PublicKey.parse(subscriber)).limit(1)
+                    evts = self.client.get_events_of([subscriptionfilter], timedelta(seconds=3))
+                    print(evts)
+                    if len(evts) > 0:
+                        event7001id = evts[0].id().to_hex()
+                        print(evts[0].as_json())
+                        tier_dtag = ""
+                        recipient = ""
+                        cadence = ""
+                        unit = "msats"
+                        zaps = []
+                        tier = "DVM"
+                        overall_amount = 0
+                        for tag in evts[0].tags():
+                            if tag.as_vec()[0] == "amount":
+                                overall_amount = int(tag.as_vec()[1])
+
+                                unit = tag.as_vec()[2]
+                                cadence = tag.as_vec()[3]
+                                print(str(overall_amount) + " " + unit + " " + cadence)
+                            elif tag.as_vec()[0] == "p":
+                                recipient = tag.as_vec()[1]
+                            elif tag.as_vec()[0] == "e":
+                                subscription_event_id = tag.as_vec()[1]
+                            elif tag.as_vec()[0] == "event":
+                                jsonevent = json.loads(tag.as_vec()[1])
+                                subscription_event = Event.from_json(jsonevent)
+
+                                for tag in subscription_event.tags():
+                                    if tag.as_vec()[0] == "d":
+                                        tier_dtag = tag.as_vec()[1]
+                                    elif tag.as_vec()[0] == "zap":
+                                        zaps.append(tag.as_vec())
+                                    elif tag.as_vec()[0] == "title":
+                                        tier = tag.as_vec()[1]
+
+                        if tier_dtag == "" or len(zaps) == 0:
+                            tierfilter = Filter().id(EventId.parse(subscription_event_id))
+                            evts = self.client.get_events_of([tierfilter], timedelta(seconds=3))
+                            if len(evts) > 0:
+                                for tag in evts[0].tags():
+                                    if tag.as_vec()[0] == "d":
+                                        tier_dtag = tag.as_vec()[0]
+
+                        isactivesubscription = False
+                        recipe = ""
+                        subscription = get_from_subscription_sql_table(dvm_config.DB, event7001id)
+
+                        zapsstr = json.dumps(zaps)
+                        print(zapsstr)
+                        success = True
+                        if subscription is None or subscription.end <= Timestamp.now().as_secs():
+                            # rather check nostr if our db is right
+                            subscription_status = nip88_has_active_subscription(
+                                PublicKey.parse(subscriber),
+                                tier_dtag, self.client, recipient, checkCanceled=False)
+
+                            if not subscription_status["isActive"]:
+                                start = Timestamp.now().as_secs()
+                                end = infer_subscription_end_time(start, cadence)
+
+                                # we add or update the subscription in the db, with non-active subscription to avoid double payments
+                                if subscription is None:
+                                    add_to_subscription_sql_table(dvm_config.DB, event7001id, recipient, subscriber,
+                                                                  nwc,
+                                                                  cadence, overall_amount, unit, start, end, tier_dtag,
+                                                                  zapsstr, recipe, isactivesubscription,
+                                                                  Timestamp.now().as_secs(), tier)
+                                    print("new subscription entry before payment")
+                                else:
+                                    update_subscription_sql_table(dvm_config.DB, event7001id, recipient, subscriber,
+                                                                  nwc,
+                                                                  cadence, overall_amount, unit, start, end,
+                                                                  tier_dtag, zapsstr, recipe, isactivesubscription,
+                                                                  Timestamp.now().as_secs(), tier)
+                                    print("updated subscription entry before payment")
+
+                                # we attempt to pay the subscription
+                                success = pay_zap_split(nwc, overall_amount, zaps, tier, unit)
+
+                            else:
+                                start = Timestamp.now().as_secs()
+                                end = subscription_status["validUntil"]
+                        else:
+                            start = subscription.begin
+                            end = subscription.end
+
+                        if success:
+                            # we create a payment recipe
+                            recipe = make_subscription_zap_recipe(event7001id, recipient, subscriber, start, end,
+                                                                  tier_dtag)
+                            print("RECIPE " + recipe)
+                            isactivesubscription = True
+
+                            # we then update the subscription based on payment success
+                            update_subscription_sql_table(dvm_config.DB, event7001id, recipient, subscriber, nwc,
+                                                          cadence, overall_amount, unit, start, end,
+                                                          tier_dtag, zapsstr, recipe, isactivesubscription,
+                                                          Timestamp.now().as_secs(), tier)
+                            print("updated subscription entry after payment")
+
+                            send_status_success(nostr_event, "noogle.lol")
+
+                            keys = Keys.parse(dvm_config.PRIVATE_KEY)
+                            message = ("Subscribed to DVM " + tier + ". Renewing on: " + str(
+                                Timestamp.from_secs(end).to_human_datetime().replace("Z", " ").replace("T", " ")))
+                            evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.parse(subscriber), message,
+                                                                    None).to_event(keys)
+                            send_event(evt, client=self.client, dvm_config=dvm_config)
 
-        print(f"{Timestamp.now().as_secs()}: Checking {len(subscriptions)} Subscription entries..")
 
-    def handle_subscription_renewal(self, subscription):
-        subscription_status = nip88_has_active_subscription(
-            PublicKey.parse(subscription.subscriber),
-            subscription.tier_dtag, self.client, subscription.recipent)
 
-        if subscription_status["expires"]:
-            update_subscription_sql_table(self.dvm_config.DB, subscription_status["subscriptionId"],
-                                          subscription.recipent,
-                                          subscription.subscriber, subscription.nwc,
-                                          subscription.cadence, subscription.amount, subscription.unit,
-                                          subscription.begin, subscription.end,
-                                          subscription.tier_dtag, subscription.zaps,
-                                          subscription.recipe,
-                                          False,
-                                          Timestamp.now().as_secs(), subscription.tier)
-        else:
+                except Exception as e:
+                    print(e)
+
+            except Exception as e:
+                print("Error in Subscriber " + str(e))
+
+        def handle_expired_subscription(subscription):
+            delete_threshold = 60 * 60 * 24 * 365
+            if subscription.cadence == "daily":
+                delete_threshold = 60 * 60 * 24 * 3  # After 3 days, delete the subscription, user can make a new one
+            elif subscription.cadence == "weekly":
+                delete_threshold = 60 * 60 * 24 * 21  # After 21 days, delete the subscription, user can make a new one
+            elif subscription.cadence == "monthly":
+                delete_threshold = 60 * 60 * 24 * 60  # After 60 days, delete the subscription, user can make a new one
+            elif subscription.cadence == "yearly":
+                delete_threshold = 60 * 60 * 24 * 500  # After 500 days, delete the subscription, user can make a new one
+
+            if subscription.end < (Timestamp.now().as_secs() - delete_threshold):
+                delete_from_subscription_sql_table(dvm_config.DB, subscription.id)
+                print("Delete expired subscription")
+
+        def handle_subscription_renewal(subscription):
             zaps = json.loads(subscription.zaps)
-            success = self.pay_zap_split(subscription.nwc, subscription.amount, zaps, subscription.tier,
-                                         subscription.unit)
+            success = pay_zap_split(subscription.nwc, subscription.amount, zaps, subscription.tier,
+                                    subscription.unit)
             if success:
-                end = self.infer_subscription_end_time(Timestamp.now().as_secs(), subscription.cadence)
-                recipe = self.make_subscription_zap_recipe(subscription.id, subscription.recipent,
-                                                           subscription.subscriber, subscription.begin,
-                                                           end, subscription.tier_dtag)
+                end = infer_subscription_end_time(Timestamp.now().as_secs(), subscription.cadence)
+                recipe = make_subscription_zap_recipe(subscription.id, subscription.recipent,
+                                                      subscription.subscriber, subscription.begin,
+                                                      end, subscription.tier_dtag)
             else:
                 end = Timestamp.now().as_secs()
                 recipe = subscription.recipe
 
-            update_subscription_sql_table(self.dvm_config.DB, subscription.id,
+            update_subscription_sql_table(dvm_config.DB, subscription.id,
                                           subscription.recipent,
                                           subscription.subscriber, subscription.nwc,
-                                          subscription.cadence, subscription.amount, subscription.unit,
+                                          subscription.cadence, subscription.amount,
+                                          subscription.unit,
                                           subscription.begin, end,
                                           subscription.tier_dtag, subscription.zaps, recipe,
                                           success,
                                           Timestamp.now().as_secs(), subscription.tier)
 
-            print("Updated subscription entry")
+            print("updated subscription entry")
+
+            keys = Keys.parse(dvm_config.PRIVATE_KEY)
+            message = (
+                    "Renewed Subscription to DVM " + subscription.tier + ". Next renewal: " + str(
+                Timestamp.from_secs(end).to_human_datetime().replace("Z", " ").replace("T",
+                                                                                       " ")))
+            evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.parse(subscription.subscriber),
+                                                    message,
+                                                    None).to_event(keys)
+            send_event(evt, client=self.client, dvm_config=dvm_config)
+
+        def check_subscriptions():
+            subscriptions = get_all_subscriptions_from_sql_table(dvm_config.DB)
+
+            for subscription in subscriptions:
+                if subscription.active:
+                    if subscription.end < Timestamp.now().as_secs():
+                        # We could directly zap, but let's make another check if our subscription expired
+                        subscription_status = nip88_has_active_subscription(
+                            PublicKey.parse(subscription.subscriber),
+                            subscription.tier_dtag, self.client, subscription.recipent)
+
+                        if subscription_status["expires"]:
+                            # if subscription expires, just note it as not active
+                            update_subscription_sql_table(dvm_config.DB, subscription_status["subscriptionId"],
+                                                          subscription.recipent,
+                                                          subscription.subscriber, subscription.nwc,
+                                                          subscription.cadence, subscription.amount,
+                                                          subscription.unit,
+                                                          subscription.begin, subscription.end,
+                                                          subscription.tier_dtag, subscription.zaps,
+                                                          subscription.recipe,
+                                                          False,
+                                                          Timestamp.now().as_secs(), subscription.tier)
+                        else:
+                            handle_subscription_renewal(subscription)
 
-            message = (f"Renewed Subscription to DVM {subscription.tier}. "
-                       f"Next renewal: {Timestamp.from_secs(end).to_human_datetime().replace('Z', ' ').replace('T', ' ')}")
-            self.send_direct_message(subscription.subscriber, message)
-
-    def handle_expired_subscription(self, subscription):
-        delete_threshold = 60 * 60 * 24 * 365
-        if subscription.cadence == "daily":
-            delete_threshold = 60 * 60 * 24 * 3  # After 3 days, delete the subscription, user can make a new one
-        elif subscription.cadence == "weekly":
-            delete_threshold = 60 * 60 * 24 * 21  # After 21 days, delete the subscription, user can make a new one
-        elif subscription.cadence == "monthly":
-            delete_threshold = 60 * 60 * 24 * 60  # After 60 days, delete the subscription, user can make a new one
-        elif subscription.cadence == "yearly":
-            delete_threshold = 60 * 60 * 24 * 500  # After 500 days, delete the subscription, user can make a new one
-
-        if subscription.end < (Timestamp.now().as_secs() - delete_threshold):
-            delete_from_subscription_sql_table(self.dvm_config.DB, subscription.id)
-            print("Deleted expired subscription")
-
-    def pay_zap_split(self, nwc, overall_amount, zaps, tier, unit="msats"):
-        overallsplit = sum(int(zap[3]) for zap in zaps)
-        zapped_amount = 0
-
-        for zap in zaps:
-            if zap[1] == "":
-                zap[1] = self.keys.public_key().to_hex()
-
-            name, nip05, lud16 = fetch_user_metadata(zap[1], self.client)
-            splitted_amount = int((int(zap[3]) / overallsplit) * int(overall_amount) / 1000)
-
-            invoice = zaprequest(lud16, splitted_amount, tier, None,
-                                 PublicKey.parse(zap[1]), self.keys, DVMConfig.RELAY_LIST)
-
-            if invoice is not None:
-                nwc_event_id = nwc_zap(nwc, invoice, self.keys, zap[2])
-                if nwc_event_id is None:
-                    print(f"Error zapping {lud16}")
                 else:
-                    zapped_amount += splitted_amount * 1000
-                    print(f"{zapped_amount}/{overall_amount}")
+                    handle_expired_subscription(subscription)
 
-        return zapped_amount >= overall_amount * 0.8
+            print(str(Timestamp.now().as_secs()) + ": Checking " + str(
+                len(subscriptions)) + " Subscription entries..")
 
-    def make_subscription_zap_recipe(self, event7001, recipient, subscriber, start, end, tier_dtag):
-        message = "Paid by subscription service"
-        p_tag = Tag.parse(["p", recipient])
-        p_subscriber_tag = Tag.parse(["P", subscriber])
-        e_tag = Tag.parse(["e", event7001])
-        valid_tag = Tag.parse(["valid", str(start), str(end)])
-        tier_tag = Tag.parse(["tier", tier_dtag])
-        alt_tag = Tag.parse(["alt", "This is a NIP90 DVM Subscription Payment Recipe"])
-
-        tags = [p_tag, p_subscriber_tag, e_tag, valid_tag, tier_tag, alt_tag]
-
-        event = EventBuilder(EventDefinitions.KIND_NIP88_PAYMENT_RECIPE,
-                             message, tags).to_event(self.keys)
-
-        recipeid = self.client.send_event(event)
-        recipe = recipeid.to_hex()
-        return recipe
-
-    def infer_subscription_end_time(self, start, cadence):
-        end = start
-        if cadence == "daily":
-            end = start + 60 * 60 * 24
-        elif cadence == "weekly":
-            end = start + 60 * 60 * 24 * 7
-        elif cadence == "monthly":
-            end = start + 60 * 60 * 24 * 31
-        elif cadence == "yearly":
-            end = start + 60 * 60 * 24 * 356
-        return end
-
-    def send_direct_message(self, recipient, message):
-        evt = EventBuilder.encrypted_direct_msg(self.keys, PublicKey.parse(recipient), message, None).to_event(
-            self.keys)
-        send_event(evt, client=self.client, dvm_config=self.dvm_config)
-
-    class NotificationHandler(HandleNotification):
-        def __init__(self, subscription):
-            self.subscription = subscription
-
-        def handle(self, relay_url, subscription_id, nostr_event: Event):
-            if nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION.as_u64():
-                self.subscription.handle_nwc_request(nostr_event)
-            elif nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT.as_u64():
-                self.subscription.handle_cancel(nostr_event)
-
-        def handle_msg(self, relay_url, msg):
-            pass
-
-    def send_status_success(self, original_event, domain):
-
-        e_tag = Tag.parse(["e", original_event.id().to_hex()])
-        p_tag = Tag.parse(["p", original_event.author().to_hex()])
-        status_tag = Tag.parse(["status", "success", "Job has been scheduled, you can manage it on " + domain])
-        reply_tags = [status_tag]
-        encryption_tags = []
-
-        encrypted_tag = Tag.parse(["encrypted"])
-        encryption_tags.append(encrypted_tag)
-        encryption_tags.append(p_tag)
-        encryption_tags.append(e_tag)
-
-        str_tags = []
-        for element in reply_tags:
-            str_tags.append(element.as_vec())
-
-        content = json.dumps(str_tags)
-        content = nip04_encrypt(self.keys.secret_key(), PublicKey.from_hex(original_event.author().to_hex()),
-                                content)
-        reply_tags = encryption_tags
-
-        keys = Keys.parse(self.dvm_config.PRIVATE_KEY)
-        reaction_event = EventBuilder(EventDefinitions.KIND_FEEDBACK, str(content), reply_tags).to_event(keys)
-        send_event(reaction_event, client=self.client, dvm_config=self.dvm_config)
-
-    def handle_cancel(self, nostr_event):
-        print(nostr_event.as_json())
-        sender = nostr_event.author().to_hex()
-        if sender == self.keys.public_key().to_hex():
-            return
-
-        kind7001eventid = ""
-        recipient = ""
-        for tag in nostr_event.tags():
-            if tag.as_vec()[0] == "p":
-                recipient = tag.as_vec()[1]
-            elif tag.as_vec()[0] == "e":
-                kind7001eventid = tag.as_vec()[1]
-
-        if kind7001eventid != "":
-            subscription = get_from_subscription_sql_table(self.dvm_config.DB, kind7001eventid)
-
-            if subscription is not None:
-                update_subscription_sql_table(self.dvm_config.DB, kind7001eventid, recipient,
-                                              subscription.subscriber, subscription.nwc, subscription.cadence,
-                                              subscription.amount, subscription.unit, subscription.begin,
-                                              subscription.end,
-                                              subscription.tier_dtag, subscription.zaps, subscription.recipe,
-                                              False, Timestamp.now().as_secs(), subscription.tier)
-
-    def handle_nwc_request(self, nostr_event):
-        print(nostr_event.as_json())
-        sender = nostr_event.author().to_hex()
-        if sender == self.keys.public_key().to_hex():
-            return
+        self.client.handle_notifications(NotificationHandler())
 
         try:
-            decrypted_text = nip04_decrypt(self.keys.secret_key(), nostr_event.author(), nostr_event.content())
-            try:
-                jsonevent = json.loads(decrypted_text)
-                nwc = ""
-                subscriber = ""
-                for entry in jsonevent:
-                    if entry[1] == "nwc":
-                        nwc = entry[2]
-                    elif entry[1] == "p":
-                        subscriber = entry[2]
-
-                subscriptionfilter = Filter().kind(EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT).author(
-                    PublicKey.parse(subscriber)).limit(1)
-                evts = self.client.get_events_of([subscriptionfilter], timedelta(seconds=3))
-
-                if len(evts) > 0:
-                    self.process_subscription_event(evts[0], nwc, subscriber)
-            except Exception as e:
-                print(f"Error processing JSON event: {e}")
-        except Exception as e:
-            print(f"Error decrypting event content: {e}")
-
-    def process_subscription_event(self, subscription_event, nwc, subscriber):
-        event7001id = subscription_event.id().to_hex()
-        tier_dtag = ""
-        recipient = ""
-        cadence = ""
-        unit = "msats"
-        zaps = []
-        tier = "DVM"
-        overall_amount = 0
-        subscription_event_id = ""
-
-        for tag in subscription_event.tags():
-            if tag.as_vec()[0] == "amount":
-                overall_amount = int(tag.as_vec()[1])
-                unit = tag.as_vec()[2]
-                cadence = tag.as_vec()[3]
-                print(f"{overall_amount} {unit} {cadence}")
-            elif tag.as_vec()[0] == "p":
-                recipient = tag.as_vec()[1]
-            elif tag.as_vec()[0] == "e":
-                subscription_event_id = tag.as_vec()[1]
-            elif tag.as_vec()[0] == "event":
-                jsonevent = json.loads(tag.as_vec()[1])
-                subscription_event = Event.from_json(jsonevent)
-
-                for tag in subscription_event.tags():
-                    if tag.as_vec()[0] == "d":
-                        tier_dtag = tag.as_vec()[1]
-                    elif tag.as_vec()[0] == "zap":
-                        zaps.append(tag.as_vec())
-                    elif tag.as_vec()[0] == "title":
-                        tier = tag.as_vec()[1]
-
-        if tier_dtag == "" or len(zaps) == 0:
-            tierfilter = Filter().id(EventId.parse(subscription_event_id))
-            evts = self.client.get_events_of([tierfilter], timedelta(seconds=3))
-            if len(evts) > 0:
-                for tag in evts[0].tags():
-                    if tag.as_vec()[0] == "d":
-                        tier_dtag = tag.as_vec()[0]
-
-        isactivesubscription = False
-        recipe = ""
-
-        subscription = get_from_subscription_sql_table(self.dvm_config.DB, event7001id)
-        zapsstr = json.dumps(zaps)
-        print(zapsstr)
-        success = True
-        if subscription is None or subscription.end <= Timestamp.now().as_secs():
-            # rather check nostr if our db is right
-            subscription_status = nip88_has_active_subscription(
-                PublicKey.parse(subscriber),
-                tier_dtag, self.client, recipient, checkCanceled=False)
-
-            if not subscription_status["isActive"]:
-
-                success = self.pay_zap_split(nwc, overall_amount, zaps, tier, unit)
-                start = Timestamp.now().as_secs()
-                end = self.infer_subscription_end_time(start, cadence)
-            else:
-                start = Timestamp.now().as_secs()
-                end = subscription_status["validUntil"]
-        else:
-            start = subscription.begin
-            end = subscription.end
-
-        if success:
-            recipe = self.make_subscription_zap_recipe(event7001id, recipient, subscriber, start, end,
-                                                       tier_dtag)
-            print("RECIPE " + recipe)
-            isactivesubscription = True
-
-        if subscription is None:
-            add_to_subscription_sql_table(self.dvm_config.DB, event7001id, recipient, subscriber, nwc,
-                                          cadence, overall_amount, unit, start, end, tier_dtag,
-                                          zapsstr, recipe, isactivesubscription,
-                                          Timestamp.now().as_secs(), tier)
-            print("new subscription entry")
-        else:
-            update_subscription_sql_table(self.dvm_config.DB, event7001id, recipient, subscriber, nwc,
-                                          cadence, overall_amount, unit, start, end,
-                                          tier_dtag, zapsstr, recipe, isactivesubscription,
-                                          Timestamp.now().as_secs(), tier)
-            print("updated subscription entry")
-
-        self.send_status_success(subscription_event, "noogle.lol")
-
-        message = ("Subscribed to DVM " + tier + ". Renewing on: " + str(
-            Timestamp.from_secs(end).to_human_datetime().replace("Z", " ").replace("T", " ")))
-        self.send_direct_message(subscriber, message)
+            while True:
+                time.sleep(60.0)
+                check_subscriptions()
+        except KeyboardInterrupt:
+            print('Stay weird!')
+            os.kill(os.getpid(), signal.SIGTERM)
```

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search_wine.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
         database = NostrDatabase.sqlite("db/nostr_recent_notes2.db")
         cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
         cli.add_relay("wss://relay.damus.io")
-        cli.add_relay( "wss://nos.lol")
-        cli.add_relay( "wss://pablof7z.nostr1.com")
+        cli.add_relay("wss://nos.lol")
+        cli.add_relay("wss://pablof7z.nostr1.com")
 
         cli.connect()
 
         user = PublicKey.parse(options["user"])
         followers_filter = Filter().author(user).kinds([Kind(3)]).limit(1)
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
         print(followers)
```

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/convert_media.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/imageinterrogator.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/imageupscale.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/search_users.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_google.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_pdf.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/texttospeech.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/translation_google.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/translation_libretranslate.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_svd.py` & `nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/admin_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/backend_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/cashu_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/database_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/definitions.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/dvmconfig.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/external_dvm_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/mediasource_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/nip88_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/nip89_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/nip89_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from datetime import timedelta
 from hashlib import sha256
 from pathlib import Path
 
 import dotenv
-from nostr_sdk import Tag, Keys, EventBuilder, Filter, Alphabet, PublicKey, Client, EventId, SingleLetterTag
+from nostr_sdk import Tag, Keys, EventBuilder, Filter, Alphabet, PublicKey, Client, EventId, SingleLetterTag, Kind
 
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.nostr_utils import send_event
 
 
 class NIP89Config:
     DTAG: str = ""
@@ -55,16 +55,16 @@
             print("NIP89 announcement deleted from known relays!")
         else:
             print("Privatekey does not belong to event")
 
 
 def nip89_delete_announcement(eid: str, keys: Keys, dtag: str, client: Client, config):
     e_tag = Tag.parse(["e", eid])
-    a_tag = Tag.parse(["a", str(EventDefinitions.KIND_ANNOUNCEMENT) + ":" + keys.public_key().to_hex() + ":" + dtag])
-    event = EventBuilder(5, "", [e_tag, a_tag]).to_event(keys)
+    a_tag = Tag.parse(["a", str(EventDefinitions.KIND_ANNOUNCEMENT.as_u64()) + ":" + keys.public_key().to_hex() + ":" + dtag])
+    event = EventBuilder(Kind(5), "", [e_tag, a_tag]).to_event(keys)
     send_event(event, client, config)
 
 
 def nip89_fetch_all_dvms(client):
     ktags = []
     for i in range(5000, 5999):
         ktags.append(str(i))
```

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/nostr_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/nwc_tools.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/output_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/output_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,49 +186,49 @@
     alt_description = "This is a reaction to a NIP90 DVM AI task. "
 
     if status == "processing":
         if content is not None and content != "":
             alt_description = content
             reaction = alt_description
         else:
-            alt_description = "NIP90 DVM AI task " + task + " started processing. "
+            alt_description = "NIP90 DVM task " + task + " started processing. "
             reaction = alt_description + emoji.emojize(":thumbs_up:")
     elif status == "success":
-        alt_description = "NIP90 DVM AI task " + task + " finished successfully. "
+        alt_description = "NIP90 DVM task " + task + " finished successfully. "
         reaction = alt_description + emoji.emojize(":call_me_hand:")
     elif status == "chain-scheduled":
-        alt_description = "NIP90 DVM AI task " + task + " Chain Task scheduled"
+        alt_description = "NIP90 DVM task " + task + " Chain Task scheduled"
         reaction = alt_description + emoji.emojize(":thumbs_up:")
     elif status == "error":
-        alt_description = "NIP90 DVM AI task " + task + " had an error. "
+        alt_description = "NIP90 DVM task " + task + " had an error. "
         if content is None:
             reaction = alt_description + emoji.emojize(":thumbs_down:")
         else:
             reaction = alt_description + emoji.emojize(":thumbs_down:") + " " + content
 
     elif status == "payment-required":
-        alt_description = "NIP90 DVM AI task " + task + " requires payment of min " + str(
+        alt_description = "NIP90 DVM task " + task + " requires payment of min " + str(
             amount) + " Sats. "
         reaction = alt_description + emoji.emojize(":orange_heart:")
 
     elif status == "subscription-required":
         if content is not None and content != "":
             alt_description = content
             reaction = alt_description
 
         else:
-            alt_description = "NIP90 DVM AI task " + task + " requires payment for subscription"
+            alt_description = "NIP90 DVM task " + task + " requires payment for subscription"
             reaction = alt_description + emoji.emojize(":orange_heart:")
 
 
 
     elif status == "payment-rejected":
-        alt_description = "NIP90 DVM AI task " + task + " payment is below required amount of " + str(
+        alt_description = "NIP90 DVM task " + task + " payment is below required amount of " + str(
             amount) + " Sats. "
         reaction = alt_description + emoji.emojize(":thumbs_down:")
     elif status == "user-blocked-from-service":
-        alt_description = "NIP90 DVM AI task " + task + " can't be performed. User has been blocked from Service. "
+        alt_description = "NIP90 DVM task " + task + " can't be performed. User has been blocked from Service. "
         reaction = alt_description + emoji.emojize(":thumbs_down:")
     else:
         reaction = emoji.emojize(":thumbs_down:")
 
     return alt_description, reaction
```

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/subscription_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm/utils/zap_utils.py` & `nostr-dvm-0.3.2/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/nostr_dvm.egg-info/PKG-INFO` & `nostr-dvm-0.3.2/nostr_dvm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.1
+Version: 0.3.2
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr-dvm-0.3.1/nostr_dvm.egg-info/SOURCES.txt` & `nostr-dvm-0.3.2/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/setup.py` & `nostr-dvm-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. '
                     'This is an early stage release. Interfaces might change/brick')
 
 # Setting up
 setup(
     name="nostr-dvm",
```

### Comparing `nostr-dvm-0.3.1/tests/test_dvm_client.py` & `nostr-dvm-0.3.2/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.1/tests/test_events.py` & `nostr-dvm-0.3.2/tests/test_events.py`

 * *Files identical despite different names*

