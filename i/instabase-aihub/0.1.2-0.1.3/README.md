# Comparing `tmp/instabase-aihub-0.1.2.tar.gz` & `tmp/instabase-aihub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instabase-aihub-0.1.2.tar", last modified: Thu May  2 21:43:39 2024, max compression
+gzip compressed data, was "instabase-aihub-0.1.3.tar", last modified: Fri May 10 00:14:28 2024, max compression
```

## Comparing `instabase-aihub-0.1.2.tar` & `instabase-aihub-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-02 21:43:39.173415 instabase-aihub-0.1.2/
--rw-r--r--   0 anil       (501) staff       (20)     1097 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/LICENSE
--rw-r--r--   0 anil       (501) staff       (20)     2825 2024-05-02 21:43:39.173208 instabase-aihub-0.1.2/PKG-INFO
--rw-r--r--   0 anil       (501) staff       (20)     2387 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/README.md
-drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-02 21:43:39.149249 instabase-aihub-0.1.2/aihub/
--rw-r--r--   0 anil       (501) staff       (20)     3179 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/aihub/__init__.py
--rw-r--r--   0 anil       (501) staff       (20)     6643 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/aihub/aihub.py
-drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-02 21:43:39.152351 instabase-aihub-0.1.2/aihub/api/
--rw-r--r--   0 anil       (501) staff       (20)      181 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/api/__init__.py
--rw-r--r--   0 anil       (501) staff       (20)    81385 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/api/batch_api.py
--rw-r--r--   0 anil       (501) staff       (20)    98256 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/api/conversation_api.py
--rw-r--r--   0 anil       (501) staff       (20)    50994 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/api/run_api.py
--rw-r--r--   0 anil       (501) staff       (20)    24892 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/api_client.py
--rw-r--r--   0 anil       (501) staff       (20)      674 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/api_response.py
--rw-r--r--   0 anil       (501) staff       (20)    14254 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/configuration.py
--rw-r--r--   0 anil       (501) staff       (20)     5463 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/exceptions.py
-drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-02 21:43:39.168800 instabase-aihub-0.1.2/aihub/models/
--rw-r--r--   0 anil       (501) staff       (20)     2552 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/__init__.py
--rw-r--r--   0 anil       (501) staff       (20)     2414 2024-05-02 21:43:18.000000 instabase-aihub-0.1.2/aihub/models/batch.py
--rw-r--r--   0 anil       (501) staff       (20)     2502 2024-05-02 21:43:18.000000 instabase-aihub-0.1.2/aihub/models/batch_deletion_job_response.py
--rw-r--r--   0 anil       (501) staff       (20)     3907 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/batch_info.py
--rw-r--r--   0 anil       (501) staff       (20)     3490 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/conversation.py
--rw-r--r--   0 anil       (501) staff       (20)     3123 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/conversation_response.py
--rw-r--r--   0 anil       (501) staff       (20)     3783 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/conversation_response_upload_status.py
--rw-r--r--   0 anil       (501) staff       (20)     2614 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/conversation_response_upload_status_failure_inner.py
--rw-r--r--   0 anil       (501) staff       (20)     2619 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/conversation_response_upload_status_success_inner.py
--rw-r--r--   0 anil       (501) staff       (20)     2782 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/conversation_summary.py
--rw-r--r--   0 anil       (501) staff       (20)     3164 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/converse_request.py
--rw-r--r--   0 anil       (501) staff       (20)     2715 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/create_batch_request.py
--rw-r--r--   0 anil       (501) staff       (20)     2559 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/delete_documents_from_conversation_request.py
--rw-r--r--   0 anil       (501) staff       (20)     3838 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document.py
--rw-r--r--   0 anil       (501) staff       (20)     3084 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_details.py
--rw-r--r--   0 anil       (501) staff       (20)     3082 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_field.py
--rw-r--r--   0 anil       (501) staff       (20)     2789 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_field_confidence.py
--rw-r--r--   0 anil       (501) staff       (20)     2950 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_metadata_response.py
--rw-r--r--   0 anil       (501) staff       (20)     2868 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_upload_response.py
--rw-r--r--   0 anil       (501) staff       (20)     3836 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_upload_response_upload_status.py
--rw-r--r--   0 anil       (501) staff       (20)     2737 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_upload_response_upload_status_failure_inner.py
--rw-r--r--   0 anil       (501) staff       (20)     2602 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/document_upload_response_upload_status_success_inner.py
--rw-r--r--   0 anil       (501) staff       (20)     2378 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/error.py
--rw-r--r--   0 anil       (501) staff       (20)     3108 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/file_with_documents.py
--rw-r--r--   0 anil       (501) staff       (20)     2712 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/job_status_response.py
--rw-r--r--   0 anil       (501) staff       (20)     2878 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/list_batches200_response.py
--rw-r--r--   0 anil       (501) staff       (20)     2996 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/list_conversations200_response.py
--rw-r--r--   0 anil       (501) staff       (20)     2655 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/prompt_response.py
--rw-r--r--   0 anil       (501) staff       (20)     3074 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/results_response.py
--rw-r--r--   0 anil       (501) staff       (20)     4035 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/run.py
--rw-r--r--   0 anil       (501) staff       (20)     3420 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/models/run_app_request.py
--rw-r--r--   0 anil       (501) staff       (20)        0 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/py.typed
--rw-r--r--   0 anil       (501) staff       (20)     8302 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/aihub/rest.py
-drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-02 21:43:39.172657 instabase-aihub-0.1.2/instabase_aihub.egg-info/
--rw-r--r--   0 anil       (501) staff       (20)     2825 2024-05-02 21:43:38.000000 instabase-aihub-0.1.2/instabase_aihub.egg-info/PKG-INFO
--rw-r--r--   0 anil       (501) staff       (20)     1804 2024-05-02 21:43:39.000000 instabase-aihub-0.1.2/instabase_aihub.egg-info/SOURCES.txt
--rw-r--r--   0 anil       (501) staff       (20)        1 2024-05-02 21:43:38.000000 instabase-aihub-0.1.2/instabase_aihub.egg-info/dependency_links.txt
--rw-r--r--   0 anil       (501) staff       (20)       76 2024-05-02 21:43:38.000000 instabase-aihub-0.1.2/instabase_aihub.egg-info/requires.txt
--rw-r--r--   0 anil       (501) staff       (20)        6 2024-05-02 21:43:38.000000 instabase-aihub-0.1.2/instabase_aihub.egg-info/top_level.txt
--rw-r--r--   0 anil       (501) staff       (20)      693 2024-05-02 21:43:19.000000 instabase-aihub-0.1.2/pyproject.toml
--rw-r--r--   0 anil       (501) staff       (20)       69 2024-05-02 21:43:39.173801 instabase-aihub-0.1.2/setup.cfg
--rw-r--r--   0 anil       (501) staff       (20)     1168 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/setup.py
-drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-02 21:43:39.172160 instabase-aihub-0.1.2/test/
--rw-r--r--   0 anil       (501) staff       (20)     5656 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/test/test_batch_api.py
--rw-r--r--   0 anil       (501) staff       (20)     6786 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/test/test_conversation_api.py
--rw-r--r--   0 anil       (501) staff       (20)     3443 2024-05-02 21:43:20.000000 instabase-aihub-0.1.2/test/test_run_api.py
+drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-10 00:14:28.018800 instabase-aihub-0.1.3/
+-rw-r--r--   0 anil       (501) staff       (20)     1097 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/LICENSE
+-rw-r--r--   0 anil       (501) staff       (20)     2825 2024-05-10 00:14:28.018583 instabase-aihub-0.1.3/PKG-INFO
+-rw-r--r--   0 anil       (501) staff       (20)     2387 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/README.md
+drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-10 00:14:27.995775 instabase-aihub-0.1.3/aihub/
+-rw-r--r--   0 anil       (501) staff       (20)     3179 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/__init__.py
+-rw-r--r--   0 anil       (501) staff       (20)     6892 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/aihub.py
+drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-10 00:14:27.997843 instabase-aihub-0.1.3/aihub/api/
+-rw-r--r--   0 anil       (501) staff       (20)      181 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/api/__init__.py
+-rw-r--r--   0 anil       (501) staff       (20)    81385 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/api/batch_api.py
+-rw-r--r--   0 anil       (501) staff       (20)    98256 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/api/conversation_api.py
+-rw-r--r--   0 anil       (501) staff       (20)    50994 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/api/run_api.py
+-rw-r--r--   0 anil       (501) staff       (20)    24892 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/api_client.py
+-rw-r--r--   0 anil       (501) staff       (20)      674 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/api_response.py
+-rw-r--r--   0 anil       (501) staff       (20)    14254 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/configuration.py
+-rw-r--r--   0 anil       (501) staff       (20)     5463 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/exceptions.py
+drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-10 00:14:28.014375 instabase-aihub-0.1.3/aihub/models/
+-rw-r--r--   0 anil       (501) staff       (20)     2552 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/models/__init__.py
+-rw-r--r--   0 anil       (501) staff       (20)     2414 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/batch.py
+-rw-r--r--   0 anil       (501) staff       (20)     2502 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/batch_deletion_job_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     3907 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/batch_info.py
+-rw-r--r--   0 anil       (501) staff       (20)     3490 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/conversation.py
+-rw-r--r--   0 anil       (501) staff       (20)     3123 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/conversation_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     3783 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/conversation_response_upload_status.py
+-rw-r--r--   0 anil       (501) staff       (20)     2614 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/conversation_response_upload_status_failure_inner.py
+-rw-r--r--   0 anil       (501) staff       (20)     2619 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/conversation_response_upload_status_success_inner.py
+-rw-r--r--   0 anil       (501) staff       (20)     2782 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/conversation_summary.py
+-rw-r--r--   0 anil       (501) staff       (20)     3164 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/converse_request.py
+-rw-r--r--   0 anil       (501) staff       (20)     2715 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/create_batch_request.py
+-rw-r--r--   0 anil       (501) staff       (20)     2559 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/delete_documents_from_conversation_request.py
+-rw-r--r--   0 anil       (501) staff       (20)     3838 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document.py
+-rw-r--r--   0 anil       (501) staff       (20)     3084 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_details.py
+-rw-r--r--   0 anil       (501) staff       (20)     3082 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_field.py
+-rw-r--r--   0 anil       (501) staff       (20)     2789 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_field_confidence.py
+-rw-r--r--   0 anil       (501) staff       (20)     2950 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_metadata_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     2868 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_upload_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     3836 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_upload_response_upload_status.py
+-rw-r--r--   0 anil       (501) staff       (20)     2737 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_upload_response_upload_status_failure_inner.py
+-rw-r--r--   0 anil       (501) staff       (20)     2602 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/document_upload_response_upload_status_success_inner.py
+-rw-r--r--   0 anil       (501) staff       (20)     2378 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/error.py
+-rw-r--r--   0 anil       (501) staff       (20)     3108 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/file_with_documents.py
+-rw-r--r--   0 anil       (501) staff       (20)     2712 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/job_status_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     2878 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/list_batches200_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     2996 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/list_conversations200_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     2655 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/prompt_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     3074 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/results_response.py
+-rw-r--r--   0 anil       (501) staff       (20)     4035 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/run.py
+-rw-r--r--   0 anil       (501) staff       (20)     3420 2024-05-10 00:14:15.000000 instabase-aihub-0.1.3/aihub/models/run_app_request.py
+-rw-r--r--   0 anil       (501) staff       (20)        0 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/py.typed
+-rw-r--r--   0 anil       (501) staff       (20)     8302 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/aihub/rest.py
+drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-10 00:14:28.018026 instabase-aihub-0.1.3/instabase_aihub.egg-info/
+-rw-r--r--   0 anil       (501) staff       (20)     2825 2024-05-10 00:14:27.000000 instabase-aihub-0.1.3/instabase_aihub.egg-info/PKG-INFO
+-rw-r--r--   0 anil       (501) staff       (20)     1804 2024-05-10 00:14:27.000000 instabase-aihub-0.1.3/instabase_aihub.egg-info/SOURCES.txt
+-rw-r--r--   0 anil       (501) staff       (20)        1 2024-05-10 00:14:27.000000 instabase-aihub-0.1.3/instabase_aihub.egg-info/dependency_links.txt
+-rw-r--r--   0 anil       (501) staff       (20)       76 2024-05-10 00:14:27.000000 instabase-aihub-0.1.3/instabase_aihub.egg-info/requires.txt
+-rw-r--r--   0 anil       (501) staff       (20)        6 2024-05-10 00:14:27.000000 instabase-aihub-0.1.3/instabase_aihub.egg-info/top_level.txt
+-rw-r--r--   0 anil       (501) staff       (20)      693 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/pyproject.toml
+-rw-r--r--   0 anil       (501) staff       (20)       69 2024-05-10 00:14:28.019197 instabase-aihub-0.1.3/setup.cfg
+-rw-r--r--   0 anil       (501) staff       (20)     1168 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/setup.py
+drwxr-xr-x   0 anil       (501) staff       (20)        0 2024-05-10 00:14:28.017457 instabase-aihub-0.1.3/test/
+-rw-r--r--   0 anil       (501) staff       (20)     5656 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/test/test_batch_api.py
+-rw-r--r--   0 anil       (501) staff       (20)     6786 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/test/test_conversation_api.py
+-rw-r--r--   0 anil       (501) staff       (20)     3443 2024-05-10 00:14:16.000000 instabase-aihub-0.1.3/test/test_run_api.py
```

### Comparing `instabase-aihub-0.1.2/LICENSE` & `instabase-aihub-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/PKG-INFO` & `instabase-aihub-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instabase-aihub
-Version: 0.1.2
+Version: 0.1.3
 Summary: AI Hub API
 Home-page: https://platform.instabase.com/docs/aihub/
 Author: Instabase Support
 Author-email: support@instabase.com
 License: MIT
 Keywords: Instabase,AI Hub API
 Description-Content-Type: text/markdown
