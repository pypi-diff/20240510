# Comparing `tmp/qa_metrics-0.2.8.tar.gz` & `tmp/qa_metrics-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_metrics-0.2.8.tar", last modified: Tue Apr  2 13:33:21 2024, max compression
+gzip compressed data, was "qa_metrics-0.2.9.tar", last modified: Tue Apr 23 20:50:01 2024, max compression
```

## Comparing `qa_metrics-0.2.8.tar` & `qa_metrics-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 13:33:21.784973 qa_metrics-0.2.8/
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1071 2024-04-02 05:44:57.000000 qa_metrics-0.2.8/LICENSE
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       69 2024-04-02 05:44:57.000000 qa_metrics-0.2.8/MANIFEST.in
--rw-r--r--   0 zli12321 (14416) activetopic (18517)     8634 2024-04-02 13:33:21.784973 qa_metrics-0.2.8/PKG-INFO
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     7809 2024-04-02 13:32:12.000000 qa_metrics-0.2.8/README.md
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 13:33:21.782973 qa_metrics-0.2.8/qa_metrics/
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2324 2024-04-02 05:44:57.000000 qa_metrics-0.2.8/qa_metrics/__init__.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1122 2024-04-02 05:44:57.000000 qa_metrics-0.2.8/qa_metrics/em.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2853 2024-04-02 05:44:57.000000 qa_metrics-0.2.8/qa_metrics/f1.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)    15909 2024-04-02 05:44:58.000000 qa_metrics-0.2.8/qa_metrics/pedant.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     6541 2024-04-02 05:53:35.000000 qa_metrics-0.2.8/qa_metrics/prompt_llm.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1201 2024-04-02 05:44:58.000000 qa_metrics-0.2.8/qa_metrics/prompt_open_llm.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)    14173 2024-04-02 05:44:58.000000 qa_metrics-0.2.8/qa_metrics/transformerMatcher.py
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 13:33:21.783974 qa_metrics-0.2.8/qa_metrics/utils/
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:44:57.000000 qa_metrics-0.2.8/qa_metrics/utils/__init__.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2724 2024-04-02 05:44:58.000000 qa_metrics-0.2.8/qa_metrics/utils/tools.py
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 13:33:21.783974 qa_metrics-0.2.8/qa_metrics.egg-info/
--rw-r--r--   0 zli12321 (14416) activetopic (18517)     8634 2024-04-02 13:33:19.000000 qa_metrics-0.2.8/qa_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)      428 2024-04-02 13:33:20.000000 qa_metrics-0.2.8/qa_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)        1 2024-04-02 13:33:19.000000 qa_metrics-0.2.8/qa_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       75 2024-04-02 13:33:19.000000 qa_metrics-0.2.8/qa_metrics.egg-info/requires.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       11 2024-04-02 13:33:19.000000 qa_metrics-0.2.8/qa_metrics.egg-info/top_level.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       38 2024-04-02 13:33:21.784973 qa_metrics-0.2.8/setup.cfg
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1296 2024-04-02 13:32:20.000000 qa_metrics-0.2.8/setup.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-23 20:50:01.107652 qa_metrics-0.2.9/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1071 2024-04-02 05:44:57.000000 qa_metrics-0.2.9/LICENSE
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       69 2024-04-02 05:44:57.000000 qa_metrics-0.2.9/MANIFEST.in
+-rw-r--r--   0 zli12321 (14416) activetopic (18517)     8634 2024-04-23 20:50:01.107652 qa_metrics-0.2.9/PKG-INFO
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     7809 2024-04-02 13:38:07.000000 qa_metrics-0.2.9/README.md
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-23 20:50:01.106652 qa_metrics-0.2.9/qa_metrics/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2324 2024-04-02 05:44:57.000000 qa_metrics-0.2.9/qa_metrics/__init__.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1122 2024-04-02 05:44:57.000000 qa_metrics-0.2.9/qa_metrics/em.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2853 2024-04-02 05:44:57.000000 qa_metrics-0.2.9/qa_metrics/f1.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)    15261 2024-04-23 20:48:35.000000 qa_metrics-0.2.9/qa_metrics/pedant.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     6541 2024-04-02 05:53:35.000000 qa_metrics-0.2.9/qa_metrics/prompt_llm.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1201 2024-04-02 05:44:58.000000 qa_metrics-0.2.9/qa_metrics/prompt_open_llm.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)    14173 2024-04-02 05:44:58.000000 qa_metrics-0.2.9/qa_metrics/transformerMatcher.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-23 20:50:01.107652 qa_metrics-0.2.9/qa_metrics/utils/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:44:57.000000 qa_metrics-0.2.9/qa_metrics/utils/__init__.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     3977 2024-04-23 20:38:42.000000 qa_metrics-0.2.9/qa_metrics/utils/tools.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-23 20:50:01.107652 qa_metrics-0.2.9/qa_metrics.egg-info/
+-rw-r--r--   0 zli12321 (14416) activetopic (18517)     8634 2024-04-23 20:50:00.000000 qa_metrics-0.2.9/qa_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)      428 2024-04-23 20:50:00.000000 qa_metrics-0.2.9/qa_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)        1 2024-04-23 20:50:00.000000 qa_metrics-0.2.9/qa_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       75 2024-04-23 20:50:00.000000 qa_metrics-0.2.9/qa_metrics.egg-info/requires.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       11 2024-04-23 20:50:00.000000 qa_metrics-0.2.9/qa_metrics.egg-info/top_level.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       38 2024-04-23 20:50:01.107652 qa_metrics-0.2.9/setup.cfg
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1296 2024-04-23 20:49:38.000000 qa_metrics-0.2.9/setup.py
```

### Comparing `qa_metrics-0.2.8/LICENSE` & `qa_metrics-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.8/PKG-INFO` & `qa_metrics-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa_metrics
-Version: 0.2.8
+Version: 0.2.9
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -81,16 +81,16 @@
 '''
 ```
 
 ###### deepinfra (See below for descriptions of more models)
 ```python
 from qa_metrics.prompt_open_llm import OpenLLM
 model = OpenLLM()
-model.set_deepinfra_api_key(YOUR_OPENAI_KEY)
-model.prompt(prompt=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
+model.set_deepinfra_key(YOUR_DEEPINFRA_KEY)
+model.prompt(message=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
 
 '''
 'correct'
 '''
 ```
 
 #### Exact Match
```

### Comparing `qa_metrics-0.2.8/README.md` & `qa_metrics-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 '''
 ```
 
 ###### deepinfra (See below for descriptions of more models)
 ```python
 from qa_metrics.prompt_open_llm import OpenLLM
 model = OpenLLM()
