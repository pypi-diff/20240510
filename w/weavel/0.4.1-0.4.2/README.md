# Comparing `tmp/weavel-0.4.1.tar.gz` & `tmp/weavel-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weavel-0.4.1.tar", last modified: Fri Apr  5 02:57:23 2024, max compression
+gzip compressed data, was "weavel-0.4.2.tar", last modified: Fri May 10 09:48:49 2024, max compression
```

## Comparing `weavel-0.4.1.tar` & `weavel-0.4.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.145640 weavel-0.4.1/
--rw-r--r--   0 jypark     (501) staff       (20)        0 2024-01-15 02:29:57.000000 weavel-0.4.1/LICENSE
--rw-r--r--   0 jypark     (501) staff       (20)      406 2024-04-05 02:57:23.145516 weavel-0.4.1/PKG-INFO
--rw-r--r--   0 jypark     (501) staff       (20)       15 2024-02-08 04:16:27.000000 weavel-0.4.1/README.md
--rw-r--r--   0 jypark     (501) staff       (20)       38 2024-04-05 02:57:23.145685 weavel-0.4.1/setup.cfg
--rw-r--r--   0 jypark     (501) staff       (20)     1244 2024-04-05 02:54:59.000000 weavel-0.4.1/setup.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.139823 weavel-0.4.1/testapp/
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.140324 weavel-0.4.1/testapp/daily_dialog/
--rw-r--r--   0 jypark     (501) staff       (20)     9480 2024-02-06 10:50:36.000000 weavel-0.4.1/testapp/daily_dialog/run_qa_extractor.py
--rw-r--r--   0 jypark     (501) staff       (20)     8672 2024-02-06 10:50:37.000000 weavel-0.4.1/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py
--rw-r--r--   0 jypark     (501) staff       (20)     4110 2024-02-06 12:05:08.000000 weavel-0.4.1/testapp/daily_dialog/save_to_db.py
--rw-r--r--   0 jypark     (501) staff       (20)     1298 2024-03-21 06:59:25.000000 weavel-0.4.1/testapp/demo.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.140762 weavel-0.4.1/testapp/py_files/
--rw-r--r--   0 jypark     (501) staff       (20)     1065 2024-01-24 05:01:55.000000 weavel-0.4.1/testapp/py_files/duplicate_log_test.py
--rw-r--r--   0 jypark     (501) staff       (20)     1892 2024-01-30 03:05:12.000000 weavel-0.4.1/testapp/py_files/poe_test.py
--rw-r--r--   0 jypark     (501) staff       (20)     1068 2024-01-24 07:27:52.000000 weavel-0.4.1/testapp/py_files/save_mock_data.py
--rw-r--r--   0 jypark     (501) staff       (20)     1160 2024-01-24 11:29:54.000000 weavel-0.4.1/testapp/py_files/save_mock_retention_data.py
--rw-r--r--   0 jypark     (501) staff       (20)    43795 2024-03-22 07:15:41.000000 weavel-0.4.1/testapp/test.py
--rw-r--r--   0 jypark     (501) staff       (20)      278 2024-04-05 02:56:14.000000 weavel-0.4.1/testapp/test_identify.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.138949 weavel-0.4.1/venv/
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.143127 weavel-0.4.1/venv/bin/
--rwxr-xr-x   0 jypark     (501) staff       (20)     8236 2024-02-02 10:25:14.000000 weavel-0.4.1/venv/bin/pwiz.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      648 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2html.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      770 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 jypark     (501) staff       (20)     1105 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      847 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      670 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2man.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      836 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      642 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      655 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      691 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      927 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      656 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      724 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rstpep2html.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.143970 weavel-0.4.1/weavel/
--rw-r--r--   0 jypark     (501) staff       (20)      107 2024-04-05 02:56:10.000000 weavel-0.4.1/weavel/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     6063 2024-02-08 04:18:02.000000 weavel-0.4.1/weavel/_api_client.py
--rw-r--r--   0 jypark     (501) staff       (20)     1692 2024-04-05 02:11:37.000000 weavel-0.4.1/weavel/_buffer_storage.py
--rw-r--r--   0 jypark     (501) staff       (20)      211 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/_constants.py
--rw-r--r--   0 jypark     (501) staff       (20)    10005 2024-04-05 02:24:57.000000 weavel-0.4.1/weavel/_worker.py
--rw-r--r--   0 jypark     (501) staff       (20)     5824 2024-04-05 02:54:30.000000 weavel-0.4.1/weavel/client.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.145012 weavel-0.4.1/weavel/poe/
--rw-r--r--   0 jypark     (501) staff       (20)       58 2024-01-30 04:23:45.000000 weavel-0.4.1/weavel/poe/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     1749 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/poe/_poe_buffer_storage.py
--rw-r--r--   0 jypark     (501) staff       (20)     4756 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/poe/_poe_worker.py
--rw-r--r--   0 jypark     (501) staff       (20)     1278 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/poe/poe_client.py
--rw-r--r--   0 jypark     (501) staff       (20)     2701 2024-04-05 02:24:52.000000 weavel-0.4.1/weavel/types.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.145337 weavel-0.4.1/weavel/utils/
--rw-r--r--   0 jypark     (501) staff       (20)       43 2024-01-15 06:20:46.000000 weavel-0.4.1/weavel/utils/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     1134 2024-01-15 05:54:15.000000 weavel-0.4.1/weavel/utils/crypto.py
--rw-r--r--   0 jypark     (501) staff       (20)      679 2024-01-15 11:33:18.000000 weavel-0.4.1/weavel/utils/logger.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.144531 weavel-0.4.1/weavel.egg-info/
--rw-r--r--   0 jypark     (501) staff       (20)      406 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/PKG-INFO
--rw-r--r--   0 jypark     (501) staff       (20)     1115 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/SOURCES.txt
--rw-r--r--   0 jypark     (501) staff       (20)        1 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/dependency_links.txt
--rw-r--r--   0 jypark     (501) staff       (20)      184 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/requires.txt
--rw-r--r--   0 jypark     (501) staff       (20)       20 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/top_level.txt
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.704493 weavel-0.4.2/
+-rw-r--r--   0 jypark     (501) staff       (20)        0 2024-01-15 02:29:57.000000 weavel-0.4.2/LICENSE
+-rw-r--r--   0 jypark     (501) staff       (20)      406 2024-05-10 09:48:49.704382 weavel-0.4.2/PKG-INFO
+-rw-r--r--   0 jypark     (501) staff       (20)       15 2024-02-08 04:16:27.000000 weavel-0.4.2/README.md
+-rw-r--r--   0 jypark     (501) staff       (20)       38 2024-05-10 09:48:49.704535 weavel-0.4.2/setup.cfg
+-rw-r--r--   0 jypark     (501) staff       (20)     1244 2024-05-10 09:47:45.000000 weavel-0.4.2/setup.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.696619 weavel-0.4.2/testapp/
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.697635 weavel-0.4.2/testapp/daily_dialog/
+-rw-r--r--   0 jypark     (501) staff       (20)     9480 2024-02-06 10:50:36.000000 weavel-0.4.2/testapp/daily_dialog/run_qa_extractor.py
+-rw-r--r--   0 jypark     (501) staff       (20)     8672 2024-02-06 10:50:37.000000 weavel-0.4.2/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py
+-rw-r--r--   0 jypark     (501) staff       (20)     4110 2024-02-06 12:05:08.000000 weavel-0.4.2/testapp/daily_dialog/save_to_db.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1478 2024-04-23 07:57:50.000000 weavel-0.4.2/testapp/demo.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.698774 weavel-0.4.2/testapp/py_files/
+-rw-r--r--   0 jypark     (501) staff       (20)     1065 2024-01-24 05:01:55.000000 weavel-0.4.2/testapp/py_files/duplicate_log_test.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1892 2024-01-30 03:05:12.000000 weavel-0.4.2/testapp/py_files/poe_test.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1068 2024-01-24 07:27:52.000000 weavel-0.4.2/testapp/py_files/save_mock_data.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1160 2024-01-24 11:29:54.000000 weavel-0.4.2/testapp/py_files/save_mock_retention_data.py
+-rw-r--r--   0 jypark     (501) staff       (20)    43795 2024-03-22 07:15:41.000000 weavel-0.4.2/testapp/test.py
+-rw-r--r--   0 jypark     (501) staff       (20)      278 2024-04-05 04:45:14.000000 weavel-0.4.2/testapp/test_identify.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.695048 weavel-0.4.2/venv/
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.701248 weavel-0.4.2/venv/bin/
+-rwxr-xr-x   0 jypark     (501) staff       (20)     8236 2024-02-02 10:25:14.000000 weavel-0.4.2/venv/bin/pwiz.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      648 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      770 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)     1105 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      847 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      670 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      836 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      642 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      655 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      691 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      927 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      656 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      724 2024-01-15 02:43:20.000000 weavel-0.4.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.702576 weavel-0.4.2/weavel/
+-rw-r--r--   0 jypark     (501) staff       (20)      107 2024-05-10 09:47:51.000000 weavel-0.4.2/weavel/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     6063 2024-02-08 04:18:02.000000 weavel-0.4.2/weavel/_api_client.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1692 2024-04-05 02:11:37.000000 weavel-0.4.2/weavel/_buffer_storage.py
+-rw-r--r--   0 jypark     (501) staff       (20)      211 2024-03-22 06:53:42.000000 weavel-0.4.2/weavel/_constants.py
+-rw-r--r--   0 jypark     (501) staff       (20)    10904 2024-05-10 09:39:20.000000 weavel-0.4.2/weavel/_worker.py
+-rw-r--r--   0 jypark     (501) staff       (20)     5824 2024-04-05 02:54:30.000000 weavel-0.4.2/weavel/client.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.703874 weavel-0.4.2/weavel/poe/
+-rw-r--r--   0 jypark     (501) staff       (20)       58 2024-01-30 04:23:45.000000 weavel-0.4.2/weavel/poe/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1749 2024-03-22 06:53:42.000000 weavel-0.4.2/weavel/poe/_poe_buffer_storage.py
+-rw-r--r--   0 jypark     (501) staff       (20)     4768 2024-05-10 09:30:15.000000 weavel-0.4.2/weavel/poe/_poe_worker.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1300 2024-05-10 09:38:47.000000 weavel-0.4.2/weavel/poe/poe_client.py
+-rw-r--r--   0 jypark     (501) staff       (20)     2701 2024-04-05 02:24:52.000000 weavel-0.4.2/weavel/types.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.704216 weavel-0.4.2/weavel/utils/
+-rw-r--r--   0 jypark     (501) staff       (20)       43 2024-01-15 06:20:46.000000 weavel-0.4.2/weavel/utils/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1134 2024-01-15 05:54:15.000000 weavel-0.4.2/weavel/utils/crypto.py
+-rw-r--r--   0 jypark     (501) staff       (20)      679 2024-01-15 11:33:18.000000 weavel-0.4.2/weavel/utils/logger.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-10 09:48:49.703192 weavel-0.4.2/weavel.egg-info/
+-rw-r--r--   0 jypark     (501) staff       (20)      406 2024-05-10 09:48:49.000000 weavel-0.4.2/weavel.egg-info/PKG-INFO
+-rw-r--r--   0 jypark     (501) staff       (20)     1115 2024-05-10 09:48:49.000000 weavel-0.4.2/weavel.egg-info/SOURCES.txt
+-rw-r--r--   0 jypark     (501) staff       (20)        1 2024-05-10 09:48:49.000000 weavel-0.4.2/weavel.egg-info/dependency_links.txt
+-rw-r--r--   0 jypark     (501) staff       (20)      184 2024-05-10 09:48:49.000000 weavel-0.4.2/weavel.egg-info/requires.txt
+-rw-r--r--   0 jypark     (501) staff       (20)       20 2024-05-10 09:48:49.000000 weavel-0.4.2/weavel.egg-info/top_level.txt
```

### Comparing `weavel-0.4.1/setup.py` & `weavel-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read README.md for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="weavel",
-    version="0.4.1",
+    version="0.4.2",
     packages=find_namespace_packages(),
     entry_points={},
     description="Weavel, natural language analysis Dashboard for LLM Agent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="weavel",
     url="https://github.com/weavel-ai/weavel-python",