```

### Comparing `instabase-aihub-0.1.2/README.md` & `instabase-aihub-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/__init__.py` & `instabase-aihub-0.1.3/aihub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: support@instabase.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 # import apis into sdk package
 from aihub.api.batch_api import BatchApi
 from aihub.api.conversation_api import ConversationApi
 from aihub.api.run_api import RunApi
 
 # import ApiClient
```

### Comparing `instabase-aihub-0.1.2/aihub/aihub.py` & `instabase-aihub-0.1.3/aihub/aihub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from aihub.api.batch_api import BatchApi
 from aihub.api.conversation_api import ConversationApi
 from aihub.api.run_api import RunApi
 from aihub.api_client import ApiClient
-import os
 
 
 class AIHub:
 
   def __init__(self,
                api_key,
                ib_context=None,
@@ -135,29 +134,36 @@
 
   class Runs:
 
     def __init__(self, api_instance, ib_context):
       self.api_instance = api_instance
       self.ib_context = ib_context
 
-    def run(self, app_name=None, files=[], app_id=None, settings=None):
+    def run(self,
+            app_name=None,
+            app_id=None,
+            files=[],
+            owner=None,
+            settings=None):
       results = self.api_instance.run_app_sync(
           app_name=app_name,
-          files=files,
           app_id=app_id,
+          files=files,
+          owner=owner,
           settings=settings,
           ib_context=self.ib_context)
       return results
 
     def create(self,
                app_name=None,
-               batch_id=None,
                app_id=None,
+               batch_id=None,
                input_dir=None,
                output_dir=None,
+               owner=None,
                settings=None):
       # Validate that one of batch_id or input_dir is provided
       if not batch_id and not input_dir:
         raise ValueError("Either batch_id or input_dir is required.")
 
       # Construct the dictionary with only the set values
       run_details = {}
@@ -166,16 +172,24 @@
       elif app_id:  # Use elif because only one of them needs to be set
         run_details['app_id'] = app_id
 
       if batch_id:
         run_details['batch_id'] = batch_id
       elif input_dir:  # Use elif for the same reason
         run_details['input_dir'] = input_dir
-      run_details['output_dir'] = output_dir
-      run_details['settings'] = settings
+
+      if output_dir is not None:
+        run_details['output_dir'] = output_dir
+
+      if settings is not None:
+        run_details['settings'] = settings
+
+      if owner is not None:
+        run_details['owner'] = owner
+
       # Call run_app with the constructed dictionary
       run = self.api_instance.run_app(run_details, ib_context=self.ib_context)
       return run
 
     def status(self, id):
       status = self.api_instance.get_run_status(id, ib_context=self.ib_context)
       return status
```

### Comparing `instabase-aihub-0.1.2/aihub/api/batch_api.py` & `instabase-aihub-0.1.3/aihub/api/batch_api.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/api/conversation_api.py` & `instabase-aihub-0.1.3/aihub/api/conversation_api.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/api/run_api.py` & `instabase-aihub-0.1.3/aihub/api/run_api.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/api_client.py` & `instabase-aihub-0.1.3/aihub/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `instabase-aihub-0.1.2/aihub/api_response.py` & `instabase-aihub-0.1.3/aihub/api_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/configuration.py` & `instabase-aihub-0.1.3/aihub/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.1.2".\
+               "SDK Package Version: 0.1.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `instabase-aihub-0.1.2/aihub/exceptions.py` & `instabase-aihub-0.1.3/aihub/exceptions.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/__init__.py` & `instabase-aihub-0.1.3/aihub/models/__init__.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/batch.py` & `instabase-aihub-0.1.3/aihub/models/batch.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/batch_deletion_job_response.py` & `instabase-aihub-0.1.3/aihub/models/batch_deletion_job_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/batch_info.py` & `instabase-aihub-0.1.3/aihub/models/batch_info.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/conversation.py` & `instabase-aihub-0.1.3/aihub/models/conversation.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/conversation_response.py` & `instabase-aihub-0.1.3/aihub/models/conversation_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/conversation_response_upload_status.py` & `instabase-aihub-0.1.3/aihub/models/conversation_response_upload_status.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/conversation_response_upload_status_failure_inner.py` & `instabase-aihub-0.1.3/aihub/models/conversation_response_upload_status_failure_inner.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/conversation_response_upload_status_success_inner.py` & `instabase-aihub-0.1.3/aihub/models/conversation_response_upload_status_success_inner.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/conversation_summary.py` & `instabase-aihub-0.1.3/aihub/models/conversation_summary.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/converse_request.py` & `instabase-aihub-0.1.3/aihub/models/converse_request.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/create_batch_request.py` & `instabase-aihub-0.1.3/aihub/models/create_batch_request.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/delete_documents_from_conversation_request.py` & `instabase-aihub-0.1.3/aihub/models/delete_documents_from_conversation_request.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document.py` & `instabase-aihub-0.1.3/aihub/models/document.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_details.py` & `instabase-aihub-0.1.3/aihub/models/document_details.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_field.py` & `instabase-aihub-0.1.3/aihub/models/document_field.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_field_confidence.py` & `instabase-aihub-0.1.3/aihub/models/document_field_confidence.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_metadata_response.py` & `instabase-aihub-0.1.3/aihub/models/document_metadata_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_upload_response.py` & `instabase-aihub-0.1.3/aihub/models/document_upload_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_upload_response_upload_status.py` & `instabase-aihub-0.1.3/aihub/models/document_upload_response_upload_status.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_upload_response_upload_status_failure_inner.py` & `instabase-aihub-0.1.3/aihub/models/document_upload_response_upload_status_failure_inner.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/document_upload_response_upload_status_success_inner.py` & `instabase-aihub-0.1.3/aihub/models/document_upload_response_upload_status_success_inner.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/error.py` & `instabase-aihub-0.1.3/aihub/models/error.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/file_with_documents.py` & `instabase-aihub-0.1.3/aihub/models/file_with_documents.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/job_status_response.py` & `instabase-aihub-0.1.3/aihub/models/job_status_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/list_batches200_response.py` & `instabase-aihub-0.1.3/aihub/models/list_batches200_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/list_conversations200_response.py` & `instabase-aihub-0.1.3/aihub/models/list_conversations200_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/prompt_response.py` & `instabase-aihub-0.1.3/aihub/models/prompt_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/results_response.py` & `instabase-aihub-0.1.3/aihub/models/results_response.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/run.py` & `instabase-aihub-0.1.3/aihub/models/run.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/models/run_app_request.py` & `instabase-aihub-0.1.3/aihub/models/run_app_request.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/aihub/rest.py` & `instabase-aihub-0.1.3/aihub/rest.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/instabase_aihub.egg-info/PKG-INFO` & `instabase-aihub-0.1.3/instabase_aihub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instabase-aihub
-Version: 0.1.2
+Version: 0.1.3
 Summary: AI Hub API
 Home-page: https://platform.instabase.com/docs/aihub/
 Author: Instabase Support
 Author-email: support@instabase.com
 License: MIT
 Keywords: Instabase,AI Hub API
 Description-Content-Type: text/markdown
```

### Comparing `instabase-aihub-0.1.2/instabase_aihub.egg-info/SOURCES.txt` & `instabase-aihub-0.1.3/instabase_aihub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/pyproject.toml` & `instabase-aihub-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aihub"
-version = "0.1.2"
+version = "0.1.3"
 description = "AI Hub API"
 authors = ["Instabase Support <support@instabase.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "AI Hub API"]
 include = ["aihub/py.typed"]
```

### Comparing `instabase-aihub-0.1.2/setup.py` & `instabase-aihub-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/test/test_batch_api.py` & `instabase-aihub-0.1.3/test/test_batch_api.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/test/test_conversation_api.py` & `instabase-aihub-0.1.3/test/test_conversation_api.py`

 * *Files identical despite different names*

### Comparing `instabase-aihub-0.1.2/test/test_run_api.py` & `instabase-aihub-0.1.3/test/test_run_api.py`

 * *Files identical despite different names*

