# Comparing `tmp/SquirroClient-3.9.6.tar.gz` & `tmp/SquirroClient-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SquirroClient-3.9.6.tar", last modified: Fri Feb 16 10:39:08 2024, max compression
+gzip compressed data, was "SquirroClient-3.9.7.tar", last modified: Fri Mar  1 09:33:15 2024, max compression
```

## Comparing `SquirroClient-3.9.6.tar` & `SquirroClient-3.9.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 10:39:08.815060 SquirroClient-3.9.6/
--rw-r--r--   0 root         (0) root         (0)       12 2022-09-02 15:25:32.000000 SquirroClient-3.9.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      905 2024-02-16 10:39:08.815060 SquirroClient-3.9.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      238 2022-09-02 15:25:32.000000 SquirroClient-3.9.6/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 10:39:08.809060 SquirroClient-3.9.6/SquirroClient.egg-info/
--rw-r--r--   0 root         (0) root         (0)      905 2024-02-16 10:39:08.000000 SquirroClient-3.9.6/SquirroClient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1919 2024-02-16 10:39:08.000000 SquirroClient-3.9.6/SquirroClient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 10:39:08.000000 SquirroClient-3.9.6/SquirroClient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-02-16 10:39:08.000000 SquirroClient-3.9.6/SquirroClient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-16 10:39:08.000000 SquirroClient-3.9.6/SquirroClient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-16 10:39:08.815060 SquirroClient-3.9.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1300 2024-02-16 10:39:08.000000 SquirroClient-3.9.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 10:39:08.810060 SquirroClient-3.9.6/squirro_client/
--rw-r--r--   0 root         (0) root         (0)      517 2024-02-16 10:39:08.000000 SquirroClient-3.9.6/squirro_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17143 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/base.py
--rw-r--r--   0 root         (0) root         (0)    11588 2023-03-22 13:13:55.000000 SquirroClient-3.9.6/squirro_client/document_uploader.py
--rw-r--r--   0 root         (0) root         (0)     2049 2022-11-11 12:29:55.000000 SquirroClient-3.9.6/squirro_client/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3007 2023-01-11 18:47:03.000000 SquirroClient-3.9.6/squirro_client/internal.py
--rw-r--r--   0 root         (0) root         (0)    27024 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/item_uploader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 10:39:08.815060 SquirroClient-3.9.6/squirro_client/topic/
--rw-r--r--   0 root         (0) root         (0)    75143 2024-02-16 10:30:29.000000 SquirroClient-3.9.6/squirro_client/topic/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12108 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/communities.py
--rw-r--r--   0 root         (0) root         (0)     5739 2024-02-16 10:30:29.000000 SquirroClient-3.9.6/squirro_client/topic/community_subscription.py
--rw-r--r--   0 root         (0) root         (0)     9745 2024-02-16 10:30:29.000000 SquirroClient-3.9.6/squirro_client/topic/community_types.py
--rw-r--r--   0 root         (0) root         (0)    15281 2024-01-19 18:57:06.000000 SquirroClient-3.9.6/squirro_client/topic/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4444 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/contributingrecords.py
--rw-r--r--   0 root         (0) root         (0)    27783 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/dashboards.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/email_templates.py
--rw-r--r--   0 root         (0) root         (0)     6651 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/enrichments.py
--rw-r--r--   0 root         (0) root         (0)     2950 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/entities.py
--rw-r--r--   0 root         (0) root         (0)     8152 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/facets.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-01-11 18:47:03.000000 SquirroClient-3.9.6/squirro_client/topic/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-05-30 19:11:26.000000 SquirroClient-3.9.6/squirro_client/topic/globaltemp.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/guidefiles.py
--rw-r--r--   0 root         (0) root         (0)    17837 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/machinelearning.py
--rw-r--r--   0 root         (0) root         (0)     3699 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/ml_candidate_set.py
--rw-r--r--   0 root         (0) root         (0)    18842 2023-11-10 14:54:18.000000 SquirroClient-3.9.6/squirro_client/topic/ml_groundtruth.py
--rw-r--r--   0 root         (0) root         (0)     7110 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/ml_model.py
--rw-r--r--   0 root         (0) root         (0)     7838 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/ml_publish.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-03-22 13:13:55.000000 SquirroClient-3.9.6/squirro_client/topic/ml_sentence_splitter.py
--rw-r--r--   0 root         (0) root         (0)     2723 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/ml_template.py
--rw-r--r--   0 root         (0) root         (0)     6535 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/ml_user_feedback.py
--rw-r--r--   0 root         (0) root         (0)     6783 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/notes.py
--rw-r--r--   0 root         (0) root         (0)    10022 2023-01-11 18:47:03.000000 SquirroClient-3.9.6/squirro_client/topic/objects.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/pipeline_sections.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/pipeline_status.py
--rw-r--r--   0 root         (0) root         (0)    16021 2023-09-29 12:34:05.000000 SquirroClient-3.9.6/squirro_client/topic/pipeline_workflows.py
--rw-r--r--   0 root         (0) root         (0)     3797 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/project_translations.py
--rw-r--r--   0 root         (0) root         (0)    37604 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/projects.py
--rw-r--r--   0 root         (0) root         (0)     9190 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/savedsearches.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/smart_answers.py
--rw-r--r--   0 root         (0) root         (0)    16260 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/smartfilters.py
--rw-r--r--   0 root         (0) root         (0)    31093 2024-01-19 18:57:06.000000 SquirroClient-3.9.6/squirro_client/topic/sources.py
--rw-r--r--   0 root         (0) root         (0)     9472 2023-01-11 18:47:03.000000 SquirroClient-3.9.6/squirro_client/topic/subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     2067 2022-09-02 15:25:32.000000 SquirroClient-3.9.6/squirro_client/topic/suggest_images.py
--rw-r--r--   0 root         (0) root         (0)     5593 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/synonyms.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/tasks.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/themes.py
--rw-r--r--   0 root         (0) root         (0)    20851 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/trenddetection.py
--rw-r--r--   0 root         (0) root         (0)    11092 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/topic/widgets_assets.py
--rw-r--r--   0 root         (0) root         (0)    28176 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/user.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-09-18 11:11:40.000000 SquirroClient-3.9.6/squirro_client/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 09:33:15.532454 SquirroClient-3.9.7/
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-02 17:52:25.000000 SquirroClient-3.9.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      905 2024-03-01 09:33:15.532454 SquirroClient-3.9.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      238 2022-09-02 17:52:25.000000 SquirroClient-3.9.7/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 09:33:15.526454 SquirroClient-3.9.7/SquirroClient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      905 2024-03-01 09:33:15.000000 SquirroClient-3.9.7/SquirroClient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-03-01 09:33:15.000000 SquirroClient-3.9.7/SquirroClient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 09:33:15.000000 SquirroClient-3.9.7/SquirroClient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-03-01 09:33:15.000000 SquirroClient-3.9.7/SquirroClient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-03-01 09:33:15.000000 SquirroClient-3.9.7/SquirroClient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-01 09:33:15.532454 SquirroClient-3.9.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-03-01 09:33:14.000000 SquirroClient-3.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 09:33:15.527454 SquirroClient-3.9.7/squirro_client/
+-rw-r--r--   0 root         (0) root         (0)      517 2024-03-01 09:33:14.000000 SquirroClient-3.9.7/squirro_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17143 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/base.py
+-rw-r--r--   0 root         (0) root         (0)    11588 2023-07-12 18:41:04.000000 SquirroClient-3.9.7/squirro_client/document_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2022-11-11 15:50:29.000000 SquirroClient-3.9.7/squirro_client/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-01-23 22:44:30.000000 SquirroClient-3.9.7/squirro_client/internal.py
+-rw-r--r--   0 root         (0) root         (0)    27024 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/item_uploader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 09:33:15.532454 SquirroClient-3.9.7/squirro_client/topic/
+-rw-r--r--   0 root         (0) root         (0)    75143 2024-02-16 10:28:26.000000 SquirroClient-3.9.7/squirro_client/topic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12108 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/communities.py
+-rw-r--r--   0 root         (0) root         (0)     5739 2024-02-16 10:28:26.000000 SquirroClient-3.9.7/squirro_client/topic/community_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     9745 2024-02-16 10:28:26.000000 SquirroClient-3.9.7/squirro_client/topic/community_types.py
+-rw-r--r--   0 root         (0) root         (0)    15281 2024-01-19 19:26:29.000000 SquirroClient-3.9.7/squirro_client/topic/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/contributingrecords.py
+-rw-r--r--   0 root         (0) root         (0)    27783 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/dashboards.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/email_templates.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/enrichments.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/entities.py
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/facets.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-01-23 22:44:30.000000 SquirroClient-3.9.7/squirro_client/topic/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-12 18:41:04.000000 SquirroClient-3.9.7/squirro_client/topic/globaltemp.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/guidefiles.py
+-rw-r--r--   0 root         (0) root         (0)    17837 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/machinelearning.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/ml_candidate_set.py
+-rw-r--r--   0 root         (0) root         (0)    18842 2023-11-10 15:31:48.000000 SquirroClient-3.9.7/squirro_client/topic/ml_groundtruth.py
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/ml_model.py
+-rw-r--r--   0 root         (0) root         (0)     7838 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/ml_publish.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-07-12 18:41:04.000000 SquirroClient-3.9.7/squirro_client/topic/ml_sentence_splitter.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/ml_template.py
+-rw-r--r--   0 root         (0) root         (0)     6535 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/ml_user_feedback.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/notes.py
+-rw-r--r--   0 root         (0) root         (0)    10022 2023-01-23 22:44:30.000000 SquirroClient-3.9.7/squirro_client/topic/objects.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/pipeline_sections.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/pipeline_status.py
+-rw-r--r--   0 root         (0) root         (0)    16021 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/pipeline_workflows.py
+-rw-r--r--   0 root         (0) root         (0)     3797 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/project_translations.py
+-rw-r--r--   0 root         (0) root         (0)    37604 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/projects.py
+-rw-r--r--   0 root         (0) root         (0)     9190 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/savedsearches.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/smart_answers.py
+-rw-r--r--   0 root         (0) root         (0)    16260 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/smartfilters.py
+-rw-r--r--   0 root         (0) root         (0)    31093 2024-01-19 19:26:29.000000 SquirroClient-3.9.7/squirro_client/topic/sources.py
+-rw-r--r--   0 root         (0) root         (0)     9472 2023-01-11 22:15:35.000000 SquirroClient-3.9.7/squirro_client/topic/subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2022-09-02 17:52:25.000000 SquirroClient-3.9.7/squirro_client/topic/suggest_images.py
+-rw-r--r--   0 root         (0) root         (0)     5593 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/synonyms.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/themes.py
+-rw-r--r--   0 root         (0) root         (0)    20851 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/trenddetection.py
+-rw-r--r--   0 root         (0) root         (0)    11092 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/topic/widgets_assets.py
+-rw-r--r--   0 root         (0) root         (0)    28176 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/user.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-09-29 12:50:00.000000 SquirroClient-3.9.7/squirro_client/util.py
```

### Comparing `SquirroClient-3.9.6/PKG-INFO` & `SquirroClient-3.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SquirroClient
-Version: 3.9.6
+Version: 3.9.7
 Summary: Python client for the Squirro API
 Home-page: http://dev.squirro.com/docs/tools/python/index.html
 Author: Squirro Team
 Author-email: support@squirro.com
 License: Commercial
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SquirroClient-3.9.6/SquirroClient.egg-info/PKG-INFO` & `SquirroClient-3.9.7/SquirroClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SquirroClient
-Version: 3.9.6
+Version: 3.9.7
 Summary: Python client for the Squirro API
 Home-page: http://dev.squirro.com/docs/tools/python/index.html
 Author: Squirro Team
 Author-email: support@squirro.com
 License: Commercial
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SquirroClient-3.9.6/SquirroClient.egg-info/SOURCES.txt` & `SquirroClient-3.9.7/SquirroClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/setup.py` & `SquirroClient-3.9.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 
 from setuptools import find_packages, setup
 
 install_requires = open("requirements.txt").read().splitlines()
 
 # Note: This variable is matched in the `make publish-client` sed command to set a static version for a release.