```

### Comparing `weavel-0.4.1/testapp/daily_dialog/run_qa_extractor.py` & `weavel-0.4.2/testapp/daily_dialog/run_qa_extractor.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py` & `weavel-0.4.2/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/testapp/daily_dialog/save_to_db.py` & `weavel-0.4.2/testapp/daily_dialog/save_to_db.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/testapp/demo.py` & `weavel-0.4.2/testapp/demo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from weavel import create_client, WeavelClient, Trace
 from uuid import uuid4
 
 client: WeavelClient = create_client()
 
 user_identifier = "USER IDENTIFIER EXAMPLE"
 
-client.track(user_identifier, "paid", {"amount": "100"})
-trace: Trace = client.open_trace(user_identifier, trace_id=str(uuid4())) # -> trace_id
+# client.track(user_identifier, "paid", {"amount": "100"})
+# trace: Trace = client.open_trace(user_identifier, trace_id='3714d452-ad29-4811-9ee0-8aec1771eaf8') # -> trace_id
 
-res = "I can assist you with a variety of tasks. I can help answer questions, provide information, give suggestions, assist with research, set reminders, manage your schedule, make reservations, provide translations, and much more. Just let me know what you need help with!"
+# trace_id='3714d452-ad29-4811-9ee0-8aec1771eaf8'
+trace: Trace = client.resume_trace(user_identifier, trace_id='3714d452-ad29-4811-9ee0-8aec1771eaf8')
+# res = "I can assist you with a variety of tasks. I can help answer questions, provide information, give suggestions, assist with research, set reminders, manage your schedule, make reservations, provide translations, and much more. Just let me know what you need help with!"
 
