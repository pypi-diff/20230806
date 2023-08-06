# Comparing `tmp/shortgpt-0.1.3.tar.gz` & `tmp/shortgpt-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortgpt-0.1.3.tar", last modified: Sat Aug  5 08:01:54 2023, max compression
+gzip compressed data, was "shortgpt-0.1.31.tar", last modified: Sun Aug  6 18:14:28 2023, max compression
```

## Comparing `shortgpt-0.1.3.tar` & `shortgpt-0.1.31.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.200000 shortgpt-0.1.3/
--rw-rw-rw-   0        0        0     2446 2023-07-28 20:38:40.000000 shortgpt-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    11354 2023-08-05 08:01:56.000000 shortgpt-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    10523 2023-08-04 05:22:42.000000 shortgpt-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 08:01:56.000000 shortgpt-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1734 2023-08-05 08:01:32.000000 shortgpt-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.340000 shortgpt-0.1.3/shortGPT/
--rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 shortgpt-0.1.3/shortGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.360000 shortgpt-0.1.3/shortGPT/api_utils/
--rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 shortgpt-0.1.3/shortGPT/api_utils/__init__.py
--rw-rw-rw-   0        0        0     2150 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/api_utils/eleven_api.py
--rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 shortgpt-0.1.3/shortGPT/api_utils/image_api.py
--rw-rw-rw-   0        0        0     2231 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/api_utils/pexels_api.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.390000 shortgpt-0.1.3/shortGPT/audio/
--rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 shortgpt-0.1.3/shortGPT/audio/__init__.py
--rw-rw-rw-   0        0        0     2684 2023-07-31 18:40:34.000000 shortgpt-0.1.3/shortGPT/audio/audio_duration.py
--rw-rw-rw-   0        0        0     3515 2023-07-31 18:40:34.000000 shortgpt-0.1.3/shortGPT/audio/audio_utils.py
--rw-rw-rw-   0        0        0     1874 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/audio/edge_voice_module.py
--rw-rw-rw-   0        0        0     1496 2023-08-05 06:24:20.000000 shortgpt-0.1.3/shortGPT/audio/eleven_voice_module.py
--rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 shortgpt-0.1.3/shortGPT/audio/voice_module.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.420000 shortgpt-0.1.3/shortGPT/config/
--rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 shortgpt-0.1.3/shortGPT/config/__init__.py
--rw-rw-rw-   0        0        0      715 2023-08-04 20:21:38.000000 shortgpt-0.1.3/shortGPT/config/api_db.py
--rw-rw-rw-   0        0        0    11721 2023-08-05 07:57:16.000000 shortgpt-0.1.3/shortGPT/config/asset_db.py
--rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 shortgpt-0.1.3/shortGPT/config/config.py
--rw-rw-rw-   0        0        0    11200 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/config/languages.py
--rw-rw-rw-   0        0        0     1144 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/config/path_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.440000 shortgpt-0.1.3/shortGPT/database/
--rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.3/shortGPT/database/__init__.py
--rw-rw-rw-   0        0        0      784 2023-07-31 18:40:34.000000 shortgpt-0.1.3/shortGPT/database/content_data_manager.py
--rw-rw-rw-   0        0        0     1167 2023-07-31 18:40:34.000000 shortgpt-0.1.3/shortGPT/database/content_database.py
--rw-rw-rw-   0        0        0     3914 2023-07-31 18:40:34.000000 shortgpt-0.1.3/shortGPT/database/db_document.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.460000 shortgpt-0.1.3/shortGPT/editing_framework/
--rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.3/shortGPT/editing_framework/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/core_editing_engine.py
--rw-rw-rw-   0        0        0    11160 2023-08-05 07:31:50.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_engine.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.480000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/
--rw-rw-rw-   0        0        0        0 2023-08-05 06:39:50.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/__init__.py
--rw-rw-rw-   0        0        0      374 2023-07-08 06:01:18.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/add_background_video.json
--rw-rw-rw-   0        0        0      289 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/add_background_voiceover.json
--rw-rw-rw-   0        0        0      182 2023-06-24 19:21:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/add_voiceover.json
--rw-rw-rw-   0        0        0      457 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/background_music.json
--rw-rw-rw-   0        0        0      553 2023-07-16 07:07:54.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json
--rw-rw-rw-   0        0        0      546 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/extract_audio.json
--rw-rw-rw-   0        0        0      350 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/insert_audio.json
--rw-rw-rw-   0        0        0      616 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption.json
--rw-rw-rw-   0        0        0      617 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption_arabic.json
--rw-rw-rw-   0        0        0      558 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json
--rw-rw-rw-   0        0        0      579 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption_landscape.json
--rw-rw-rw-   0        0        0      404 2023-06-26 06:51:40.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/show_reddit_image.json
--rw-rw-rw-   0        0        0      686 2023-06-24 02:50:20.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/show_top_image.json
--rw-rw-rw-   0        0        0      512 2023-06-24 20:04:38.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/show_watermark.json
--rw-rw-rw-   0        0        0      594 2023-08-05 07:58:02.000000 shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/subscribe_animation.json
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.500000 shortgpt-0.1.3/shortGPT/editing_framework/flows/
--rw-rw-rw-   0        0        0        0 2023-08-05 06:39:56.000000 shortgpt-0.1.3/shortGPT/editing_framework/flows/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-07-03 07:06:58.000000 shortgpt-0.1.3/shortGPT/editing_framework/flows/build_reddit_image.json
--rw-rw-rw-   0        0        0     1107 2023-07-11 20:20:30.000000 shortgpt-0.1.3/shortGPT/editing_framework/rendering_logger.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.520000 shortgpt-0.1.3/shortGPT/editing_utils/
--rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 shortgpt-0.1.3/shortGPT/editing_utils/__init__.py
--rw-rw-rw-   0        0        0     2455 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_utils/captions.py
--rw-rw-rw-   0        0        0      781 2023-07-11 20:20:28.000000 shortgpt-0.1.3/shortGPT/editing_utils/editing_images.py
--rw-rw-rw-   0        0        0     3423 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/editing_utils/handle_videos.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.650000 shortgpt-0.1.3/shortGPT/engine/
--rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 shortgpt-0.1.3/shortGPT/engine/__init__.py
--rw-rw-rw-   0        0        0     4180 2023-08-05 07:55:40.000000 shortgpt-0.1.3/shortGPT/engine/abstract_content_engine.py
--rw-rw-rw-   0        0        0     8437 2023-08-05 07:58:38.000000 shortgpt-0.1.3/shortGPT/engine/content_short_engine.py
--rw-rw-rw-   0        0        0     7884 2023-08-05 07:01:08.000000 shortgpt-0.1.3/shortGPT/engine/content_translation_engine.py
--rw-rw-rw-   0        0        0     7854 2023-08-05 07:01:14.000000 shortgpt-0.1.3/shortGPT/engine/content_video_engine.py
--rw-rw-rw-   0        0        0     1023 2023-07-29 19:03:56.000000 shortgpt-0.1.3/shortGPT/engine/facts_short_engine.py
--rw-rw-rw-   0        0        0     8336 2023-08-05 07:01:20.000000 shortgpt-0.1.3/shortGPT/engine/multi_language_translation_engine.py
--rw-rw-rw-   0        0        0     5897 2023-08-05 07:58:54.000000 shortgpt-0.1.3/shortGPT/engine/reddit_short_engine.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.690000 shortgpt-0.1.3/shortGPT/gpt/
--rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 shortgpt-0.1.3/shortGPT/gpt/__init__.py
--rw-rw-rw-   0        0        0      915 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/facts_gpt.py
--rw-rw-rw-   0        0        0     1269 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/gpt_chat_video.py
--rw-rw-rw-   0        0        0     1782 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/gpt_editing.py
--rw-rw-rw-   0        0        0      513 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/gpt_translate.py
--rw-rw-rw-   0        0        0     3638 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/gpt_utils.py
--rw-rw-rw-   0        0        0      386 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/gpt_voice.py
--rw-rw-rw-   0        0        0      803 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/gpt_yt.py
--rw-rw-rw-   0        0        0     2240 2023-08-05 07:22:12.000000 shortgpt-0.1.3/shortGPT/gpt/reddit_gpt.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.710000 shortgpt-0.1.3/shortGPT/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-08-05 06:34:46.000000 shortgpt-0.1.3/shortGPT/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      970 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/chat_video_edit_script.yaml
--rw-rw-rw-   0        0        0      918 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/chat_video_script.yaml
--rw-rw-rw-   0        0        0     3199 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/editing_generate_images.yaml
--rw-rw-rw-   0        0        0     1897 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/editing_generate_videos.yaml
--rw-rw-rw-   0        0        0     1629 2023-07-07 17:47:06.000000 shortgpt-0.1.3/shortGPT/prompt_templates/facts_generator.yaml
--rw-rw-rw-   0        0        0      342 2023-07-07 17:46:48.000000 shortgpt-0.1.3/shortGPT/prompt_templates/facts_subjects_generation.yaml
--rw-rw-rw-   0        0        0     1910 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/reddit_extract_question.yaml
--rw-rw-rw-   0        0        0      722 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/reddit_filter_realistic.yaml
--rw-rw-rw-   0        0        0     1657 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/reddit_generate_question.yaml
--rw-rw-rw-   0        0        0     1604 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/reddit_generate_script.yaml
--rw-rw-rw-   0        0        0     1160 2023-06-29 23:38:32.000000 shortgpt-0.1.3/shortGPT/prompt_templates/reddit_story_filter.yaml
--rw-rw-rw-   0        0        0      245 2023-07-07 06:42:50.000000 shortgpt-0.1.3/shortGPT/prompt_templates/reddit_username.yaml
--rw-rw-rw-   0        0        0      757 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/translate_content.yaml
--rw-rw-rw-   0        0        0      356 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/voice_identify_gender.yaml
--rw-rw-rw-   0        0        0      814 2023-07-28 20:38:42.000000 shortgpt-0.1.3/shortGPT/prompt_templates/yt_title_description.yaml
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.730000 shortgpt-0.1.3/shortGPT/tracking/
--rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 shortgpt-0.1.3/shortGPT/tracking/__init__.py
--rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 shortgpt-0.1.3/shortGPT/tracking/api_tracking.py
--rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 shortgpt-0.1.3/shortGPT/tracking/cost_analytics.py
-drwxrwxrwx   0        0        0        0 2023-08-05 08:01:52.860000 shortgpt-0.1.3/shortgpt.egg-info/
--rw-rw-rw-   0        0        0    11354 2023-08-05 08:01:52.000000 shortgpt-0.1.3/shortgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2023-08-05 08:01:54.000000 shortgpt-0.1.3/shortgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 08:01:52.000000 shortgpt-0.1.3/shortgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2023-08-05 08:01:52.000000 shortgpt-0.1.3/shortgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 08:01:52.000000 shortgpt-0.1.3/shortgpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.440000 shortgpt-0.1.31/
+-rw-rw-rw-   0        0        0     2446 2023-07-28 20:38:40.000000 shortgpt-0.1.31/LICENSE
+-rw-rw-rw-   0        0        0    10415 2023-08-06 18:14:30.000000 shortgpt-0.1.31/PKG-INFO
+-rw-rw-rw-   0        0        0     9616 2023-08-06 18:11:22.000000 shortgpt-0.1.31/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 18:14:30.000000 shortgpt-0.1.31/setup.cfg
+-rw-rw-rw-   0        0        0     1735 2023-08-06 18:13:06.000000 shortgpt-0.1.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.520000 shortgpt-0.1.31/shortGPT/
+-rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 shortgpt-0.1.31/shortGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.550000 shortgpt-0.1.31/shortGPT/api_utils/
+-rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 shortgpt-0.1.31/shortGPT/api_utils/__init__.py
+-rw-rw-rw-   0        0        0     2150 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/api_utils/eleven_api.py
+-rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 shortgpt-0.1.31/shortGPT/api_utils/image_api.py
+-rw-rw-rw-   0        0        0     2231 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/api_utils/pexels_api.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.570000 shortgpt-0.1.31/shortGPT/audio/
+-rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 shortgpt-0.1.31/shortGPT/audio/__init__.py
+-rw-rw-rw-   0        0        0     2684 2023-07-31 18:40:34.000000 shortgpt-0.1.31/shortGPT/audio/audio_duration.py
+-rw-rw-rw-   0        0        0     3515 2023-07-31 18:40:34.000000 shortgpt-0.1.31/shortGPT/audio/audio_utils.py
+-rw-rw-rw-   0        0        0     1874 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/audio/edge_voice_module.py
+-rw-rw-rw-   0        0        0     1496 2023-08-05 06:24:20.000000 shortgpt-0.1.31/shortGPT/audio/eleven_voice_module.py
+-rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 shortgpt-0.1.31/shortGPT/audio/voice_module.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.590000 shortgpt-0.1.31/shortGPT/config/
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 shortgpt-0.1.31/shortGPT/config/__init__.py
+-rw-rw-rw-   0        0        0      715 2023-08-04 20:21:38.000000 shortgpt-0.1.31/shortGPT/config/api_db.py
+-rw-rw-rw-   0        0        0    11832 2023-08-06 18:10:46.000000 shortgpt-0.1.31/shortGPT/config/asset_db.py
+-rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 shortgpt-0.1.31/shortGPT/config/config.py
+-rw-rw-rw-   0        0        0    11200 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/config/languages.py
+-rw-rw-rw-   0        0        0     1144 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/config/path_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.610000 shortgpt-0.1.31/shortGPT/database/
+-rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.31/shortGPT/database/__init__.py
+-rw-rw-rw-   0        0        0      784 2023-07-31 18:40:34.000000 shortgpt-0.1.31/shortGPT/database/content_data_manager.py
+-rw-rw-rw-   0        0        0     1167 2023-07-31 18:40:34.000000 shortgpt-0.1.31/shortGPT/database/content_database.py
+-rw-rw-rw-   0        0        0     3914 2023-07-31 18:40:34.000000 shortgpt-0.1.31/shortGPT/database/db_document.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.640000 shortgpt-0.1.31/shortGPT/editing_framework/
+-rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.31/shortGPT/editing_framework/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/core_editing_engine.py
+-rw-rw-rw-   0        0        0    11160 2023-08-05 07:31:50.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_engine.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.660000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:39:50.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-07-08 06:01:18.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/add_background_video.json
+-rw-rw-rw-   0        0        0      289 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/add_background_voiceover.json
+-rw-rw-rw-   0        0        0      182 2023-06-24 19:21:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/add_voiceover.json
+-rw-rw-rw-   0        0        0      457 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/background_music.json
+-rw-rw-rw-   0        0        0      553 2023-07-16 07:07:54.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json
+-rw-rw-rw-   0        0        0      546 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/extract_audio.json
+-rw-rw-rw-   0        0        0      350 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/insert_audio.json
+-rw-rw-rw-   0        0        0      616 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption.json
+-rw-rw-rw-   0        0        0      617 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption_arabic.json
+-rw-rw-rw-   0        0        0      558 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json
+-rw-rw-rw-   0        0        0      579 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption_landscape.json
+-rw-rw-rw-   0        0        0      404 2023-06-26 06:51:40.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/show_reddit_image.json
+-rw-rw-rw-   0        0        0      686 2023-06-24 02:50:20.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/show_top_image.json
+-rw-rw-rw-   0        0        0      512 2023-06-24 20:04:38.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/show_watermark.json
+-rw-rw-rw-   0        0        0      594 2023-08-05 07:58:02.000000 shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/subscribe_animation.json
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.690000 shortgpt-0.1.31/shortGPT/editing_framework/flows/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:39:56.000000 shortgpt-0.1.31/shortGPT/editing_framework/flows/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-07-03 07:06:58.000000 shortgpt-0.1.31/shortGPT/editing_framework/flows/build_reddit_image.json
+-rw-rw-rw-   0        0        0     1107 2023-07-11 20:20:30.000000 shortgpt-0.1.31/shortGPT/editing_framework/rendering_logger.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.720000 shortgpt-0.1.31/shortGPT/editing_utils/
+-rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 shortgpt-0.1.31/shortGPT/editing_utils/__init__.py
+-rw-rw-rw-   0        0        0     2455 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_utils/captions.py
+-rw-rw-rw-   0        0        0      781 2023-07-11 20:20:28.000000 shortgpt-0.1.31/shortGPT/editing_utils/editing_images.py
+-rw-rw-rw-   0        0        0     3423 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/editing_utils/handle_videos.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.740000 shortgpt-0.1.31/shortGPT/engine/
+-rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 shortgpt-0.1.31/shortGPT/engine/__init__.py
+-rw-rw-rw-   0        0        0     4180 2023-08-05 07:55:40.000000 shortgpt-0.1.31/shortGPT/engine/abstract_content_engine.py
+-rw-rw-rw-   0        0        0     8513 2023-08-05 08:18:00.000000 shortgpt-0.1.31/shortGPT/engine/content_short_engine.py
+-rw-rw-rw-   0        0        0     7884 2023-08-05 07:01:08.000000 shortgpt-0.1.31/shortGPT/engine/content_translation_engine.py
+-rw-rw-rw-   0        0        0     7930 2023-08-05 08:18:04.000000 shortgpt-0.1.31/shortGPT/engine/content_video_engine.py
+-rw-rw-rw-   0        0        0     1023 2023-07-29 19:03:56.000000 shortgpt-0.1.31/shortGPT/engine/facts_short_engine.py
+-rw-rw-rw-   0        0        0     8336 2023-08-05 07:01:20.000000 shortgpt-0.1.31/shortGPT/engine/multi_language_translation_engine.py
+-rw-rw-rw-   0        0        0     5897 2023-08-05 07:58:54.000000 shortgpt-0.1.31/shortGPT/engine/reddit_short_engine.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.770000 shortgpt-0.1.31/shortGPT/gpt/
+-rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 shortgpt-0.1.31/shortGPT/gpt/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/facts_gpt.py
+-rw-rw-rw-   0        0        0     1269 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/gpt_chat_video.py
+-rw-rw-rw-   0        0        0     1782 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/gpt_editing.py
+-rw-rw-rw-   0        0        0      513 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/gpt_translate.py
+-rw-rw-rw-   0        0        0     3638 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/gpt_utils.py
+-rw-rw-rw-   0        0        0      386 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/gpt_voice.py
+-rw-rw-rw-   0        0        0      803 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/gpt_yt.py
+-rw-rw-rw-   0        0        0     2240 2023-08-05 07:22:12.000000 shortgpt-0.1.31/shortGPT/gpt/reddit_gpt.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.790000 shortgpt-0.1.31/shortGPT/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:34:46.000000 shortgpt-0.1.31/shortGPT/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      970 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/chat_video_edit_script.yaml
+-rw-rw-rw-   0        0        0      918 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/chat_video_script.yaml
+-rw-rw-rw-   0        0        0     3199 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/editing_generate_images.yaml
+-rw-rw-rw-   0        0        0     1897 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/editing_generate_videos.yaml
+-rw-rw-rw-   0        0        0     1629 2023-07-07 17:47:06.000000 shortgpt-0.1.31/shortGPT/prompt_templates/facts_generator.yaml
+-rw-rw-rw-   0        0        0      342 2023-07-07 17:46:48.000000 shortgpt-0.1.31/shortGPT/prompt_templates/facts_subjects_generation.yaml
+-rw-rw-rw-   0        0        0     1910 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/reddit_extract_question.yaml
+-rw-rw-rw-   0        0        0      722 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/reddit_filter_realistic.yaml
+-rw-rw-rw-   0        0        0     1657 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/reddit_generate_question.yaml
+-rw-rw-rw-   0        0        0     1604 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/reddit_generate_script.yaml
+-rw-rw-rw-   0        0        0     1160 2023-06-29 23:38:32.000000 shortgpt-0.1.31/shortGPT/prompt_templates/reddit_story_filter.yaml
+-rw-rw-rw-   0        0        0      245 2023-07-07 06:42:50.000000 shortgpt-0.1.31/shortGPT/prompt_templates/reddit_username.yaml
+-rw-rw-rw-   0        0        0      757 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/translate_content.yaml
+-rw-rw-rw-   0        0        0      356 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/voice_identify_gender.yaml
+-rw-rw-rw-   0        0        0      814 2023-07-28 20:38:42.000000 shortgpt-0.1.31/shortGPT/prompt_templates/yt_title_description.yaml
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.810000 shortgpt-0.1.31/shortGPT/tracking/
+-rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 shortgpt-0.1.31/shortGPT/tracking/__init__.py
+-rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 shortgpt-0.1.31/shortGPT/tracking/api_tracking.py
+-rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 shortgpt-0.1.31/shortGPT/tracking/cost_analytics.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:14:26.830000 shortgpt-0.1.31/shortgpt.egg-info/
+-rw-rw-rw-   0        0        0    10415 2023-08-06 18:14:28.000000 shortgpt-0.1.31/shortgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2023-08-06 18:14:28.000000 shortgpt-0.1.31/shortgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 18:14:28.000000 shortgpt-0.1.31/shortgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-08-06 18:14:28.000000 shortgpt-0.1.31/shortgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 18:14:28.000000 shortgpt-0.1.31/shortgpt.egg-info/top_level.txt
```

### Comparing `shortgpt-0.1.3/LICENSE` & `shortgpt-0.1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/PKG-INFO` & `shortgpt-0.1.31/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortgpt
-Version: 0.1.3
+Version: 0.1.31
 Summary: Automating video and short content creation with AI
 Author: RayVentura
 Author-email: 
 Keywords: python,video,content creation,AI,automation,editing,voiceover synthesis,video captions,asset sourcing,tinyDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,30 +12,48 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # 🚀🎬 ShortGPT
