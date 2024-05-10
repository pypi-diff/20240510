# Comparing `tmp/ultima_scraper_api-2.2.26.tar.gz` & `tmp/ultima_scraper_api-2.2.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-2.2.26.tar", max compression
+gzip compressed data, was "ultima_scraper_api-2.2.27.tar", max compression
```

## Comparing `ultima_scraper_api-2.2.26.tar` & `ultima_scraper_api-2.2.27.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1250 2024-05-03 05:28:22.251305 ultima_scraper_api-2.2.26/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-2.2.26/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2670 2023-12-18 07:32:59.535607 ultima_scraper_api-2.2.26/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-2.2.26/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     3731 2023-11-30 04:05:19.333425 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     2469 2023-12-23 23:02:11.519743 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0     2121 2024-04-19 13:03:24.099066 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/auth_streamliner.py
--rw-r--r--   0        0        0      645 2023-11-30 04:11:43.238177 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     3078 2024-01-07 02:45:02.897270 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0     4702 2023-12-18 07:25:38.835846 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/authenticator.py
--rw-r--r--   0        0        0      249 2023-12-02 19:12:21.898179 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    13161 2024-01-05 16:32:00.286752 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6563 2023-12-08 09:33:53.172671 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0      655 2023-07-08 10:22:46.596423 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/comment_model.py
--rw-r--r--   0        0        0    10154 2024-01-19 07:32:56.430688 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     5901 2023-12-24 00:37:27.225759 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     7306 2023-12-08 09:34:03.579498 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3268 2023-12-08 09:34:06.692880 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0     1089 2023-11-30 08:28:59.843675 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/subscription_model.py
--rw-r--r--   0        0        0    27567 2024-01-06 09:15:49.418317 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     6779 2024-04-07 09:53:53.542364 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     3153 2024-04-19 11:24:28.858672 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0     6350 2024-04-19 11:24:56.548781 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/authenticator.py
--rw-r--r--   0        0        0      205 2023-11-29 18:32:12.431939 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    16913 2024-01-27 18:26:04.212500 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0     1162 2023-12-24 00:29:33.748277 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/chat_model.py
--rw-r--r--   0        0        0      767 2023-12-02 20:22:41.700921 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/comment_model.py
--rw-r--r--   0        0        0    13638 2024-01-27 18:49:15.248861 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      749 2023-12-16 09:18:58.087530 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2866 2024-04-19 16:10:51.488058 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py
--rw-r--r--   0        0        0     3398 2024-01-07 04:37:41.374763 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     6124 2023-12-29 18:58:00.754610 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
--rw-r--r--   0        0        0     3973 2023-12-16 08:52:44.831588 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0      287 2023-12-18 12:07:14.644579 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/stat.py
--rw-r--r--   0        0        0     1459 2023-12-16 08:53:28.469427 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0     1824 2023-11-30 06:17:33.423820 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
--rw-r--r--   0        0        0    34773 2024-04-19 11:22:51.908339 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0     2034 2023-12-24 00:53:00.148066 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/vault.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     7762 2024-04-19 16:01:23.321429 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     4145 2024-04-25 13:15:38.873678 ultima_scraper_api-2.2.26/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-2.2.26/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-07-11 08:47:19.301278 ultima_scraper_api-2.2.26/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.26/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0     1952 2023-12-02 23:30:30.482767 ultima_scraper_api-2.2.26/ultima_scraper_api/config.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.26/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.26/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-2.2.26/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1362 2023-12-02 21:48:17.148944 ultima_scraper_api-2.2.26/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-2.2.26/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-2.2.26/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    10552 2024-01-27 17:24:53.956943 ultima_scraper_api-2.2.26/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-2.2.26/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-2.2.26/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     2318 2024-04-19 11:26:51.545962 ultima_scraper_api-2.2.26/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-2.2.26/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      631 2023-10-08 19:23:00.177284 ultima_scraper_api-2.2.26/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2417 2023-12-23 22:49:39.932066 ultima_scraper_api-2.2.26/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    15648 2024-01-27 17:26:37.159460 ultima_scraper_api-2.2.26/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-2.2.26/ultima_scraper_api/models/__init__.py
--rw-r--r--   0        0        0      641 2023-12-02 23:28:01.235613 ultima_scraper_api-2.2.26/ultima_scraper_api/models/subscription_model.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-2.2.26/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1224 1970-01-01 00:00:00.000000 ultima_scraper_api-2.2.26/PKG-INFO
+-rw-r--r--   0        0        0     1250 2024-05-10 06:50:24.325489 ultima_scraper_api-2.2.27/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-2.2.27/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2670 2023-12-18 07:32:59.535607 ultima_scraper_api-2.2.27/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-2.2.27/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     3731 2023-11-30 04:05:19.333425 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     2469 2023-12-23 23:02:11.519743 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0     2121 2024-04-19 13:03:24.099066 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/auth_streamliner.py
+-rw-r--r--   0        0        0      645 2023-11-30 04:11:43.238177 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     3078 2024-01-07 02:45:02.897270 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0     4702 2023-12-18 07:25:38.835846 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/authenticator.py
+-rw-r--r--   0        0        0      249 2023-12-02 19:12:21.898179 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    13161 2024-01-05 16:32:00.286752 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6563 2023-12-08 09:33:53.172671 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0      655 2023-07-08 10:22:46.596423 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/comment_model.py
+-rw-r--r--   0        0        0    10154 2024-01-19 07:32:56.430688 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     5901 2023-12-24 00:37:27.225759 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     7306 2023-12-08 09:34:03.579498 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3268 2023-12-08 09:34:06.692880 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0     1089 2023-11-30 08:28:59.843675 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27567 2024-01-06 09:15:49.418317 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     6779 2024-04-07 09:53:53.542364 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     3153 2024-04-19 11:24:28.858672 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0     6350 2024-04-19 11:24:56.548781 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/authenticator.py
+-rw-r--r--   0        0        0      205 2023-11-29 18:32:12.431939 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    16913 2024-01-27 18:26:04.212500 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0     1162 2023-12-24 00:29:33.748277 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/chat_model.py
+-rw-r--r--   0        0        0      767 2023-12-02 20:22:41.700921 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/comment_model.py
+-rw-r--r--   0        0        0    13638 2024-01-27 18:49:15.248861 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      749 2023-12-16 09:18:58.087530 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2866 2024-04-19 16:10:51.488058 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py
+-rw-r--r--   0        0        0     3398 2024-01-07 04:37:41.374763 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     6124 2023-12-29 18:58:00.754610 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3973 2023-12-16 08:52:44.831588 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0      287 2023-12-18 12:07:14.644579 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/stat.py
+-rw-r--r--   0        0        0     1459 2023-12-16 08:53:28.469427 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1824 2023-11-30 06:17:33.423820 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    34773 2024-04-19 11:22:51.908339 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0     2034 2023-12-24 00:53:00.148066 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/vault.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     7762 2024-04-19 16:01:23.321429 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     4145 2024-04-25 13:15:38.873678 ultima_scraper_api-2.2.27/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-2.2.27/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-07-11 08:47:19.301278 ultima_scraper_api-2.2.27/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.27/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0     1982 2024-05-07 09:23:48.955094 ultima_scraper_api-2.2.27/ultima_scraper_api/config.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.27/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.27/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-2.2.27/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1362 2023-12-02 21:48:17.148944 ultima_scraper_api-2.2.27/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-2.2.27/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-2.2.27/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    10552 2024-01-27 17:24:53.956943 ultima_scraper_api-2.2.27/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-2.2.27/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-2.2.27/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     2318 2024-04-19 11:26:51.545962 ultima_scraper_api-2.2.27/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-2.2.27/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      631 2023-10-08 19:23:00.177284 ultima_scraper_api-2.2.27/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2417 2023-12-23 22:49:39.932066 ultima_scraper_api-2.2.27/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    15648 2024-01-27 17:26:37.159460 ultima_scraper_api-2.2.27/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-2.2.27/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      641 2023-12-02 23:28:01.235613 ultima_scraper_api-2.2.27/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-2.2.27/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1224 1970-01-01 00:00:00.000000 ultima_scraper_api-2.2.27/PKG-INFO
```

### Comparing `ultima_scraper_api-2.2.26/pyproject.toml` & `ultima_scraper_api-2.2.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "2.2.26"
+version = "2.2.27"
 description = ""
 authors = ["UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>"]
 packages = [{ include = "ultima_scraper_api" }]
 include = ["ultima_scraper_api/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
```

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/__init__.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/auth_streamliner.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/auth_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/authenticator.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/authenticator.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/comment_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/comment_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/subscription_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/authenticator.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/authenticator.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/chat_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/chat_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/comment_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/comment_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/only_drm.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/only_drm.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/classes/vault.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/classes/vault.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/apis/user_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/config.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,25 +54,25 @@
 class GlobalAPI(BaseModel):
     media_quality: MediaQuality = MediaQuality()
     webhooks: Webhooks = Webhooks()
 
 
 class OnlyFansAPIConfig(GlobalAPI):
     class OnlyFansCache(GlobalCache):
-        paid_content = 3600 * 1
+        paid_content:int = 3600 * 1
 
     dynamic_rules_url: str = "https://raw.githubusercontent.com/DATAHOARDERS/dynamic-rules/main/onlyfans.json"
-    cache = OnlyFansCache()
+    cache:OnlyFansCache = OnlyFansCache()
 
 
 class FanslyAPIConfig(GlobalAPI):
     class FanslyCache(GlobalCache):
         pass
 
-    cache = FanslyCache()
+    cache:FanslyCache = FanslyCache()
 
 
 class Sites(BaseModel):
     onlyfans: OnlyFansAPIConfig = OnlyFansAPIConfig()
     fansly: FanslyAPIConfig = FanslyAPIConfig()
 
     def get_settings(self, site_name: site_name_literals):
```

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-2.2.27/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-2.2.27/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/helpers/main_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/ultima_scraper_api/models/subscription_model.py` & `ultima_scraper_api-2.2.27/ultima_scraper_api/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.26/PKG-INFO` & `ultima_scraper_api-2.2.27/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 2.2.26
+Version: 2.2.27
 Summary: 
 Author: UltimaHoarder
 Author-email: 1285176+UltimaHoarder@users.noreply.github.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