-# print(res.choices[0].message.content)
+# # print(res.choices[0].message.content)
 
-trace.log_message("assistant", res)
+# trace.log_message("assistant", res)
 
-user_message = "How to buy a math textbook?"
+user_message = "I love your service!"
 trace.log_message("user", user_message)
 
 # res = openai_client.chat.completions.create(
 #     model="gpt-3.5-turbo",
 #     messages=[
 #         {"role": "system", "content": "You are a helpful assistant"},
 #         {"role": "user", "content": user_message}
```

### Comparing `weavel-0.4.1/testapp/py_files/duplicate_log_test.py` & `weavel-0.4.2/testapp/py_files/duplicate_log_test.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/testapp/py_files/poe_test.py` & `weavel-0.4.2/testapp/py_files/poe_test.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/testapp/py_files/save_mock_data.py` & `weavel-0.4.2/testapp/py_files/save_mock_data.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/testapp/py_files/save_mock_retention_data.py` & `weavel-0.4.2/testapp/py_files/save_mock_retention_data.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/testapp/test.py` & `weavel-0.4.2/testapp/test.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/pwiz.py` & `weavel-0.4.2/venv/bin/pwiz.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2html.py` & `weavel-0.4.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2html4.py` & `weavel-0.4.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2html5.py` & `weavel-0.4.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2latex.py` & `weavel-0.4.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2man.py` & `weavel-0.4.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2odt.py` & `weavel-0.4.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2odt_prepstyles.py` & `weavel-0.4.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2pseudoxml.py` & `weavel-0.4.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2s5.py` & `weavel-0.4.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2xetex.py` & `weavel-0.4.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rst2xml.py` & `weavel-0.4.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/venv/bin/rstpep2html.py` & `weavel-0.4.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel/_api_client.py` & `weavel-0.4.2/weavel/_api_client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel/_buffer_storage.py` & `weavel-0.4.2/weavel/_buffer_storage.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel/_worker.py` & `weavel-0.4.2/weavel/_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import time
-from datetime import datetime
+from datetime import UTC, datetime, timezone
 from typing import Dict, List, Optional, Union
 from threading import Thread
 from concurrent.futures import Future, ThreadPoolExecutor
 
 from weavel.types import (
     TraceDataRole,
     OpenTraceBody,
@@ -57,19 +57,24 @@
         metadata: Optional[Dict[str, str]] = None,
     ) -> str:
         """Start the new trace for user_id.
 
         Returns:
             The trace id.
         """
