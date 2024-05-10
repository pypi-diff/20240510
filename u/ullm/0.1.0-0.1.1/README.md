# Comparing `tmp/ullm-0.1.0.tar.gz` & `tmp/ullm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ullm-0.1.0.tar", last modified: Thu May  9 09:08:31 2024, max compression
+gzip compressed data, was "ullm-0.1.1.tar", last modified: Thu May  9 09:30:42 2024, max compression
```

## Comparing `ullm-0.1.0.tar` & `ullm-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:08:31.112565 ullm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    17648 2024-05-09 09:08:31.112565 ullm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-09 09:08:26.000000 ullm-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-09 09:08:26.000000 ullm-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:08:31.112565 ullm-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:08:31.104565 ullm-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-09 09:08:26.000000 ullm-0.1.0/tests/test_openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:08:31.108565 ullm-0.1.0/ullm/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (127)    23335 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/deepseek.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/iflytek.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/minimax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/moonshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/stepfun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/zero_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-09 09:08:26.000000 ullm-0.1.0/ullm/zhipu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:08:31.108565 ullm-0.1.0/ullm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17648 2024-05-09 09:08:31.000000 ullm-0.1.0/ullm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 09:08:31.000000 ullm-0.1.0/ullm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:08:31.000000 ullm-0.1.0/ullm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 09:08:31.000000 ullm-0.1.0/ullm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 09:08:31.000000 ullm-0.1.0/ullm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 09:08:31.000000 ullm-0.1.0/ullm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.487064 ullm-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-09 09:30:42.487064 ullm-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-09 09:30:37.000000 ullm-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-09 09:30:37.000000 ullm-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:30:42.487064 ullm-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.483064 ullm-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-09 09:30:37.000000 ullm-0.1.1/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.487064 ullm-0.1.1/ullm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23335 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/deepseek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/iflytek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/minimax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/moonshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/stepfun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/zero_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/zhipu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.487064 ullm-0.1.1/ullm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/top_level.txt
```

### Comparing `ullm-0.1.0/PKG-INFO` & `ullm-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: arrow
 Requires-Dist: websocket-client
 Requires-Dist: requests
 Requires-Dist: python-magic
 Requires-Dist: click
+Requires-Dist: deepmerge
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 <h1 align="center">ullm</h1>
 <p align="center">A unified interface for local Large Language Model(LLM) models and online LLM providers.</p>
 <h4 align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.1.0 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.1.1 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
-Requires-Dist: python-magic Requires-Dist: click Provides-Extra: test Requires-
-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: python-magic Requires-Dist: click Requires-Dist: deepmerge
+Provides-Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist:
+pytest-cov; extra == "test"
                               ************ uullllmm ************
  A unified interface for local Large Language Model(LLM) models and online LLM
                                   providers.
             ****** _[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]]_[[_PP_rr_ee_--_cc_oo_mm_mm_ii_tt_ _ss_tt_aa_tt_uu_ss_]]_[[_BB_uu_ii_ll_dd_ _ss_tt_aa_tt_uu_ss_]] ******
 ullm å¸æè½ä¸ºæ¬å°æ¨¡åä»¥åä¼å¤å¨çº¿ LLM
 æå¡æä¾ç»ä¸çè°ç¨æ¹å¼ï¼ä½¿å¾å¼åèè½å¤æ çå°å¨ä¸åæ¨¡åæ
 LLM æå¡ä¹é´åæ¢ï¼èæ éæ´æ¹ä»£ç ã > [!NOTE] >
```

### Comparing `ullm-0.1.0/README.md` & `ullm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/pyproject.toml` & `ullm-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "ullm"
-version = "0.1.0"
+version = "0.1.1"
 description = "A unified interface for local Large Language Model(LLM) models and online LLM providers."
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
     "pydantic",
     "arrow",
     "websocket-client",
     "requests",
     "python-magic",
     "click",
+    "deepmerge",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `ullm-0.1.0/tests/test_openai.py` & `ullm-0.1.1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/__init__.py` & `ullm-0.1.1/ullm/__init__.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/alibaba.py` & `ullm-0.1.1/ullm/alibaba.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/anthropic.py` & `ullm-0.1.1/ullm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/baichuan.py` & `ullm-0.1.1/ullm/baichuan.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/baidu.py` & `ullm-0.1.1/ullm/baidu.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/base.py` & `ullm-0.1.1/ullm/base.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/cli.py` & `ullm-0.1.1/ullm/cli.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/cohere.py` & `ullm-0.1.1/ullm/cohere.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/deepseek.py` & `ullm-0.1.1/ullm/deepseek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/google.py` & `ullm-0.1.1/ullm/google.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/groq.py` & `ullm-0.1.1/ullm/groq.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/iflytek.py` & `ullm-0.1.1/ullm/iflytek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/minimax.py` & `ullm-0.1.1/ullm/minimax.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/moonshot.py` & `ullm-0.1.1/ullm/moonshot.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/ollama.py` & `ullm-0.1.1/ullm/ollama.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/openai.py` & `ullm-0.1.1/ullm/openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/openrouter.py` & `ullm-0.1.1/ullm/openrouter.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/perplexity.py` & `ullm-0.1.1/ullm/perplexity.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/stepfun.py` & `ullm-0.1.1/ullm/stepfun.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/zero_one.py` & `ullm-0.1.1/ullm/zero_one.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm/zhipu.py` & `ullm-0.1.1/ullm/zhipu.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.0/ullm.egg-info/PKG-INFO` & `ullm-0.1.1/ullm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: arrow
 Requires-Dist: websocket-client
 Requires-Dist: requests
 Requires-Dist: python-magic
 Requires-Dist: click
+Requires-Dist: deepmerge
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 <h1 align="center">ullm</h1>
 <p align="center">A unified interface for local Large Language Model(LLM) models and online LLM providers.</p>
 <h4 align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.1.0 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.1.1 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
-Requires-Dist: python-magic Requires-Dist: click Provides-Extra: test Requires-
-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: python-magic Requires-Dist: click Requires-Dist: deepmerge
+Provides-Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist:
+pytest-cov; extra == "test"
                               ************ uullllmm ************
  A unified interface for local Large Language Model(LLM) models and online LLM
                                   providers.
             ****** _[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]]_[[_PP_rr_ee_--_cc_oo_mm_mm_ii_tt_ _ss_tt_aa_tt_uu_ss_]]_[[_BB_uu_ii_ll_dd_ _ss_tt_aa_tt_uu_ss_]] ******
 ullm å¸æè½ä¸ºæ¬å°æ¨¡åä»¥åä¼å¤å¨çº¿ LLM
 æå¡æä¾ç»ä¸çè°ç¨æ¹å¼ï¼ä½¿å¾å¼åèè½å¤æ çå°å¨ä¸åæ¨¡åæ
 LLM æå¡ä¹é´åæ¢ï¼èæ éæ´æ¹ä»£ç ã > [!NOTE] >
```

### Comparing `ullm-0.1.0/ullm.egg-info/SOURCES.txt` & `ullm-0.1.1/ullm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