-[![](https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ)
-[![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/shortgpt)
-<div align="center">
-    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
+<p align="center">
+  <a href="https://discord.gg/uERx39ru3R">
+    <img src="https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat">
+  </a>
+  <a href="https://twitter.com/RayVenturaHQ">
+    <img src="https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura">
+  </a>
+  <a href="https://star-history.com/#rayventura/shortgpt)">
+    <img src="https://img.shields.io/github/stars/rayventura/shortgpt?style=social">
+  </a>
+  <a href="https://pypi.org/project/shortgpt/">
+    <img src="https://static.pepy.tech/personalized-badge/shortgpt?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads/month">
+  </a>
+  <a href="https://docs.shortgpt.ai/">
+    <img src="https://img.shields.io/badge/docs-visit-blue">
+  </a>  
+</p>
+
+<div align="center" style="border-radius: 20px;" width="18%">
+    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="18%"/>
 </div>
 <div align="center">
   <a href="https://discord.gg/uERx39ru3R">
-    <img src="https://img.shields.io/badge/discord-join%20chat-blue.svg" alt="Join our Discord" height="34">
+    <img src="https://img.shields.io/discord/1126042224979886160?color=7289da&logo=discord&logoColor=blue&labelColor=white&color=cyan" alt="Join our Discord" height="34">
   </a>
 </div>
 
 <div align="center">
 ⚡ Automating video and short content creation with AI ⚡
 </div>
+</br>
 
+If you're only interested in using ShortGPT programatically (pip library), go on [the documentation website](https://docs.shortgpt.ai/docs/how-to-install).
+Otherwise, follow the installation steps below for running the web app locally. 
 ## 🎥 Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U))
 
 https://github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-6365c27ea5fe
 ## 🎥 Voice Dubbing
 
 
 https://github.com/RayVentura/ShortGPT/assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef
@@ -49,15 +67,15 @@
 ## 📝 Introduction to ShortGPT 
 ShortGPT is a powerful framework for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
 
 - 🎞️ **Automated editing framework**: Streamlines the video creation process with an LLM oriented video editing language.
 
 - 📃 **Scripts and Prompts**: Provides ready-to-use scripts and prompts for various LLM automated editing processes.
 
-- 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, and Portuguese 🇵🇹.
+- 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, Portuguese 🇵🇹, Russian 🇷🇺, Mandarin Chinese 🇨🇳, Japanese 🇯🇵, Hindi 🇮🇳,Korean 🇰🇷, and way over 30 more languages (with EdgeTTS)
 
 - 🔗 **Caption Generation**: Automates the generation of video captions.
 
 - 🌐🎥 **Asset Sourcing**: Sources images and video footage from the internet, connecting with the web and Pexels API as necessary.
 
 - 🧠 **Memory and persistency**: Ensures long-term persistency of automated editing variables with TinyDB.
 
@@ -68,64 +86,21 @@
 1. Click on the link to the Google Colab notebook: [https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
 2. Once you're in the notebook, simply run the cells in order from top to bottom. You can do this by clicking on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy using ShortGPT!
 
 # Instructions for running shortGPT
 This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
 
-## Prerequisites
-Before you begin, ensure that you have the following prerequisites installed on your system:
-- Python 3.x
-- Pip (Python package installer)
+
 
 ## Installation Steps
 Follow the instructions below to install ImageMagick, FFmpeg, and clone the shortGPT repository:
 
-### Step 1: Install ImageMagick
-1. For `Windows` download the installer from the official ImageMagick website and follow the installation instructions.
-      
-      [https://imagemagick.org/script/download.php](https://imagemagick.org/script/download.php)
-          
-2. For Ubuntu/Debian-based systems, use the command:
-     ```
-     sudo apt-get install imagemagick
-     ```
-     Then run the following command to fix a moviepy Imagemagick policy.xml incompatibility problem:
-     ```
-     !sed -i '/<policy domain="path" rights="none" pattern="@\*"/d' /etc/ImageMagick-6/policy.xml
-     ```    
-4. For macOS using Homebrew, use the command:
-     ```
-     brew install imagemagick
-     ```
-2. Verify the installation by running the following command:
-   ```
-   convert --version
-   ```
-   You should see the ImageMagick version information if the installation was successful.
-
-### Step 2: Install FFmpeg (REQUIRED FOR SHORTGPT TO WORK)
-1. For `Windows`Download the FFmpeg binaries from this Windows Installer (It will download ffmpeg, ffprobe and add it to your path).
-      
-      [https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306)
-      
-2. For macOS using Homebrew, use the command:
-     ```
-     brew install ffmpeg
-     ```   
-    For Ubuntu/Debian-based systems, use the command:
-     ```
-     sudo apt-get install ffmpeg
-     ```
-2. Verify the installation by running the following command:
-   ```
-   ffmpeg -version
-   ```
-   You should see the FFmpeg version information if the installation was successful.
-
+### Step 1 and 2, install Ffmpeg and ImageMagick
+For the updated installation steps, please follow Step 1 and 2 in our official documentation [docs.shortgpt.ai/docs/how-to-install](https://docs.shortgpt.ai/docs/how-to-install).
 ### Step 3: Clone the shortGPT Repository
 
 1. Open a terminal or command prompt.
 2. Execute the following command to clone the shortGPT repository:
    ```
    git clone https://github.com/rayventura/shortgpt.git
    ```
@@ -149,32 +124,22 @@
 2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to run the script:
    ```
    python runShortGPT.py
    ```
 4. After running the script, a Gradio interface should open at your local host on port 31415 (http://localhost:31415). 
 
-## Putting API Keys
-The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for running short automations. For video automations, you will also need to add a Pexels API.
-
-Follow these steps to add your OpenAI and ElevenLabs API keys:
-
-1. Open [http://localhost:31415/?__theme=light](http://localhost:31415/?__theme=light) from a web browser. 
-2. Click on the `config` tab located at the left side bar of the user interface.
-3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the corresponding input fields.
-4. Click `Save` to save your API keys.
-
-That's it! You have successfully set up your API keys and can now utilize the functionality of ShortGPT in the Gradio interface.
-
 ## Framework overview
 
 - 🎬 The `ContentShortEngine` is designed for creating shorts, handling tasks from script generation to final rendering, including adding YouTube metadata.
 
 - 🎥 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like generating audio, automatically sourcing background video footage, timing captions, and preparing background assets.
-  
+
+- 🗣️ The `ContentTranslationEngine` is designed to dub and translate entire videos, from mainstream languages to more specific target languages. It takes a video file, or youtube link, transcribe it's audio, translates the content, voices it in a target language, adds captions , and gives back a new video, in a totally different language.
+
 - 🎞️ The automated `EditingEngine`, using Editing Markup Language and JSON, breaks down the editing process into manageable and customizable blocks, comprehensible to Large Language Models.
 
 💡 ShortGPT offers customization options to suit your needs, from language selection to watermark addition.
 
 🔧 As a framework, ShortGPT is adaptable and flexible, offering the potential for efficient, creative content creation.
 
 More documentation incomming, please be patient.
@@ -186,14 +151,16 @@
 
 - **Moviepy**: Moviepy is used for video editing, allowing ShortGPT to make video editing and rendering
 
 - **Openai**: Openai is used for automating the entire process, including generating scripts and prompts for LLM automated editing processes.
 
 - **ElevenLabs**: ElevenLabs is used for voice synthesis, supporting multiple languages for voiceover creation.
 
+- **EdgeTTS**: Microsoft's FREE EdgeTTS is used for voice synthesis, supporting way many more language than ElevenLabs currently.
+
 - **Pexels**: Pexels is used for sourcing background footage, allowing ShortGPT to connect with the web and access a wide range of images and videos.
 
 - **Bing Image**: Bing Image is used for sourcing images, providing a comprehensive database for ShortGPT to retrieve relevant visuals.
 
 These technologies work together to provide a seamless and efficient experience in automating video and short content creation with AI.
 
 ## 💁 Contributing
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
-Metadata-Version: 2.1 Name: shortgpt Version: 0.1.3 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.1.31 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
-LICENSE # ðð¬ ShortGPT [![](https://dcbadge.vercel.app/api/server/
-uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R) [![Twitter]
-(https://img.shields.io/twitter/url/https/twitter.com/
-rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://
-twitter.com/RayVenturaHQ) [![GitHub star chart](https://img.shields.io/github/
-stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
-shortgpt)
+LICENSE # ðð¬ ShortGPT
+  [https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat]
+            [https://img.shields.io/twitter/url/https/twitter.com/
+     rayventurahq.svg?style=social&label=Follow%20%40RayVentura] [https://
+    img.shields.io/github/stars/rayventura/shortgpt?style=social] [https://
+                     static.pepy.tech/personalized-badge/
+shortgpt?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads/
+             month] [https://img.shields.io/badge/docs-visit-blue]
                                 [ShortGPT-logo]
                               [Join_our_Discord]
           â¡ Automating video and short content creation with AI â¡
+ If you're only interested in using ShortGPT programatically (pip library), go
+on [the documentation website](https://docs.shortgpt.ai/docs/how-to-install).
+Otherwise, follow the installation steps below for running the web app locally.
 ## ð¥ Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U)) https:
 //github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-
 6365c27ea5fe ## ð¥ Voice Dubbing https://github.com/RayVentura/ShortGPT/
 assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef ## ð Show Your Support
 We hope you find ShortGPT helpful! If you do, let us know by giving us a star
 â­ on the repo. It's easy, just click on the 'Star' button at the top right of
 the page. Your support means a lot to us and keeps us motivated to improve and
@@ -31,107 +35,87 @@
 powerful framework for automating content creation. It simplifies video
 creation, footage sourcing, voiceover synthesis, and editing tasks. - ðï¸
 **Automated editing framework**: Streamlines the video creation process with an
 LLM oriented video editing language. - ð **Scripts and Prompts**: Provides
 ready-to-use scripts and prompts for various LLM automated editing processes. -
 ð£ï¸ **Voiceover / Content Creation**: Supports multiple languages including
 English ðºð¸, Spanish ðªð¸, Arabic ð¦ðª, French ð«ð·, Polish
-ðµð±, German ð©ðª, Italian ð®ð¹, and Portuguese ðµð¹. - ð
-**Caption Generation**: Automates the generation of video captions. - ðð¥
-**Asset Sourcing**: Sources images and video footage from the internet,
-connecting with the web and Pexels API as necessary. - ð§  **Memory and
-persistency**: Ensures long-term persistency of automated editing variables
-with TinyDB. ## ð Quick Start: Run ShortGPT on Google Colab (https://
+ðµð±, German ð©ðª, Italian ð®ð¹, Portuguese ðµð¹, Russian
+ð·ðº, Mandarin Chinese ð¨ð³, Japanese ð¯ðµ, Hindi ð®ð³,Korean
+ð°ð·, and way over 30 more languages (with EdgeTTS) - ð **Caption
+Generation**: Automates the generation of video captions. - ðð¥ **Asset
+Sourcing**: Sources images and video footage from the internet, connecting with
+the web and Pexels API as necessary. - ð§  **Memory and persistency**: Ensures
+long-term persistency of automated editing variables with TinyDB. ## ð Quick
+Start: Run ShortGPT on Google Colab (https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) If you prefer not to install the
+prerequisites on your local system, you can use the Google Colab notebook. This
+option is free and requires no installation setup. 1. Click on the link to the
+Google Colab notebook: [https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://
 colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
-If you prefer not to install the prerequisites on your local system, you can
-use the Google Colab notebook. This option is free and requires no installation
-setup. 1. Click on the link to the Google Colab notebook: [https://
-colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing]
-(https://colab.research.google.com/drive/
-1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) 2. Once you're in the notebook,
-simply run the cells in order from top to bottom. You can do this by clicking
-on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy
-using ShortGPT! # Instructions for running shortGPT This guide provides step-
-by-step instructions for installing ImageMagick and FFmpeg on your system,
-which are both required to do automated editing. Once installed, you can
-proceed to run `runShortGPT.py` successfully. ## Prerequisites Before you
-begin, ensure that you have the following prerequisites installed on your
-system: - Python 3.x - Pip (Python package installer) ## Installation Steps
-Follow the instructions below to install ImageMagick, FFmpeg, and clone the
-shortGPT repository: ### Step 1: Install ImageMagick 1. For `Windows` download
-the installer from the official ImageMagick website and follow the installation
-instructions. [https://imagemagick.org/script/download.php](https://
-imagemagick.org/script/download.php) 2. For Ubuntu/Debian-based systems, use
-the command: ``` sudo apt-get install imagemagick ``` Then run the following
-command to fix a moviepy Imagemagick policy.xml incompatibility problem: ```
-!sed -i '/
-' /etc/ImageMagick-6/policy.xml ``` 4. For macOS using Homebrew, use the
-command: ``` brew install imagemagick ``` 2. Verify the installation by running
-the following command: ``` convert --version ``` You should see the ImageMagick
-version information if the installation was successful. ### Step 2: Install
-FFmpeg (REQUIRED FOR SHORTGPT TO WORK) 1. For `Windows`Download the FFmpeg
-binaries from this Windows Installer (It will download ffmpeg, ffprobe and add
-it to your path). [https://github.com/icedterminal/ffmpeg-installer/releases/
-tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/
-tag/6.0.0.20230306) 2. For macOS using Homebrew, use the command: ``` brew
-install ffmpeg ``` For Ubuntu/Debian-based systems, use the command: ``` sudo
-apt-get install ffmpeg ``` 2. Verify the installation by running the following
-command: ``` ffmpeg -version ``` You should see the FFmpeg version information
-if the installation was successful. ### Step 3: Clone the shortGPT Repository
-1. Open a terminal or command prompt. 2. Execute the following command to clone
-the shortGPT repository: ``` git clone https://github.com/rayventura/
-shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a terminal or
-command prompt. 2. Navigate to the directory where `runShortGPT.py` is located
-(the cloned repo). 3. Execute the following command to install the required
-Python dependencies: ``` pip install -r requirements.txt ``` This command will
-install the necessary packages specified in the `requirements.txt` file. ##
-Running runShortGPT.py Web Interface Once you have successfully installed
-ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py`
-by following these steps: 1. Open a terminal or command prompt. 2. Navigate to
-the directory where `runShortGPT.py` is located (the cloned repo). 3. Execute
-the following command to run the script: ``` python runShortGPT.py ``` 4. After
-running the script, a Gradio interface should open at your local host on port
-31415 (http://localhost:31415). ## Putting API Keys The ShortGPT UI needs you
-to input at least OpenAI and ElevenLabs api keys for running short automations.
-For video automations, you will also need to add a Pexels API. Follow these
-steps to add your OpenAI and ElevenLabs API keys: 1. Open [http://localhost:
-31415/?__theme=light](http://localhost:31415/?__theme=light) from a web
-browser. 2. Click on the `config` tab located at the left side bar of the user
-interface. 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the
-corresponding input fields. 4. Click `Save` to save your API keys. That's it!
-You have successfully set up your API keys and can now utilize the
-functionality of ShortGPT in the Gradio interface. ## Framework overview - ð¬
-The `ContentShortEngine` is designed for creating shorts, handling tasks from
-script generation to final rendering, including adding YouTube metadata. - ð¥
-The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like
-generating audio, automatically sourcing background video footage, timing
-captions, and preparing background assets. - ðï¸ The automated
-`EditingEngine`, using Editing Markup Language and JSON, breaks down the
-editing process into manageable and customizable blocks, comprehensible to
-Large Language Models. ð¡ ShortGPT offers customization options to suit your
-needs, from language selection to watermark addition. ð§ As a framework,
-ShortGPT is adaptable and flexible, offering the potential for efficient,
-creative content creation. More documentation incomming, please be patient. ##
-Technologies Used ShortGPT utilizes the following technologies to power its
-functionality: - **Moviepy**: Moviepy is used for video editing, allowing
-ShortGPT to make video editing and rendering - **Openai**: Openai is used for
-automating the entire process, including generating scripts and prompts for LLM
-automated editing processes. - **ElevenLabs**: ElevenLabs is used for voice
-synthesis, supporting multiple languages for voiceover creation. - **Pexels**:
-Pexels is used for sourcing background footage, allowing ShortGPT to connect
-with the web and access a wide range of images and videos. - **Bing Image**:
-Bing Image is used for sourcing images, providing a comprehensive database for
-ShortGPT to retrieve relevant visuals. These technologies work together to
-provide a seamless and efficient experience in automating video and short
-content creation with AI. ## ð Contributing As an open-source project in a
-rapidly developing field, we are extremely open to contributions, whether it
-would be in the form of a new feature, improved infrastructure, or better
-documentation. ## ð Get in touch on Twitter ð¦ Keep up with the latest
-happenings, announcements, and insights about Short-GPT by checking out our
-Twitter accounts. Spark a conversation with our developer and the AI's own
-account for fascinating dialogues, latest news about the project, and more. -
-**Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ).
-Deep-dive into behind-the-scenes, project news, and related topics from the
-person behind ShortGPT. We're eager to interact with you and listen to your
-feedback, concepts, and experiences with Short-GPT. Come on board on Twitter
-and let's navigate the future of AI as a team! ð¡ð¤
+2. Once you're in the notebook, simply run the cells in order from top to
+bottom. You can do this by clicking on each cell and pressing the 'Play'
+button, or by using the keyboard . Enjoy using ShortGPT! # Instructions for
+running shortGPT This guide provides step-by-step instructions for installing
+ImageMagick and FFmpeg on your system, which are both required to do automated
+editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
+## Installation Steps Follow the instructions below to install ImageMagick,
+FFmpeg, and clone the shortGPT repository: ### Step 1 and 2, install Ffmpeg and
+ImageMagick For the updated installation steps, please follow Step 1 and 2 in
+our official documentation [docs.shortgpt.ai/docs/how-to-install](https://
+docs.shortgpt.ai/docs/how-to-install). ### Step 3: Clone the shortGPT
+Repository 1. Open a terminal or command prompt. 2. Execute the following
+command to clone the shortGPT repository: ``` git clone https://github.com/
+rayventura/shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a
+terminal or command prompt. 2. Navigate to the directory where `runShortGPT.py`
+is located (the cloned repo). 3. Execute the following command to install the
+required Python dependencies: ``` pip install -r requirements.txt ``` This
+command will install the necessary packages specified in the `requirements.txt`
+file. ## Running runShortGPT.py Web Interface Once you have successfully
+installed ImageMagick, FFmpeg, and the Python dependencies, you can run
+`runShortGPT.py` by following these steps: 1. Open a terminal or command
+prompt. 2. Navigate to the directory where `runShortGPT.py` is located (the
+cloned repo). 3. Execute the following command to run the script: ``` python
+runShortGPT.py ``` 4. After running the script, a Gradio interface should open
+at your local host on port 31415 (http://localhost:31415). ## Framework
+overview - ð¬ The `ContentShortEngine` is designed for creating shorts,
+handling tasks from script generation to final rendering, including adding
+YouTube metadata. - ð¥ The `ContentVideoEngine` is ideal for longer videos,
+taking care of tasks like generating audio, automatically sourcing background
+video footage, timing captions, and preparing background assets. - ð£ï¸ The
+`ContentTranslationEngine` is designed to dub and translate entire videos, from
+mainstream languages to more specific target languages. It takes a video file,
+or youtube link, transcribe it's audio, translates the content, voices it in a
+target language, adds captions , and gives back a new video, in a totally
+different language. - ðï¸ The automated `EditingEngine`, using Editing
+Markup Language and JSON, breaks down the editing process into manageable and
+customizable blocks, comprehensible to Large Language Models. ð¡ ShortGPT
+offers customization options to suit your needs, from language selection to
+watermark addition. ð§ As a framework, ShortGPT is adaptable and flexible,
+offering the potential for efficient, creative content creation. More
+documentation incomming, please be patient. ## Technologies Used ShortGPT
+utilizes the following technologies to power its functionality: - **Moviepy**:
+Moviepy is used for video editing, allowing ShortGPT to make video editing and
+rendering - **Openai**: Openai is used for automating the entire process,
+including generating scripts and prompts for LLM automated editing processes. -
+**ElevenLabs**: ElevenLabs is used for voice synthesis, supporting multiple
+languages for voiceover creation. - **EdgeTTS**: Microsoft's FREE EdgeTTS is
+used for voice synthesis, supporting way many more language than ElevenLabs
+currently. - **Pexels**: Pexels is used for sourcing background footage,
+allowing ShortGPT to connect with the web and access a wide range of images and
+videos. - **Bing Image**: Bing Image is used for sourcing images, providing a
+comprehensive database for ShortGPT to retrieve relevant visuals. These
+technologies work together to provide a seamless and efficient experience in
+automating video and short content creation with AI. ## ð Contributing As an
+open-source project in a rapidly developing field, we are extremely open to
+contributions, whether it would be in the form of a new feature, improved
+infrastructure, or better documentation. ## ð Get in touch on Twitter ð¦
+Keep up with the latest happenings, announcements, and insights about Short-GPT
+by checking out our Twitter accounts. Spark a conversation with our developer
+and the AI's own account for fascinating dialogues, latest news about the
+project, and more. - **Developer**: Stay updated [@RayVentura](https://
+twitter.com/RayVenturaHQ). Deep-dive into behind-the-scenes, project news, and
+related topics from the person behind ShortGPT. We're eager to interact with
+you and listen to your feedback, concepts, and experiences with Short-GPT. Come
+on board on Twitter and let's navigate the future of AI as a team! ð¡ð¤
                              [Star_History_Chart]
```

### Comparing `shortgpt-0.1.3/README.md` & `shortgpt-0.1.31/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 # 🚀🎬 ShortGPT
-[![](https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ)
-[![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/shortgpt)
-<div align="center">
-    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
+<p align="center">
+  <a href="https://discord.gg/uERx39ru3R">
+    <img src="https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat">
+  </a>
+  <a href="https://twitter.com/RayVenturaHQ">
+    <img src="https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura">
+  </a>
+  <a href="https://star-history.com/#rayventura/shortgpt)">
+    <img src="https://img.shields.io/github/stars/rayventura/shortgpt?style=social">
+  </a>
+  <a href="https://pypi.org/project/shortgpt/">
+    <img src="https://static.pepy.tech/personalized-badge/shortgpt?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads/month">
+  </a>
+  <a href="https://docs.shortgpt.ai/">
+    <img src="https://img.shields.io/badge/docs-visit-blue">
+  </a>  
+</p>
+
+<div align="center" style="border-radius: 20px;" width="18%">
+    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="18%"/>
 </div>
 <div align="center">
   <a href="https://discord.gg/uERx39ru3R">
-    <img src="https://img.shields.io/badge/discord-join%20chat-blue.svg" alt="Join our Discord" height="34">
+    <img src="https://img.shields.io/discord/1126042224979886160?color=7289da&logo=discord&logoColor=blue&labelColor=white&color=cyan" alt="Join our Discord" height="34">
   </a>
 </div>
 
 <div align="center">
 ⚡ Automating video and short content creation with AI ⚡
 </div>
+</br>
 
+If you're only interested in using ShortGPT programatically (pip library), go on [the documentation website](https://docs.shortgpt.ai/docs/how-to-install).
+Otherwise, follow the installation steps below for running the web app locally. 
 ## 🎥 Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U))
 
 https://github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-6365c27ea5fe
 ## 🎥 Voice Dubbing
 
 
 https://github.com/RayVentura/ShortGPT/assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef
@@ -32,15 +50,15 @@
 ## 📝 Introduction to ShortGPT 
 ShortGPT is a powerful framework for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
 
 - 🎞️ **Automated editing framework**: Streamlines the video creation process with an LLM oriented video editing language.
 
 - 📃 **Scripts and Prompts**: Provides ready-to-use scripts and prompts for various LLM automated editing processes.
 
-- 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, and Portuguese 🇵🇹.
+- 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, Portuguese 🇵🇹, Russian 🇷🇺, Mandarin Chinese 🇨🇳, Japanese 🇯🇵, Hindi 🇮🇳,Korean 🇰🇷, and way over 30 more languages (with EdgeTTS)
 
 - 🔗 **Caption Generation**: Automates the generation of video captions.
 
 - 🌐🎥 **Asset Sourcing**: Sources images and video footage from the internet, connecting with the web and Pexels API as necessary.
 
 - 🧠 **Memory and persistency**: Ensures long-term persistency of automated editing variables with TinyDB.
 
@@ -51,64 +69,21 @@
 1. Click on the link to the Google Colab notebook: [https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
 2. Once you're in the notebook, simply run the cells in order from top to bottom. You can do this by clicking on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy using ShortGPT!
 
 # Instructions for running shortGPT
 This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
 
-## Prerequisites
-Before you begin, ensure that you have the following prerequisites installed on your system:
-- Python 3.x
-- Pip (Python package installer)
+
 
 ## Installation Steps
 Follow the instructions below to install ImageMagick, FFmpeg, and clone the shortGPT repository:
 
-### Step 1: Install ImageMagick
-1. For `Windows` download the installer from the official ImageMagick website and follow the installation instructions.
-      
-      [https://imagemagick.org/script/download.php](https://imagemagick.org/script/download.php)
-          
-2. For Ubuntu/Debian-based systems, use the command:
-     ```
-     sudo apt-get install imagemagick
-     ```
-     Then run the following command to fix a moviepy Imagemagick policy.xml incompatibility problem:
-     ```
-     !sed -i '/<policy domain="path" rights="none" pattern="@\*"/d' /etc/ImageMagick-6/policy.xml
-     ```    
-4. For macOS using Homebrew, use the command:
-     ```
-     brew install imagemagick
-     ```
-2. Verify the installation by running the following command:
-   ```
-   convert --version
-   ```
-   You should see the ImageMagick version information if the installation was successful.
-
-### Step 2: Install FFmpeg (REQUIRED FOR SHORTGPT TO WORK)
-1. For `Windows`Download the FFmpeg binaries from this Windows Installer (It will download ffmpeg, ffprobe and add it to your path).
-      
-      [https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306)
-      
-2. For macOS using Homebrew, use the command:
-     ```
-     brew install ffmpeg
-     ```   
-    For Ubuntu/Debian-based systems, use the command:
-     ```
-     sudo apt-get install ffmpeg
-     ```
-2. Verify the installation by running the following command:
-   ```
-   ffmpeg -version
-   ```
-   You should see the FFmpeg version information if the installation was successful.
-
+### Step 1 and 2, install Ffmpeg and ImageMagick
+For the updated installation steps, please follow Step 1 and 2 in our official documentation [docs.shortgpt.ai/docs/how-to-install](https://docs.shortgpt.ai/docs/how-to-install).
 ### Step 3: Clone the shortGPT Repository
 
 1. Open a terminal or command prompt.
 2. Execute the following command to clone the shortGPT repository:
    ```
    git clone https://github.com/rayventura/shortgpt.git
    ```
@@ -132,32 +107,22 @@
 2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to run the script:
    ```
    python runShortGPT.py
    ```
 4. After running the script, a Gradio interface should open at your local host on port 31415 (http://localhost:31415). 
 
-## Putting API Keys
-The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for running short automations. For video automations, you will also need to add a Pexels API.
-
-Follow these steps to add your OpenAI and ElevenLabs API keys:
-
-1. Open [http://localhost:31415/?__theme=light](http://localhost:31415/?__theme=light) from a web browser. 
-2. Click on the `config` tab located at the left side bar of the user interface.
-3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the corresponding input fields.
-4. Click `Save` to save your API keys.
-
-That's it! You have successfully set up your API keys and can now utilize the functionality of ShortGPT in the Gradio interface.
-
 ## Framework overview
 
 - 🎬 The `ContentShortEngine` is designed for creating shorts, handling tasks from script generation to final rendering, including adding YouTube metadata.
 
 - 🎥 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like generating audio, automatically sourcing background video footage, timing captions, and preparing background assets.
-  
+
+- 🗣️ The `ContentTranslationEngine` is designed to dub and translate entire videos, from mainstream languages to more specific target languages. It takes a video file, or youtube link, transcribe it's audio, translates the content, voices it in a target language, adds captions , and gives back a new video, in a totally different language.
+
 - 🎞️ The automated `EditingEngine`, using Editing Markup Language and JSON, breaks down the editing process into manageable and customizable blocks, comprehensible to Large Language Models.
 
 💡 ShortGPT offers customization options to suit your needs, from language selection to watermark addition.
 
 🔧 As a framework, ShortGPT is adaptable and flexible, offering the potential for efficient, creative content creation.
 
 More documentation incomming, please be patient.
@@ -169,14 +134,16 @@
 
 - **Moviepy**: Moviepy is used for video editing, allowing ShortGPT to make video editing and rendering
 
 - **Openai**: Openai is used for automating the entire process, including generating scripts and prompts for LLM automated editing processes.
 
 - **ElevenLabs**: ElevenLabs is used for voice synthesis, supporting multiple languages for voiceover creation.
 
+- **EdgeTTS**: Microsoft's FREE EdgeTTS is used for voice synthesis, supporting way many more language than ElevenLabs currently.
+
 - **Pexels**: Pexels is used for sourcing background footage, allowing ShortGPT to connect with the web and access a wide range of images and videos.
 
 - **Bing Image**: Bing Image is used for sourcing images, providing a comprehensive database for ShortGPT to retrieve relevant visuals.
 
 These technologies work together to provide a seamless and efficient experience in automating video and short content creation with AI.
 
 ## 💁 Contributing
```

#### html2text {}

```diff
@@ -1,17 +1,21 @@
-# ðð¬ ShortGPT [![](https://dcbadge.vercel.app/api/server/
-uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R) [![Twitter]
-(https://img.shields.io/twitter/url/https/twitter.com/
-rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://
-twitter.com/RayVenturaHQ) [![GitHub star chart](https://img.shields.io/github/
-stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
-shortgpt)
+# ðð¬ ShortGPT
+  [https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat]
+            [https://img.shields.io/twitter/url/https/twitter.com/
+     rayventurahq.svg?style=social&label=Follow%20%40RayVentura] [https://
+    img.shields.io/github/stars/rayventura/shortgpt?style=social] [https://
+                     static.pepy.tech/personalized-badge/
+shortgpt?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads/
+             month] [https://img.shields.io/badge/docs-visit-blue]
                                 [ShortGPT-logo]
                               [Join_our_Discord]
           â¡ Automating video and short content creation with AI â¡
+ If you're only interested in using ShortGPT programatically (pip library), go
+on [the documentation website](https://docs.shortgpt.ai/docs/how-to-install).
+Otherwise, follow the installation steps below for running the web app locally.
 ## ð¥ Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U)) https:
 //github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-
 6365c27ea5fe ## ð¥ Voice Dubbing https://github.com/RayVentura/ShortGPT/
 assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef ## ð Show Your Support
 We hope you find ShortGPT helpful! If you do, let us know by giving us a star
 â­ on the repo. It's easy, just click on the 'Star' button at the top right of
 the page. Your support means a lot to us and keeps us motivated to improve and
@@ -23,107 +27,87 @@
 powerful framework for automating content creation. It simplifies video
 creation, footage sourcing, voiceover synthesis, and editing tasks. - ðï¸
 **Automated editing framework**: Streamlines the video creation process with an
 LLM oriented video editing language. - ð **Scripts and Prompts**: Provides
 ready-to-use scripts and prompts for various LLM automated editing processes. -
 ð£ï¸ **Voiceover / Content Creation**: Supports multiple languages including
 English ðºð¸, Spanish ðªð¸, Arabic ð¦ðª, French ð«ð·, Polish
-ðµð±, German ð©ðª, Italian ð®ð¹, and Portuguese ðµð¹. - ð
-**Caption Generation**: Automates the generation of video captions. - ðð¥
-**Asset Sourcing**: Sources images and video footage from the internet,
-connecting with the web and Pexels API as necessary. - ð§  **Memory and
-persistency**: Ensures long-term persistency of automated editing variables
-with TinyDB. ## ð Quick Start: Run ShortGPT on Google Colab (https://
+ðµð±, German ð©ðª, Italian ð®ð¹, Portuguese ðµð¹, Russian
+ð·ðº, Mandarin Chinese ð¨ð³, Japanese ð¯ðµ, Hindi ð®ð³,Korean
+ð°ð·, and way over 30 more languages (with EdgeTTS) - ð **Caption
+Generation**: Automates the generation of video captions. - ðð¥ **Asset
+Sourcing**: Sources images and video footage from the internet, connecting with
+the web and Pexels API as necessary. - ð§  **Memory and persistency**: Ensures
+long-term persistency of automated editing variables with TinyDB. ## ð Quick
+Start: Run ShortGPT on Google Colab (https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) If you prefer not to install the
+prerequisites on your local system, you can use the Google Colab notebook. This
+option is free and requires no installation setup. 1. Click on the link to the
+Google Colab notebook: [https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://
 colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
-If you prefer not to install the prerequisites on your local system, you can
-use the Google Colab notebook. This option is free and requires no installation
-setup. 1. Click on the link to the Google Colab notebook: [https://
-colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing]
-(https://colab.research.google.com/drive/
-1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) 2. Once you're in the notebook,
-simply run the cells in order from top to bottom. You can do this by clicking
-on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy
-using ShortGPT! # Instructions for running shortGPT This guide provides step-
-by-step instructions for installing ImageMagick and FFmpeg on your system,
-which are both required to do automated editing. Once installed, you can
-proceed to run `runShortGPT.py` successfully. ## Prerequisites Before you
-begin, ensure that you have the following prerequisites installed on your
-system: - Python 3.x - Pip (Python package installer) ## Installation Steps
-Follow the instructions below to install ImageMagick, FFmpeg, and clone the
-shortGPT repository: ### Step 1: Install ImageMagick 1. For `Windows` download
-the installer from the official ImageMagick website and follow the installation
-instructions. [https://imagemagick.org/script/download.php](https://
-imagemagick.org/script/download.php) 2. For Ubuntu/Debian-based systems, use
-the command: ``` sudo apt-get install imagemagick ``` Then run the following
-command to fix a moviepy Imagemagick policy.xml incompatibility problem: ```
-!sed -i '/
-' /etc/ImageMagick-6/policy.xml ``` 4. For macOS using Homebrew, use the
-command: ``` brew install imagemagick ``` 2. Verify the installation by running
-the following command: ``` convert --version ``` You should see the ImageMagick
-version information if the installation was successful. ### Step 2: Install
-FFmpeg (REQUIRED FOR SHORTGPT TO WORK) 1. For `Windows`Download the FFmpeg
-binaries from this Windows Installer (It will download ffmpeg, ffprobe and add
-it to your path). [https://github.com/icedterminal/ffmpeg-installer/releases/
-tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/
-tag/6.0.0.20230306) 2. For macOS using Homebrew, use the command: ``` brew
-install ffmpeg ``` For Ubuntu/Debian-based systems, use the command: ``` sudo
-apt-get install ffmpeg ``` 2. Verify the installation by running the following
-command: ``` ffmpeg -version ``` You should see the FFmpeg version information
-if the installation was successful. ### Step 3: Clone the shortGPT Repository
-1. Open a terminal or command prompt. 2. Execute the following command to clone
-the shortGPT repository: ``` git clone https://github.com/rayventura/
-shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a terminal or
-command prompt. 2. Navigate to the directory where `runShortGPT.py` is located
-(the cloned repo). 3. Execute the following command to install the required
-Python dependencies: ``` pip install -r requirements.txt ``` This command will
-install the necessary packages specified in the `requirements.txt` file. ##
-Running runShortGPT.py Web Interface Once you have successfully installed
-ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py`
-by following these steps: 1. Open a terminal or command prompt. 2. Navigate to
-the directory where `runShortGPT.py` is located (the cloned repo). 3. Execute
-the following command to run the script: ``` python runShortGPT.py ``` 4. After
-running the script, a Gradio interface should open at your local host on port
-31415 (http://localhost:31415). ## Putting API Keys The ShortGPT UI needs you
-to input at least OpenAI and ElevenLabs api keys for running short automations.
-For video automations, you will also need to add a Pexels API. Follow these
-steps to add your OpenAI and ElevenLabs API keys: 1. Open [http://localhost:
-31415/?__theme=light](http://localhost:31415/?__theme=light) from a web
-browser. 2. Click on the `config` tab located at the left side bar of the user
-interface. 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the
-corresponding input fields. 4. Click `Save` to save your API keys. That's it!
-You have successfully set up your API keys and can now utilize the
-functionality of ShortGPT in the Gradio interface. ## Framework overview - ð¬
-The `ContentShortEngine` is designed for creating shorts, handling tasks from
-script generation to final rendering, including adding YouTube metadata. - ð¥
-The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like
-generating audio, automatically sourcing background video footage, timing
-captions, and preparing background assets. - ðï¸ The automated
-`EditingEngine`, using Editing Markup Language and JSON, breaks down the
-editing process into manageable and customizable blocks, comprehensible to
-Large Language Models. ð¡ ShortGPT offers customization options to suit your
-needs, from language selection to watermark addition. ð§ As a framework,
-ShortGPT is adaptable and flexible, offering the potential for efficient,
-creative content creation. More documentation incomming, please be patient. ##
-Technologies Used ShortGPT utilizes the following technologies to power its
-functionality: - **Moviepy**: Moviepy is used for video editing, allowing
-ShortGPT to make video editing and rendering - **Openai**: Openai is used for
-automating the entire process, including generating scripts and prompts for LLM
-automated editing processes. - **ElevenLabs**: ElevenLabs is used for voice
-synthesis, supporting multiple languages for voiceover creation. - **Pexels**:
-Pexels is used for sourcing background footage, allowing ShortGPT to connect
-with the web and access a wide range of images and videos. - **Bing Image**:
-Bing Image is used for sourcing images, providing a comprehensive database for
-ShortGPT to retrieve relevant visuals. These technologies work together to
-provide a seamless and efficient experience in automating video and short
-content creation with AI. ## ð Contributing As an open-source project in a
-rapidly developing field, we are extremely open to contributions, whether it
-would be in the form of a new feature, improved infrastructure, or better
-documentation. ## ð Get in touch on Twitter ð¦ Keep up with the latest
-happenings, announcements, and insights about Short-GPT by checking out our
-Twitter accounts. Spark a conversation with our developer and the AI's own
-account for fascinating dialogues, latest news about the project, and more. -
-**Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ).
-Deep-dive into behind-the-scenes, project news, and related topics from the
-person behind ShortGPT. We're eager to interact with you and listen to your
-feedback, concepts, and experiences with Short-GPT. Come on board on Twitter
-and let's navigate the future of AI as a team! ð¡ð¤
+2. Once you're in the notebook, simply run the cells in order from top to
+bottom. You can do this by clicking on each cell and pressing the 'Play'
+button, or by using the keyboard . Enjoy using ShortGPT! # Instructions for
+running shortGPT This guide provides step-by-step instructions for installing
+ImageMagick and FFmpeg on your system, which are both required to do automated
+editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
+## Installation Steps Follow the instructions below to install ImageMagick,
+FFmpeg, and clone the shortGPT repository: ### Step 1 and 2, install Ffmpeg and
+ImageMagick For the updated installation steps, please follow Step 1 and 2 in
+our official documentation [docs.shortgpt.ai/docs/how-to-install](https://
+docs.shortgpt.ai/docs/how-to-install). ### Step 3: Clone the shortGPT
+Repository 1. Open a terminal or command prompt. 2. Execute the following
+command to clone the shortGPT repository: ``` git clone https://github.com/
+rayventura/shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a
+terminal or command prompt. 2. Navigate to the directory where `runShortGPT.py`
+is located (the cloned repo). 3. Execute the following command to install the
+required Python dependencies: ``` pip install -r requirements.txt ``` This
+command will install the necessary packages specified in the `requirements.txt`
+file. ## Running runShortGPT.py Web Interface Once you have successfully
+installed ImageMagick, FFmpeg, and the Python dependencies, you can run
+`runShortGPT.py` by following these steps: 1. Open a terminal or command
+prompt. 2. Navigate to the directory where `runShortGPT.py` is located (the
+cloned repo). 3. Execute the following command to run the script: ``` python
+runShortGPT.py ``` 4. After running the script, a Gradio interface should open
+at your local host on port 31415 (http://localhost:31415). ## Framework
+overview - ð¬ The `ContentShortEngine` is designed for creating shorts,
+handling tasks from script generation to final rendering, including adding
+YouTube metadata. - ð¥ The `ContentVideoEngine` is ideal for longer videos,
+taking care of tasks like generating audio, automatically sourcing background
+video footage, timing captions, and preparing background assets. - ð£ï¸ The
+`ContentTranslationEngine` is designed to dub and translate entire videos, from
+mainstream languages to more specific target languages. It takes a video file,
+or youtube link, transcribe it's audio, translates the content, voices it in a
+target language, adds captions , and gives back a new video, in a totally
+different language. - ðï¸ The automated `EditingEngine`, using Editing
+Markup Language and JSON, breaks down the editing process into manageable and
+customizable blocks, comprehensible to Large Language Models. ð¡ ShortGPT
+offers customization options to suit your needs, from language selection to
+watermark addition. ð§ As a framework, ShortGPT is adaptable and flexible,
+offering the potential for efficient, creative content creation. More
+documentation incomming, please be patient. ## Technologies Used ShortGPT
+utilizes the following technologies to power its functionality: - **Moviepy**:
+Moviepy is used for video editing, allowing ShortGPT to make video editing and
+rendering - **Openai**: Openai is used for automating the entire process,
+including generating scripts and prompts for LLM automated editing processes. -
+**ElevenLabs**: ElevenLabs is used for voice synthesis, supporting multiple
+languages for voiceover creation. - **EdgeTTS**: Microsoft's FREE EdgeTTS is
+used for voice synthesis, supporting way many more language than ElevenLabs
+currently. - **Pexels**: Pexels is used for sourcing background footage,
+allowing ShortGPT to connect with the web and access a wide range of images and
+videos. - **Bing Image**: Bing Image is used for sourcing images, providing a
+comprehensive database for ShortGPT to retrieve relevant visuals. These
+technologies work together to provide a seamless and efficient experience in
+automating video and short content creation with AI. ## ð Contributing As an
+open-source project in a rapidly developing field, we are extremely open to
+contributions, whether it would be in the form of a new feature, improved
+infrastructure, or better documentation. ## ð Get in touch on Twitter ð¦
+Keep up with the latest happenings, announcements, and insights about Short-GPT
+by checking out our Twitter accounts. Spark a conversation with our developer
+and the AI's own account for fascinating dialogues, latest news about the
+project, and more. - **Developer**: Stay updated [@RayVentura](https://
+twitter.com/RayVenturaHQ). Deep-dive into behind-the-scenes, project news, and
+related topics from the person behind ShortGPT. We're eager to interact with
+you and listen to your feedback, concepts, and experiences with Short-GPT. Come
+on board on Twitter and let's navigate the future of AI as a team! ð¡ð¤
                              [Star_History_Chart]
```

### Comparing `shortgpt-0.1.3/setup.py` & `shortgpt-0.1.31/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
+VERSION = '0.1.31'
 DESCRIPTION = 'Automating video and short content creation with AI'
 LONG_DESCRIPTION = 'A powerful tool for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.'
 
 
 setup(
     name="shortgpt",
     version=VERSION,
```

### Comparing `shortgpt-0.1.3/shortGPT/__init__.py` & `shortgpt-0.1.31/shortGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/api_utils/eleven_api.py` & `shortgpt-0.1.31/shortGPT/api_utils/eleven_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/api_utils/image_api.py` & `shortgpt-0.1.31/shortGPT/api_utils/image_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/api_utils/pexels_api.py` & `shortgpt-0.1.31/shortGPT/api_utils/pexels_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/audio/audio_duration.py` & `shortgpt-0.1.31/shortGPT/audio/audio_duration.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/audio/audio_utils.py` & `shortgpt-0.1.31/shortGPT/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/audio/edge_voice_module.py` & `shortgpt-0.1.31/shortGPT/audio/edge_voice_module.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/audio/eleven_voice_module.py` & `shortgpt-0.1.31/shortGPT/audio/eleven_voice_module.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/config/api_db.py` & `shortgpt-0.1.31/shortGPT/config/api_db.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/config/asset_db.py` & `shortgpt-0.1.31/shortGPT/config/asset_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class AssetDatabase:
     """
     Class for managing assets, both local and remote.
     The class provides methods to add, remove, get and sync assets.
     It uses a MongoDB-like database to store information about the assets.
     """
 
-    if not Path(ASSETS_DB_PATH).exists():
+    if not Path(ASSETS_DB_PATH).exists() and Path(TEMPLATE_ASSETS_DB_PATH).exists():
         shutil.copy(TEMPLATE_ASSETS_DB_PATH, ASSETS_DB_PATH)
 
     local_assets = TinyMongoDocument("asset_db", "asset_collection", "local_assets", create=True)
     remote_assets = TinyMongoDocument("asset_db", "asset_collection", "remote_assets", create=True)
     if not remote_assets._get('subscribe animation'):
         remote_assets._save({
             'subscribe animation':{
@@ -237,15 +237,15 @@
 
         Returns:
             str: Duration of the asset.
         """
         asset = cls.local_assets._get(key)
         asset['ts'] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         cls.local_assets._save({key: asset})
-        if 'duration' not in asset:
+        if 'duration' not in asset and asset['duration'] is not None:
             _, duration = cls._update_local_asset_duration(key)
             return duration
         return asset['duration']
 
     @classmethod
     def _get_remote_asset_duration(cls, key: str) -> str:
         """
@@ -256,15 +256,15 @@
 
         Returns:
             str: Duration of the asset.
         """
         asset = cls.remote_assets._get(key)
         asset['ts'] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         cls.remote_assets._save({key: asset})
-        if 'duration' in asset:
+        if 'duration' in asset and asset['duration'] is not None:
             return asset['duration']
         _, duration = cls._update_youtube_asset_duration(key)
         return duration
 
     @classmethod
     def _update_local_asset_duration(cls, key: str) -> str:
         """
```

### Comparing `shortgpt-0.1.3/shortGPT/config/config.py` & `shortgpt-0.1.31/shortGPT/config/config.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/config/languages.py` & `shortgpt-0.1.31/shortGPT/config/languages.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/config/path_utils.py` & `shortgpt-0.1.31/shortGPT/config/path_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/database/content_data_manager.py` & `shortgpt-0.1.31/shortGPT/database/content_data_manager.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/database/content_database.py` & `shortgpt-0.1.31/shortGPT/database/content_database.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/database/db_document.py` & `shortgpt-0.1.31/shortGPT/database/db_document.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/core_editing_engine.py` & `shortgpt-0.1.31/shortGPT/editing_framework/core_editing_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_engine.py` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/extract_audio.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/extract_audio.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption_arabic.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption_arabic.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/make_caption_landscape.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/make_caption_landscape.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/show_top_image.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/show_top_image.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/show_watermark.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/show_watermark.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/editing_steps/subscribe_animation.json` & `shortgpt-0.1.31/shortGPT/editing_framework/editing_steps/subscribe_animation.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/flows/build_reddit_image.json` & `shortgpt-0.1.31/shortGPT/editing_framework/flows/build_reddit_image.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_framework/rendering_logger.py` & `shortgpt-0.1.31/shortGPT/editing_framework/rendering_logger.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_utils/captions.py` & `shortgpt-0.1.31/shortGPT/editing_utils/captions.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_utils/editing_images.py` & `shortgpt-0.1.31/shortGPT/editing_utils/editing_images.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/editing_utils/handle_videos.py` & `shortgpt-0.1.31/shortGPT/editing_utils/handle_videos.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/engine/abstract_content_engine.py` & `shortgpt-0.1.31/shortGPT/engine/abstract_content_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/engine/content_short_engine.py` & `shortgpt-0.1.31/shortGPT/engine/content_short_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,16 @@
                                                                         'set_time_end': timing[1]})
 
             videoEditor.renderVideo(outputPath, logger= self.logger if self.logger is not self.default_logger else None)
 
         self._db_video_path = outputPath
 
     def _addYoutubeMetadata(self):
-
+        if not os.path.exists('videos/'):
+            os.makedirs('videos')
         self._db_yt_title, self._db_yt_description = gpt_yt.generate_title_description_dict(self._db_script)
 
         now = datetime.datetime.now()
         date_str = now.strftime("%Y-%m-%d_%H-%M-%S")
         newFileName = f"videos/{date_str} - " + \
             re.sub(r"[^a-zA-Z0-9 '\n\.]", '', self._db_yt_title)
```

### Comparing `shortgpt-0.1.3/shortGPT/engine/content_translation_engine.py` & `shortgpt-0.1.31/shortGPT/engine/content_translation_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/engine/content_video_engine.py` & `shortgpt-0.1.31/shortGPT/engine/content_video_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,16 @@
                                                           'set_time_end': t2})
 
             videoEditor.renderVideo(outputPath, logger= self.logger if self.logger is not self.default_logger else None)
 
         self._db_video_path = outputPath
 
     def _addMetadata(self):
-
+        if not os.path.exists('videos/'):
+            os.makedirs('videos')
         self._db_yt_title, self._db_yt_description = gpt_yt.generate_title_description_dict(self._db_script)
 
         now = datetime.datetime.now()
         date_str = now.strftime("%Y-%m-%d_%H-%M-%S")
         newFileName = f"videos/{date_str} - " + \
             re.sub(r"[^a-zA-Z0-9 '\n\.]", '', self._db_yt_title)
```

### Comparing `shortgpt-0.1.3/shortGPT/engine/facts_short_engine.py` & `shortgpt-0.1.31/shortGPT/engine/facts_short_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/engine/multi_language_translation_engine.py` & `shortgpt-0.1.31/shortGPT/engine/multi_language_translation_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/engine/reddit_short_engine.py` & `shortgpt-0.1.31/shortGPT/engine/reddit_short_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/gpt/facts_gpt.py` & `shortgpt-0.1.31/shortGPT/gpt/facts_gpt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/gpt/gpt_chat_video.py` & `shortgpt-0.1.31/shortGPT/gpt/gpt_chat_video.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/gpt/gpt_editing.py` & `shortgpt-0.1.31/shortGPT/gpt/gpt_editing.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/gpt/gpt_translate.py` & `shortgpt-0.1.31/shortGPT/gpt/gpt_translate.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/gpt/gpt_utils.py` & `shortgpt-0.1.31/shortGPT/gpt/gpt_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/gpt/gpt_yt.py` & `shortgpt-0.1.31/shortGPT/gpt/gpt_yt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/gpt/reddit_gpt.py` & `shortgpt-0.1.31/shortGPT/gpt/reddit_gpt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/chat_video_edit_script.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/chat_video_edit_script.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/chat_video_script.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/chat_video_script.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/editing_generate_images.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/editing_generate_images.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/editing_generate_videos.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/editing_generate_videos.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/facts_generator.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/facts_generator.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/reddit_extract_question.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/reddit_extract_question.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/reddit_filter_realistic.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/reddit_filter_realistic.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/reddit_generate_question.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/reddit_generate_question.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/reddit_generate_script.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/reddit_generate_script.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/reddit_story_filter.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/reddit_story_filter.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/translate_content.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/translate_content.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/prompt_templates/yt_title_description.yaml` & `shortgpt-0.1.31/shortGPT/prompt_templates/yt_title_description.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/tracking/api_tracking.py` & `shortgpt-0.1.31/shortGPT/tracking/api_tracking.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortGPT/tracking/cost_analytics.py` & `shortgpt-0.1.31/shortGPT/tracking/cost_analytics.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.3/shortgpt.egg-info/PKG-INFO` & `shortgpt-0.1.31/shortgpt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortgpt
-Version: 0.1.3
+Version: 0.1.31
 Summary: Automating video and short content creation with AI
 Author: RayVentura
 Author-email: 
 Keywords: python,video,content creation,AI,automation,editing,voiceover synthesis,video captions,asset sourcing,tinyDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,30 +12,48 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # 🚀🎬 ShortGPT
-[![](https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ)
-[![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/shortgpt)
-<div align="center">
-    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
+<p align="center">
+  <a href="https://discord.gg/uERx39ru3R">
+    <img src="https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat">
+  </a>
+  <a href="https://twitter.com/RayVenturaHQ">
+    <img src="https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura">
+  </a>
+  <a href="https://star-history.com/#rayventura/shortgpt)">
+    <img src="https://img.shields.io/github/stars/rayventura/shortgpt?style=social">
+  </a>
+  <a href="https://pypi.org/project/shortgpt/">
+    <img src="https://static.pepy.tech/personalized-badge/shortgpt?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads/month">
+  </a>
+  <a href="https://docs.shortgpt.ai/">
+    <img src="https://img.shields.io/badge/docs-visit-blue">
+  </a>  
+</p>
+
+<div align="center" style="border-radius: 20px;" width="18%">
+    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="18%"/>
 </div>
 <div align="center">
   <a href="https://discord.gg/uERx39ru3R">
-    <img src="https://img.shields.io/badge/discord-join%20chat-blue.svg" alt="Join our Discord" height="34">
+    <img src="https://img.shields.io/discord/1126042224979886160?color=7289da&logo=discord&logoColor=blue&labelColor=white&color=cyan" alt="Join our Discord" height="34">
   </a>
 </div>
 
 <div align="center">
 ⚡ Automating video and short content creation with AI ⚡
 </div>
+</br>
 
+If you're only interested in using ShortGPT programatically (pip library), go on [the documentation website](https://docs.shortgpt.ai/docs/how-to-install).
+Otherwise, follow the installation steps below for running the web app locally. 
 ## 🎥 Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U))
 
 https://github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-6365c27ea5fe
 ## 🎥 Voice Dubbing
 
 
 https://github.com/RayVentura/ShortGPT/assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef
@@ -49,15 +67,15 @@
 ## 📝 Introduction to ShortGPT 
 ShortGPT is a powerful framework for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
 
 - 🎞️ **Automated editing framework**: Streamlines the video creation process with an LLM oriented video editing language.
 
 - 📃 **Scripts and Prompts**: Provides ready-to-use scripts and prompts for various LLM automated editing processes.
 
-- 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, and Portuguese 🇵🇹.
+- 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, Portuguese 🇵🇹, Russian 🇷🇺, Mandarin Chinese 🇨🇳, Japanese 🇯🇵, Hindi 🇮🇳,Korean 🇰🇷, and way over 30 more languages (with EdgeTTS)
 
 - 🔗 **Caption Generation**: Automates the generation of video captions.
 
 - 🌐🎥 **Asset Sourcing**: Sources images and video footage from the internet, connecting with the web and Pexels API as necessary.
 
 - 🧠 **Memory and persistency**: Ensures long-term persistency of automated editing variables with TinyDB.
 
@@ -68,64 +86,21 @@
 1. Click on the link to the Google Colab notebook: [https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
 2. Once you're in the notebook, simply run the cells in order from top to bottom. You can do this by clicking on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy using ShortGPT!
 
 # Instructions for running shortGPT
 This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
 
-## Prerequisites
-Before you begin, ensure that you have the following prerequisites installed on your system:
-- Python 3.x
-- Pip (Python package installer)
+
 
 ## Installation Steps
 Follow the instructions below to install ImageMagick, FFmpeg, and clone the shortGPT repository:
 
-### Step 1: Install ImageMagick
-1. For `Windows` download the installer from the official ImageMagick website and follow the installation instructions.
-      
-      [https://imagemagick.org/script/download.php](https://imagemagick.org/script/download.php)
-          
-2. For Ubuntu/Debian-based systems, use the command:
-     ```
-     sudo apt-get install imagemagick
-     ```
-     Then run the following command to fix a moviepy Imagemagick policy.xml incompatibility problem:
-     ```
-     !sed -i '/<policy domain="path" rights="none" pattern="@\*"/d' /etc/ImageMagick-6/policy.xml
-     ```    
-4. For macOS using Homebrew, use the command:
-     ```
-     brew install imagemagick
-     ```
-2. Verify the installation by running the following command:
-   ```
-   convert --version
-   ```
-   You should see the ImageMagick version information if the installation was successful.
-
-### Step 2: Install FFmpeg (REQUIRED FOR SHORTGPT TO WORK)
-1. For `Windows`Download the FFmpeg binaries from this Windows Installer (It will download ffmpeg, ffprobe and add it to your path).
-      
-      [https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306)
-      
-2. For macOS using Homebrew, use the command:
-     ```
-     brew install ffmpeg
-     ```   
-    For Ubuntu/Debian-based systems, use the command:
-     ```
-     sudo apt-get install ffmpeg
-     ```
-2. Verify the installation by running the following command:
-   ```
-   ffmpeg -version
-   ```
-   You should see the FFmpeg version information if the installation was successful.
-
+### Step 1 and 2, install Ffmpeg and ImageMagick
+For the updated installation steps, please follow Step 1 and 2 in our official documentation [docs.shortgpt.ai/docs/how-to-install](https://docs.shortgpt.ai/docs/how-to-install).
 ### Step 3: Clone the shortGPT Repository
 
 1. Open a terminal or command prompt.
 2. Execute the following command to clone the shortGPT repository:
    ```
    git clone https://github.com/rayventura/shortgpt.git
    ```
@@ -149,32 +124,22 @@
 2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to run the script:
    ```
    python runShortGPT.py
    ```
 4. After running the script, a Gradio interface should open at your local host on port 31415 (http://localhost:31415). 
 
-## Putting API Keys
-The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for running short automations. For video automations, you will also need to add a Pexels API.
-
-Follow these steps to add your OpenAI and ElevenLabs API keys:
-
-1. Open [http://localhost:31415/?__theme=light](http://localhost:31415/?__theme=light) from a web browser. 
-2. Click on the `config` tab located at the left side bar of the user interface.
-3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the corresponding input fields.
-4. Click `Save` to save your API keys.
-
-That's it! You have successfully set up your API keys and can now utilize the functionality of ShortGPT in the Gradio interface.
-
 ## Framework overview
 
 - 🎬 The `ContentShortEngine` is designed for creating shorts, handling tasks from script generation to final rendering, including adding YouTube metadata.
 
 - 🎥 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like generating audio, automatically sourcing background video footage, timing captions, and preparing background assets.
-  
+
+- 🗣️ The `ContentTranslationEngine` is designed to dub and translate entire videos, from mainstream languages to more specific target languages. It takes a video file, or youtube link, transcribe it's audio, translates the content, voices it in a target language, adds captions , and gives back a new video, in a totally different language.
+
 - 🎞️ The automated `EditingEngine`, using Editing Markup Language and JSON, breaks down the editing process into manageable and customizable blocks, comprehensible to Large Language Models.
 
 💡 ShortGPT offers customization options to suit your needs, from language selection to watermark addition.
 
 🔧 As a framework, ShortGPT is adaptable and flexible, offering the potential for efficient, creative content creation.
 
 More documentation incomming, please be patient.
@@ -186,14 +151,16 @@
 
 - **Moviepy**: Moviepy is used for video editing, allowing ShortGPT to make video editing and rendering
 
 - **Openai**: Openai is used for automating the entire process, including generating scripts and prompts for LLM automated editing processes.
 
 - **ElevenLabs**: ElevenLabs is used for voice synthesis, supporting multiple languages for voiceover creation.
 
+- **EdgeTTS**: Microsoft's FREE EdgeTTS is used for voice synthesis, supporting way many more language than ElevenLabs currently.
+
 - **Pexels**: Pexels is used for sourcing background footage, allowing ShortGPT to connect with the web and access a wide range of images and videos.
 
 - **Bing Image**: Bing Image is used for sourcing images, providing a comprehensive database for ShortGPT to retrieve relevant visuals.
 
 These technologies work together to provide a seamless and efficient experience in automating video and short content creation with AI.
 
 ## 💁 Contributing
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
-Metadata-Version: 2.1 Name: shortgpt Version: 0.1.3 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.1.31 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
-LICENSE # ðð¬ ShortGPT [![](https://dcbadge.vercel.app/api/server/
-uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R) [![Twitter]
-(https://img.shields.io/twitter/url/https/twitter.com/
-rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://
-twitter.com/RayVenturaHQ) [![GitHub star chart](https://img.shields.io/github/
-stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
-shortgpt)
+LICENSE # ðð¬ ShortGPT
+  [https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat]
+            [https://img.shields.io/twitter/url/https/twitter.com/
+     rayventurahq.svg?style=social&label=Follow%20%40RayVentura] [https://
+    img.shields.io/github/stars/rayventura/shortgpt?style=social] [https://
+                     static.pepy.tech/personalized-badge/
+shortgpt?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads/
+             month] [https://img.shields.io/badge/docs-visit-blue]
                                 [ShortGPT-logo]
                               [Join_our_Discord]
           â¡ Automating video and short content creation with AI â¡
+ If you're only interested in using ShortGPT programatically (pip library), go
+on [the documentation website](https://docs.shortgpt.ai/docs/how-to-install).
+Otherwise, follow the installation steps below for running the web app locally.
 ## ð¥ Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U)) https:
 //github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-
 6365c27ea5fe ## ð¥ Voice Dubbing https://github.com/RayVentura/ShortGPT/
 assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef ## ð Show Your Support
 We hope you find ShortGPT helpful! If you do, let us know by giving us a star
 â­ on the repo. It's easy, just click on the 'Star' button at the top right of
 the page. Your support means a lot to us and keeps us motivated to improve and
@@ -31,107 +35,87 @@
 powerful framework for automating content creation. It simplifies video
 creation, footage sourcing, voiceover synthesis, and editing tasks. - ðï¸
 **Automated editing framework**: Streamlines the video creation process with an
 LLM oriented video editing language. - ð **Scripts and Prompts**: Provides
 ready-to-use scripts and prompts for various LLM automated editing processes. -
 ð£ï¸ **Voiceover / Content Creation**: Supports multiple languages including
 English ðºð¸, Spanish ðªð¸, Arabic ð¦ðª, French ð«ð·, Polish
-ðµð±, German ð©ðª, Italian ð®ð¹, and Portuguese ðµð¹. - ð
-**Caption Generation**: Automates the generation of video captions. - ðð¥
-**Asset Sourcing**: Sources images and video footage from the internet,
-connecting with the web and Pexels API as necessary. - ð§  **Memory and
-persistency**: Ensures long-term persistency of automated editing variables
-with TinyDB. ## ð Quick Start: Run ShortGPT on Google Colab (https://
+ðµð±, German ð©ðª, Italian ð®ð¹, Portuguese ðµð¹, Russian
+ð·ðº, Mandarin Chinese ð¨ð³, Japanese ð¯ðµ, Hindi ð®ð³,Korean
+ð°ð·, and way over 30 more languages (with EdgeTTS) - ð **Caption
+Generation**: Automates the generation of video captions. - ðð¥ **Asset
+Sourcing**: Sources images and video footage from the internet, connecting with
+the web and Pexels API as necessary. - ð§  **Memory and persistency**: Ensures
+long-term persistency of automated editing variables with TinyDB. ## ð Quick
+Start: Run ShortGPT on Google Colab (https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) If you prefer not to install the
+prerequisites on your local system, you can use the Google Colab notebook. This
+option is free and requires no installation setup. 1. Click on the link to the
+Google Colab notebook: [https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://
 colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
-If you prefer not to install the prerequisites on your local system, you can
-use the Google Colab notebook. This option is free and requires no installation
-setup. 1. Click on the link to the Google Colab notebook: [https://
-colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing]
-(https://colab.research.google.com/drive/
-1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) 2. Once you're in the notebook,
-simply run the cells in order from top to bottom. You can do this by clicking
-on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy
-using ShortGPT! # Instructions for running shortGPT This guide provides step-
-by-step instructions for installing ImageMagick and FFmpeg on your system,
-which are both required to do automated editing. Once installed, you can
-proceed to run `runShortGPT.py` successfully. ## Prerequisites Before you
-begin, ensure that you have the following prerequisites installed on your
-system: - Python 3.x - Pip (Python package installer) ## Installation Steps
-Follow the instructions below to install ImageMagick, FFmpeg, and clone the
-shortGPT repository: ### Step 1: Install ImageMagick 1. For `Windows` download
-the installer from the official ImageMagick website and follow the installation
-instructions. [https://imagemagick.org/script/download.php](https://
-imagemagick.org/script/download.php) 2. For Ubuntu/Debian-based systems, use
-the command: ``` sudo apt-get install imagemagick ``` Then run the following
-command to fix a moviepy Imagemagick policy.xml incompatibility problem: ```
-!sed -i '/
-' /etc/ImageMagick-6/policy.xml ``` 4. For macOS using Homebrew, use the
-command: ``` brew install imagemagick ``` 2. Verify the installation by running
-the following command: ``` convert --version ``` You should see the ImageMagick
-version information if the installation was successful. ### Step 2: Install
-FFmpeg (REQUIRED FOR SHORTGPT TO WORK) 1. For `Windows`Download the FFmpeg
-binaries from this Windows Installer (It will download ffmpeg, ffprobe and add
-it to your path). [https://github.com/icedterminal/ffmpeg-installer/releases/
-tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/
-tag/6.0.0.20230306) 2. For macOS using Homebrew, use the command: ``` brew
-install ffmpeg ``` For Ubuntu/Debian-based systems, use the command: ``` sudo
-apt-get install ffmpeg ``` 2. Verify the installation by running the following
-command: ``` ffmpeg -version ``` You should see the FFmpeg version information
-if the installation was successful. ### Step 3: Clone the shortGPT Repository
-1. Open a terminal or command prompt. 2. Execute the following command to clone
-the shortGPT repository: ``` git clone https://github.com/rayventura/
-shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a terminal or
-command prompt. 2. Navigate to the directory where `runShortGPT.py` is located
-(the cloned repo). 3. Execute the following command to install the required
-Python dependencies: ``` pip install -r requirements.txt ``` This command will
-install the necessary packages specified in the `requirements.txt` file. ##
-Running runShortGPT.py Web Interface Once you have successfully installed
-ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py`
-by following these steps: 1. Open a terminal or command prompt. 2. Navigate to
-the directory where `runShortGPT.py` is located (the cloned repo). 3. Execute
-the following command to run the script: ``` python runShortGPT.py ``` 4. After
-running the script, a Gradio interface should open at your local host on port
-31415 (http://localhost:31415). ## Putting API Keys The ShortGPT UI needs you
-to input at least OpenAI and ElevenLabs api keys for running short automations.
-For video automations, you will also need to add a Pexels API. Follow these
-steps to add your OpenAI and ElevenLabs API keys: 1. Open [http://localhost:
-31415/?__theme=light](http://localhost:31415/?__theme=light) from a web
-browser. 2. Click on the `config` tab located at the left side bar of the user
-interface. 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the
-corresponding input fields. 4. Click `Save` to save your API keys. That's it!
-You have successfully set up your API keys and can now utilize the
-functionality of ShortGPT in the Gradio interface. ## Framework overview - ð¬
-The `ContentShortEngine` is designed for creating shorts, handling tasks from
-script generation to final rendering, including adding YouTube metadata. - ð¥
-The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like
-generating audio, automatically sourcing background video footage, timing
-captions, and preparing background assets. - ðï¸ The automated
-`EditingEngine`, using Editing Markup Language and JSON, breaks down the
-editing process into manageable and customizable blocks, comprehensible to
-Large Language Models. ð¡ ShortGPT offers customization options to suit your
-needs, from language selection to watermark addition. ð§ As a framework,
-ShortGPT is adaptable and flexible, offering the potential for efficient,
-creative content creation. More documentation incomming, please be patient. ##
-Technologies Used ShortGPT utilizes the following technologies to power its
-functionality: - **Moviepy**: Moviepy is used for video editing, allowing
-ShortGPT to make video editing and rendering - **Openai**: Openai is used for
-automating the entire process, including generating scripts and prompts for LLM
-automated editing processes. - **ElevenLabs**: ElevenLabs is used for voice
-synthesis, supporting multiple languages for voiceover creation. - **Pexels**:
-Pexels is used for sourcing background footage, allowing ShortGPT to connect
-with the web and access a wide range of images and videos. - **Bing Image**:
-Bing Image is used for sourcing images, providing a comprehensive database for
-ShortGPT to retrieve relevant visuals. These technologies work together to
-provide a seamless and efficient experience in automating video and short
-content creation with AI. ## ð Contributing As an open-source project in a
-rapidly developing field, we are extremely open to contributions, whether it
-would be in the form of a new feature, improved infrastructure, or better
-documentation. ## ð Get in touch on Twitter ð¦ Keep up with the latest
-happenings, announcements, and insights about Short-GPT by checking out our
-Twitter accounts. Spark a conversation with our developer and the AI's own
-account for fascinating dialogues, latest news about the project, and more. -
-**Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ).
-Deep-dive into behind-the-scenes, project news, and related topics from the
-person behind ShortGPT. We're eager to interact with you and listen to your
-feedback, concepts, and experiences with Short-GPT. Come on board on Twitter
-and let's navigate the future of AI as a team! ð¡ð¤
+2. Once you're in the notebook, simply run the cells in order from top to
+bottom. You can do this by clicking on each cell and pressing the 'Play'
+button, or by using the keyboard . Enjoy using ShortGPT! # Instructions for
+running shortGPT This guide provides step-by-step instructions for installing
+ImageMagick and FFmpeg on your system, which are both required to do automated
+editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
+## Installation Steps Follow the instructions below to install ImageMagick,
+FFmpeg, and clone the shortGPT repository: ### Step 1 and 2, install Ffmpeg and
+ImageMagick For the updated installation steps, please follow Step 1 and 2 in
+our official documentation [docs.shortgpt.ai/docs/how-to-install](https://
+docs.shortgpt.ai/docs/how-to-install). ### Step 3: Clone the shortGPT
+Repository 1. Open a terminal or command prompt. 2. Execute the following
+command to clone the shortGPT repository: ``` git clone https://github.com/
+rayventura/shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a
+terminal or command prompt. 2. Navigate to the directory where `runShortGPT.py`
+is located (the cloned repo). 3. Execute the following command to install the
+required Python dependencies: ``` pip install -r requirements.txt ``` This
+command will install the necessary packages specified in the `requirements.txt`
+file. ## Running runShortGPT.py Web Interface Once you have successfully
+installed ImageMagick, FFmpeg, and the Python dependencies, you can run
+`runShortGPT.py` by following these steps: 1. Open a terminal or command
+prompt. 2. Navigate to the directory where `runShortGPT.py` is located (the
+cloned repo). 3. Execute the following command to run the script: ``` python
+runShortGPT.py ``` 4. After running the script, a Gradio interface should open
+at your local host on port 31415 (http://localhost:31415). ## Framework
+overview - ð¬ The `ContentShortEngine` is designed for creating shorts,
+handling tasks from script generation to final rendering, including adding
+YouTube metadata. - ð¥ The `ContentVideoEngine` is ideal for longer videos,
+taking care of tasks like generating audio, automatically sourcing background
+video footage, timing captions, and preparing background assets. - ð£ï¸ The
+`ContentTranslationEngine` is designed to dub and translate entire videos, from
+mainstream languages to more specific target languages. It takes a video file,
+or youtube link, transcribe it's audio, translates the content, voices it in a
+target language, adds captions , and gives back a new video, in a totally
+different language. - ðï¸ The automated `EditingEngine`, using Editing
+Markup Language and JSON, breaks down the editing process into manageable and
+customizable blocks, comprehensible to Large Language Models. ð¡ ShortGPT
+offers customization options to suit your needs, from language selection to
+watermark addition. ð§ As a framework, ShortGPT is adaptable and flexible,
+offering the potential for efficient, creative content creation. More
+documentation incomming, please be patient. ## Technologies Used ShortGPT
+utilizes the following technologies to power its functionality: - **Moviepy**:
+Moviepy is used for video editing, allowing ShortGPT to make video editing and
+rendering - **Openai**: Openai is used for automating the entire process,
+including generating scripts and prompts for LLM automated editing processes. -
+**ElevenLabs**: ElevenLabs is used for voice synthesis, supporting multiple
+languages for voiceover creation. - **EdgeTTS**: Microsoft's FREE EdgeTTS is
+used for voice synthesis, supporting way many more language than ElevenLabs
+currently. - **Pexels**: Pexels is used for sourcing background footage,
+allowing ShortGPT to connect with the web and access a wide range of images and
+videos. - **Bing Image**: Bing Image is used for sourcing images, providing a
+comprehensive database for ShortGPT to retrieve relevant visuals. These
+technologies work together to provide a seamless and efficient experience in
+automating video and short content creation with AI. ## ð Contributing As an
+open-source project in a rapidly developing field, we are extremely open to
+contributions, whether it would be in the form of a new feature, improved
+infrastructure, or better documentation. ## ð Get in touch on Twitter ð¦
+Keep up with the latest happenings, announcements, and insights about Short-GPT
+by checking out our Twitter accounts. Spark a conversation with our developer
+and the AI's own account for fascinating dialogues, latest news about the
+project, and more. - **Developer**: Stay updated [@RayVentura](https://
+twitter.com/RayVenturaHQ). Deep-dive into behind-the-scenes, project news, and
+related topics from the person behind ShortGPT. We're eager to interact with
+you and listen to your feedback, concepts, and experiences with Short-GPT. Come
+on board on Twitter and let's navigate the future of AI as a team! ð¡ð¤
                              [Star_History_Chart]
```

### Comparing `shortgpt-0.1.3/shortgpt.egg-info/SOURCES.txt` & `shortgpt-0.1.31/shortgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