+        if timestamp is None:
+            timestamp = datetime.now(timezone.utc)
+        elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
+            timestamp = timestamp.astimezone(timezone.utc)
+
         # add task to buffer
         request = OpenTraceBody(
             user_id=user_id,
             trace_id=trace_id,
-            timestamp=str(timestamp or datetime.now().isoformat()),
+            timestamp=timestamp.isoformat(),
             metadata=metadata,
         )
 
         self.buffer_storage.push(request)
 
         return trace_id
     
@@ -83,15 +88,15 @@
 
         Returns:
             None
         """
         request = SaveUserIdentityBody(
             user_id=user_id,
             properties=properties,
-            timestamp=str(datetime.now().isoformat()),
+            timestamp=str(datetime.now(timezone.utc).isoformat()),
         )
         self.buffer_storage.push(request)
 
         return
 
     def log_track_event(self, user_id: str, name: str, properties: Dict) -> None:
         """
@@ -105,15 +110,15 @@
         Returns:
             None
         """
         request = CaptureTrackEventBody(
             user_id=user_id,
             track_event_name=name,
             properties=properties,
-            timestamp=str(datetime.now().isoformat()),
+            timestamp=str(datetime.now(timezone.utc).isoformat()),
         )
         self.buffer_storage.push(request)
 
         return
 
     def log_user_message(
         self,
@@ -129,22 +134,27 @@
         Args:
             trace_id: The trace identifier.
             content: The data content.
             unit_name: The unit name.
             timestamp: The timestamp.
             metadata: The metadata.
         """