-__SQUIRRO_VERSION__ = "3.9.6"
+__SQUIRRO_VERSION__ = "3.9.7"
 
 setup(
     name="SquirroClient",
     # Version number also needs to be updated in squirro_client/__init__.py
     version=__SQUIRRO_VERSION__,
     description="Python client for the Squirro API",
     long_description=open("README").read(),
```

### Comparing `SquirroClient-3.9.6/squirro_client/__init__.py` & `SquirroClient-3.9.7/squirro_client/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 from .base import SquirroClient
 from .document_uploader import DocumentUploader
 from .exceptions import *  # noqa: F403
 from .item_uploader import ItemUploader
 
 # Note: This variable is matched in the `make publish-client` sed command to set a static version for a release.
-__SQUIRRO_VERSION__ = "3.9.6"
+__SQUIRRO_VERSION__ = "3.9.7"
 __version__ = __SQUIRRO_VERSION__
```

### Comparing `SquirroClient-3.9.6/squirro_client/base.py` & `SquirroClient-3.9.7/squirro_client/base.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/document_uploader.py` & `SquirroClient-3.9.7/squirro_client/document_uploader.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/exceptions.py` & `SquirroClient-3.9.7/squirro_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/internal.py` & `SquirroClient-3.9.7/squirro_client/internal.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/item_uploader.py` & `SquirroClient-3.9.7/squirro_client/item_uploader.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/__init__.py` & `SquirroClient-3.9.7/squirro_client/topic/__init__.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/communities.py` & `SquirroClient-3.9.7/squirro_client/topic/communities.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/community_subscription.py` & `SquirroClient-3.9.7/squirro_client/topic/community_subscription.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/community_types.py` & `SquirroClient-3.9.7/squirro_client/topic/community_types.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/configuration.py` & `SquirroClient-3.9.7/squirro_client/topic/configuration.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/contributingrecords.py` & `SquirroClient-3.9.7/squirro_client/topic/contributingrecords.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/dashboards.py` & `SquirroClient-3.9.7/squirro_client/topic/dashboards.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/email_templates.py` & `SquirroClient-3.9.7/squirro_client/topic/email_templates.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/enrichments.py` & `SquirroClient-3.9.7/squirro_client/topic/enrichments.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/entities.py` & `SquirroClient-3.9.7/squirro_client/topic/entities.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/facets.py` & `SquirroClient-3.9.7/squirro_client/topic/facets.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/file_upload.py` & `SquirroClient-3.9.7/squirro_client/topic/file_upload.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/globaltemp.py` & `SquirroClient-3.9.7/squirro_client/topic/globaltemp.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/guidefiles.py` & `SquirroClient-3.9.7/squirro_client/topic/guidefiles.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/machinelearning.py` & `SquirroClient-3.9.7/squirro_client/topic/machinelearning.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/ml_candidate_set.py` & `SquirroClient-3.9.7/squirro_client/topic/ml_candidate_set.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/ml_groundtruth.py` & `SquirroClient-3.9.7/squirro_client/topic/ml_groundtruth.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/ml_model.py` & `SquirroClient-3.9.7/squirro_client/topic/ml_model.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/ml_publish.py` & `SquirroClient-3.9.7/squirro_client/topic/ml_publish.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/ml_sentence_splitter.py` & `SquirroClient-3.9.7/squirro_client/topic/ml_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/ml_template.py` & `SquirroClient-3.9.7/squirro_client/topic/ml_template.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/ml_user_feedback.py` & `SquirroClient-3.9.7/squirro_client/topic/ml_user_feedback.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/notes.py` & `SquirroClient-3.9.7/squirro_client/topic/notes.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/objects.py` & `SquirroClient-3.9.7/squirro_client/topic/objects.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/pipeline_sections.py` & `SquirroClient-3.9.7/squirro_client/topic/pipeline_sections.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/pipeline_status.py` & `SquirroClient-3.9.7/squirro_client/topic/pipeline_status.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/pipeline_workflows.py` & `SquirroClient-3.9.7/squirro_client/topic/pipeline_workflows.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/project_translations.py` & `SquirroClient-3.9.7/squirro_client/topic/project_translations.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/projects.py` & `SquirroClient-3.9.7/squirro_client/topic/projects.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/savedsearches.py` & `SquirroClient-3.9.7/squirro_client/topic/savedsearches.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/smart_answers.py` & `SquirroClient-3.9.7/squirro_client/topic/smart_answers.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/smartfilters.py` & `SquirroClient-3.9.7/squirro_client/topic/smartfilters.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/sources.py` & `SquirroClient-3.9.7/squirro_client/topic/sources.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/subscriptions.py` & `SquirroClient-3.9.7/squirro_client/topic/subscriptions.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/suggest_images.py` & `SquirroClient-3.9.7/squirro_client/topic/suggest_images.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/synonyms.py` & `SquirroClient-3.9.7/squirro_client/topic/synonyms.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/tasks.py` & `SquirroClient-3.9.7/squirro_client/topic/tasks.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/themes.py` & `SquirroClient-3.9.7/squirro_client/topic/themes.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/trenddetection.py` & `SquirroClient-3.9.7/squirro_client/topic/trenddetection.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/topic/widgets_assets.py` & `SquirroClient-3.9.7/squirro_client/topic/widgets_assets.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/user.py` & `SquirroClient-3.9.7/squirro_client/user.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.9.6/squirro_client/util.py` & `SquirroClient-3.9.7/squirro_client/util.py`

 * *Files identical despite different names*

