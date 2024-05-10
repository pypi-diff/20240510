# Comparing `tmp/modelmerge-0.2.8.tar.gz` & `tmp/modelmerge-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.2.8.tar", last modified: Fri May 10 02:15:50 2024, max compression
+gzip compressed data, was "modelmerge-0.2.9.tar", last modified: Fri May 10 02:36:57 2024, max compression
```

## Comparing `modelmerge-0.2.8.tar` & `modelmerge-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.442083 modelmerge-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 02:15:41.000000 modelmerge-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-10 02:15:50.442083 modelmerge-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 02:15:41.000000 modelmerge-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:15:50.442083 modelmerge-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-10 02:15:41.000000 modelmerge-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.434083 modelmerge-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.438083 modelmerge-0.2.8/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.438083 modelmerge-0.2.8/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29963 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.438083 modelmerge-0.2.8/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/plugins/travel.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.438083 modelmerge-0.2.8/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.438083 modelmerge-0.2.8/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-10 02:15:41.000000 modelmerge-0.2.8/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.442083 modelmerge-0.2.8/src/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-10 02:15:50.000000 modelmerge-0.2.8/src/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-10 02:15:50.000000 modelmerge-0.2.8/src/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:15:50.000000 modelmerge-0.2.8/src/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 02:15:50.000000 modelmerge-0.2.8/src/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 02:15:50.000000 modelmerge-0.2.8/src/ModelMerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:15:50.442083 modelmerge-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 02:15:41.000000 modelmerge-0.2.8/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 02:15:41.000000 modelmerge-0.2.8/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 02:15:41.000000 modelmerge-0.2.8/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.829887 modelmerge-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 02:36:48.000000 modelmerge-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-10 02:36:57.829887 modelmerge-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-10 02:36:48.000000 modelmerge-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:36:57.829887 modelmerge-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-10 02:36:48.000000 modelmerge-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.825887 modelmerge-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.825887 modelmerge-0.2.9/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.829887 modelmerge-0.2.9/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.829887 modelmerge-0.2.9/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/plugins/travel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.829887 modelmerge-0.2.9/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.829887 modelmerge-0.2.9/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-10 02:36:48.000000 modelmerge-0.2.9/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.829887 modelmerge-0.2.9/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-10 02:36:57.000000 modelmerge-0.2.9/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-10 02:36:57.000000 modelmerge-0.2.9/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:36:57.000000 modelmerge-0.2.9/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 02:36:57.000000 modelmerge-0.2.9/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 02:36:57.000000 modelmerge-0.2.9/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:36:57.829887 modelmerge-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 02:36:48.000000 modelmerge-0.2.9/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 02:36:48.000000 modelmerge-0.2.9/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 02:36:48.000000 modelmerge-0.2.9/test/test_google_search.py
```

### Comparing `modelmerge-0.2.8/LICENSE` & `modelmerge-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.9/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,16 @@
             except Exception as e:
                 print(f"发生了未预料的错误: {e}")
                 return
             if response.status_code == 400:
                 del json_post["function_call"]
                 del json_post["functions"]
                 continue
+            if response.status_code == 200:
+                break
         if response.status_code != 200:
             raise Exception(f"{response.status_code} {response.reason} {response.text}")
         response_role: str = None
         full_response: str = ""
         function_full_response: str = ""
         function_call_name: str = ""
         need_function_call: bool = False
```

### Comparing `modelmerge-0.2.8/src/ModelMerge/models/claude.py` & `modelmerge-0.2.9/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/models/config.py` & `modelmerge-0.2.9/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/models/genimi.py` & `modelmerge-0.2.9/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/models/groq.py` & `modelmerge-0.2.9/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.2.9/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/tools/function_call.py` & `modelmerge-0.2.9/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/utils/prompt.py` & `modelmerge-0.2.9/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge/utils/scripts.py` & `modelmerge-0.2.9/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/src/ModelMerge.egg-info/SOURCES.txt` & `modelmerge-0.2.9/src/ModelMerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.8/test/test_google_search.py` & `modelmerge-0.2.9/test/test_google_search.py`

 * *Files identical despite different names*