+        if timestamp is None:
+            timestamp = datetime.now(timezone.utc)
+        elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
+            timestamp = timestamp.astimezone(timezone.utc)
+            
         request = CaptureTraceDataBody(
             user_id=user_id,
             trace_id=trace_id,
             role=TraceDataRole.user,
             content=content,
             unit_name=unit_name,
             metadata=metadata,
-            timestamp=str(timestamp or datetime.now().isoformat()),
+            timestamp=timestamp.isoformat(),
         )
         self.buffer_storage.push(request)
         return
 
     def log_assistant_message(
         self,
         user_id: str,
@@ -159,22 +169,27 @@
         Args:
             trace_id: The trace identifier.
             content: The data content.
             unit_name: The unit name.
             timestamp: The timestamp.
             metadata: The metadata.
         """
+        if timestamp is None:
+            timestamp = datetime.now(timezone.utc)
+        elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
+            timestamp = timestamp.astimezone(timezone.utc)
+            
         request = CaptureTraceDataBody(
             user_id=user_id,
             trace_id=trace_id,
             role=TraceDataRole.assisatant,
             content=content,
             unit_name=unit_name,
             metadata=metadata,
-            timestamp=str(timestamp or datetime.now().isoformat()),
+            timestamp=timestamp.isoformat(),
         )
         self.buffer_storage.push(request)
         return
 
     def log_inner_step(
         self,
         user_id: str,
@@ -189,22 +204,27 @@
         Args:
             trace_id: The trace identifier.
             content: The data content.
             unit_name: The unit name.
             timestamp: The timestamp.
             metadata: The metadata.
         """
+        if timestamp is None:
+            timestamp = datetime.now(timezone.utc)
+        elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
+            timestamp = timestamp.astimezone(timezone.utc)
+            
         request = CaptureTraceDataBody(
             user_id=user_id,
             trace_id=trace_id,
             role=TraceDataRole.inner_step,
             content=content,
             unit_name=unit_name,
             metadata=metadata,
-            timestamp=str(timestamp or datetime.now().isoformat()),
+            timestamp=timestamp.isoformat(),
         )
         self.buffer_storage.push(request)
         return
 
     def send_requests(
         self,
         requests: List[
```

### Comparing `weavel-0.4.1/weavel/client.py` & `weavel-0.4.2/weavel/client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel/poe/_poe_buffer_storage.py` & `weavel-0.4.2/weavel/poe/_poe_buffer_storage.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel/poe/_poe_worker.py` & `weavel-0.4.2/weavel/poe/_poe_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self._thread = Thread(target=self.consume_buffer, daemon=True)
         self._thread.start()
     
     def log(
         self,
         user_request: QueryRequest,
         bot_responses: List[PartialResponse],
-        response_timestamp: Optional[datetime] = datetime.now().isoformat(),
+        response_timestamp: Optional[datetime] = datetime.now(timezone.utc).isoformat(),
     ):
         pass
         user_log = PoeRequest(
             body=PoeSaveTraceDataBody(
                 conversation_id=user_request.conversation_id,
                 user_id=user_request.user_id,
                 message_id=user_request.message_id,
```

### Comparing `weavel-0.4.1/weavel/poe/poe_client.py` & `weavel-0.4.2/weavel/poe/poe_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import uuid
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import Dict, List, Optional, Union
 
 import pendulum
 from dotenv import load_dotenv
 from fastapi_poe import QueryRequest, PartialResponse
 
 from weavel.types import TraceDataRole
@@ -23,15 +23,15 @@
         assert self.api_key is not None, "API key not provided."
         self.worker = PoeWorker(self.api_key)
         
     def log(
         self,
         user_request: QueryRequest,
         bot_responses: List[PartialResponse],
-        response_timestamp: Optional[datetime] = datetime.now().isoformat(),
+        response_timestamp: Optional[datetime] = datetime.now(timezone.utc).isoformat(),
     ):
         self.worker.log(user_request, bot_responses, response_timestamp)
         return
     
     def close(
         self
     ):
```

### Comparing `weavel-0.4.1/weavel/types.py` & `weavel-0.4.2/weavel/types.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel/utils/crypto.py` & `weavel-0.4.2/weavel/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel/utils/logger.py` & `weavel-0.4.2/weavel/utils/logger.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.1/weavel.egg-info/SOURCES.txt` & `weavel-0.4.2/weavel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