-model.set_deepinfra_api_key(YOUR_OPENAI_KEY)
-model.prompt(prompt=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
+model.set_deepinfra_key(YOUR_DEEPINFRA_KEY)
+model.prompt(message=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
 
 '''
 'correct'
 '''
 ```
 
 #### Exact Match
```

### Comparing `qa_metrics-0.2.8/qa_metrics/__init__.py` & `qa_metrics-0.2.9/qa_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.8/qa_metrics/em.py` & `qa_metrics-0.2.9/qa_metrics/em.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.8/qa_metrics/f1.py` & `qa_metrics-0.2.9/qa_metrics/f1.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.8/qa_metrics/pedant.py` & `qa_metrics-0.2.9/qa_metrics/pedant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .f1 import f1_score_with_precision_recall
-from .utils.tools import normalize_answer, download_link, remove_punctuation
+from .utils.tools import *
 import joblib
 from scipy.sparse import hstack
 import numpy as np
 import os
+import contractions
 import requests
 
 
 class PEDANT:
     def __init__(self): 
         current_dir = os.path.dirname(__file__) 
         model_dir = os.path.join(current_dir, 'classifier') 
@@ -49,26 +50,23 @@
         self.tokenizer = joblib.load(vectorizer_path)
 
     '''
     Return the confidence score between the reference and candidate answers. 
     reference, candidate, and question are strings.
     '''
     def get_score(self, reference, candidate, question):
-        reference = remove_punctuation(normalize_answer(str(reference)))
-        candidate = remove_punctuation(normalize_answer(str(candidate)))
-        question = remove_punctuation(normalize_answer(str(question)))
-
-        if reference in candidate:
+        if remove_punctuation(normalize_answer(str(reference))) in remove_punctuation(normalize_answer(str(candidate))):
             return 1.0
 
         input_texts = []
         f1_scores, precisions, recalls = [], [], []
-        input_texts.append("[CLS] " + candidate + " [SEP] " + reference + " [SEP] " + question + " [SEP]")
-        f1_results = f1_score_with_precision_recall(reference, candidate)
-        f, p, r = f1_results['f1'], f1_results['precision'], f1_results['recall']
+        curr_input_text = "[CLS] " + contractions.fix(normalize_answer(str(candidate))) + " [SEP] " + contractions.fix(normalize_answer(str(reference))) + " [SEP] " + contractions.fix(normalize_answer(str(question))) + " [SEP]"
+        input_texts.append(curr_input_text)
+        f, p, r = calculate_f1_score_with_precision(str(candidate), str(reference))
+       
         f1_scores.append(f)
         precisions.append(p)
         recalls.append(r)
 
         f1_scores = np.array(f1_scores).reshape(-1, 1)
         precisions = np.array(precisions).reshape(-1, 1)
         recalls = np.array(recalls).reshape(-1, 1)
@@ -156,43 +154,38 @@
             
             for i in range(len(pred_probas)):
                 confidece_scores[references[i]] = {}
                 confidece_scores[references[i]][candidate] = pred_probas[i][0]
                             
             return confidece_scores
         elif isinstance(candidate, list):
-            candidates = [remove_punctuation(normalize_answer(str(ele))) for ele in candidate]
-            reference = remove_punctuation(normalize_answer(str(reference)))
-            question = remove_punctuation(normalize_answer(str(question)))
-
-            input_texts = []
-            f1_scores, precisions, recalls = [], [], []
-            for candidate in candidates:
-                input_texts.append("[CLS] " + candidate + " [SEP] " + reference + " [SEP] " + question + " [SEP]")
-                f1_results = f1_score_with_precision_recall(reference, candidate)
-                f, p, r = f1_results['f1'], f1_results['precision'], f1_results['recall']
+            references = reference
+            for reference in references:
+                curr_input_text = "[CLS] " + contractions.fix(normalize_answer(str(candidate))) + " [SEP] " + contractions.fix(normalize_answer(str(reference))) + " [SEP] " + contractions.fix(normalize_answer(str(question))) + " [SEP]"
+                input_texts.append(curr_input_text)
+                f, p, r = calculate_f1_score_with_precision(str(candidate), str(reference))
                 f1_scores.append(f)
                 precisions.append(p)
                 recalls.append(r)
 
+                        
             f1_scores = np.array(f1_scores).reshape(-1, 1)
             precisions = np.array(precisions).reshape(-1, 1)
             recalls = np.array(recalls).reshape(-1, 1)
-
+                
+           
             texts = self.tokenizer.transform(input_texts)
-
-            '''
-            Concatenate text features with f1 features
-            '''
+            # result = hstack([texts, f1_scores, precisions, recalls, edit_distances])            
+        
             features = hstack([texts, f1_scores, precisions, recalls])
             pred_probas = self.model.predict_proba(features)
             
             confidece_scores[reference] = {}
             for i in range(len(pred_probas)):
-                confidece_scores[reference][candidates[i]] = pred_probas[i][0]
+                confidece_scores[reference][candidate[i]] = pred_probas[i][0]
                             
             return confidece_scores
         else:
             confidece_scores[reference] = {}
             confidece_scores[reference][candidate] = self.get_score(reference, candidate, question)
 
             return confidece_scores
@@ -253,46 +246,34 @@
                     preds = self.model.predict(features)
 
                     if "correct" in preds:
                         judgment = True
                             
             return judgment
         elif isinstance(reference, list):
-            references = [remove_punctuation(normalize_answer(str(ele))) for ele in reference]
-            candidate = remove_punctuation(normalize_answer(str(candidate)))
-            question = remove_punctuation(normalize_answer(str(question)))
-
-            input_texts = []
-            f1_scores, precisions, recalls = [], [], []
+            references = reference
             for reference in references:
-                if reference in candidate:
-                    return True
-                input_texts.append("[CLS] " + candidate + " [SEP] " + reference + " [SEP] " + question + " [SEP]")
-                f1_results = f1_score_with_precision_recall(reference, candidate)
-                f, p, r = f1_results['f1'], f1_results['precision'], f1_results['recall']
+                curr_input_text = "[CLS] " + contractions.fix(normalize_answer(str(candidate))) + " [SEP] " + contractions.fix(normalize_answer(str(reference))) + " [SEP] " + contractions.fix(normalize_answer(str(question))) + " [SEP]"
+                input_texts.append(curr_input_text)
+                f, p, r = calculate_f1_score_with_precision(str(candidate), str(reference))
                 f1_scores.append(f)
                 precisions.append(p)
                 recalls.append(r)
 
             f1_scores = np.array(f1_scores).reshape(-1, 1)
             precisions = np.array(precisions).reshape(-1, 1)
             recalls = np.array(recalls).reshape(-1, 1)
 
             texts = self.tokenizer.transform(input_texts)
 
-            '''
-            Concatenate text features with f1 features
-            '''
-            features = hstack([texts, f1_scores, precisions, recalls])
-            preds = self.model.predict(features)
+            result = hstack([texts, f1_scores, precisions, recalls])
+            output = self.model.predict(result)
 
-            if "correct" in preds:
-                judgment = True
-                            
-            return judgment
+
+            return "correct" in output
         elif isinstance(candidate, list):
             candidates = [remove_punctuation(normalize_answer(str(ele))) for ele in candidate]
             reference = remove_punctuation(normalize_answer(str(reference)))
             question = remove_punctuation(normalize_answer(str(question)))
 
             input_texts = []
             f1_scores, precisions, recalls = [], [], []
```

### Comparing `qa_metrics-0.2.8/qa_metrics/prompt_llm.py` & `qa_metrics-0.2.9/qa_metrics/prompt_llm.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.8/qa_metrics/prompt_open_llm.py` & `qa_metrics-0.2.9/qa_metrics/prompt_open_llm.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.8/qa_metrics/transformerMatcher.py` & `qa_metrics-0.2.9/qa_metrics/transformerMatcher.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.8/qa_metrics/utils/tools.py` & `qa_metrics-0.2.9/qa_metrics/utils/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,69 @@
 import string
 import contractions
 import requests
 import os
 import regex
 from datetime import datetime
 
+def fix_answer(s):
+        def remove_articles(text):
+            return regex.sub(r'\b(a|an|the)\b', ' ', text)
+
+        def white_space_fix(text):
+            return ' '.join(text.split())
+
+        def remove_punc(text):
+            exclude = set(string.punctuation)
+            return ''.join(ch for ch in text if ch not in exclude)
+
+        def lower(text):
+            return text.lower()
+
+        return white_space_fix(remove_articles(remove_punc(lower(s))))
+
 def normalize_answer(text, lower=True):
     if isinstance(text, list):
         result = []
         for ele in text:
             ele = str(ele)
             if lower:
                 ele = ele.lower()
             translator = str.maketrans('', '', string.punctuation)
             ele = ele.translate(translator)
-            result.append(contractions.fix(' '.join(ele.split())))
+            result.append(fix_answer(' '.join(ele.split())))
         return result
     else:
         text = str(text)
         if lower:
             text = text.lower()
         translator = str.maketrans('', '', string.punctuation)
         text = text.translate(translator)
-        return contractions.fix(' '.join(text.split()))
+        return fix_answer(' '.join(text.split()))
+
+def calculate_f1_score_with_precision(str1, str2):
+    # Split the strings into sets of words
+    str1 = fix_answer(contractions.fix(normalize_answer(str1)))
+    str2 = fix_answer(contractions.fix(normalize_answer(str2)))
+    words_str1 = set(str1.split())
+    words_str2 = set(str2.split())
+
+    # Calculate true positives, false positives, and false negatives
+    tp = len(words_str1.intersection(words_str2))
+    fp = len(words_str1 - words_str2)
+    fn = len(words_str2 - words_str1)
+
+    # Calculate precision and recall
+    precision = tp / (tp + fp) if (tp + fp) > 0 else 0
+    recall = tp / (tp + fn) if (tp + fn) > 0 else 0
+
+    # Calculate F1 score
+    f1_score = 2 * (precision * recall) / (precision + recall) if (precision + recall) > 0 else 0
+
+    return f1_score, precision, recall
 
 def remove_punctuation(text):
     def remove_articles(text):
         return regex.sub(r'\b(a|an|the)\b', ' ', text)
 
     def white_space_fix(text):
         return ' '.join(text.split())
```

### Comparing `qa_metrics-0.2.8/qa_metrics.egg-info/PKG-INFO` & `qa_metrics-0.2.9/qa_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa-metrics
-Version: 0.2.8
+Version: 0.2.9
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -81,16 +81,16 @@
 '''
 ```
 
 ###### deepinfra (See below for descriptions of more models)
 ```python
 from qa_metrics.prompt_open_llm import OpenLLM
 model = OpenLLM()
-model.set_deepinfra_api_key(YOUR_OPENAI_KEY)
-model.prompt(prompt=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
+model.set_deepinfra_key(YOUR_DEEPINFRA_KEY)
+model.prompt(message=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
 
 '''
 'correct'
 '''
 ```
 
 #### Exact Match
```

### Comparing `qa_metrics-0.2.8/setup.py` & `qa_metrics-0.2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 
 
 setup(
     name='qa_metrics',
-    version='0.2.8',
+    version='0.2.9',
     author='Zongxia Li',
     author_email='zli12321@umd.edu',
     description='This package provides standard and classifier-based short form QA evaluation methods',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/zli12321/qa_metrics',
     packages=find_packages(),
```

