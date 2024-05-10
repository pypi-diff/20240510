# Comparing `tmp/apollo-ai-0.0.47.tar.gz` & `tmp/apollo-ai-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-ai-0.0.47.tar", last modified: Wed May  8 03:40:18 2024, max compression
+gzip compressed data, was "apollo-ai-0.0.48.tar", last modified: Fri May 10 20:31:59 2024, max compression
```

## Comparing `apollo-ai-0.0.47.tar` & `apollo-ai-0.0.48.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.173225 apollo-ai-0.0.47/
--rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.47/LICENSE
--rw-rw-rw-   0        0        0     9511 2024-05-08 03:40:18.171709 apollo-ai-0.0.47/PKG-INFO
--rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.47/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.067527 apollo-ai-0.0.47/apollo/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.093175 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/
--rw-rw-rw-   0        0        0     9511 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      596 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.106299 apollo-ai-0.0.47/apollo/argus/
--rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/argus/__init__.py
--rw-rw-rw-   0        0        0    12485 2024-05-08 03:26:33.000000 apollo-ai-0.0.47/apollo/argus/argus.py
--rw-rw-rw-   0        0        0     6864 2024-05-08 03:20:05.000000 apollo-ai-0.0.47/apollo/argus/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.118837 apollo-ai-0.0.47/apollo/lyre/
--rw-rw-rw-   0        0        0      149 2024-05-06 03:28:49.000000 apollo-ai-0.0.47/apollo/lyre/__init__.py
--rw-rw-rw-   0        0        0     9151 2024-05-06 03:28:49.000000 apollo-ai-0.0.47/apollo/lyre/lyre.py
--rw-rw-rw-   0        0        0     3140 2024-05-06 03:28:49.000000 apollo-ai-0.0.47/apollo/lyre/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.132404 apollo-ai-0.0.47/apollo/pythia/
--rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/pythia/__init__.py
--rw-rw-rw-   0        0        0    10013 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/pythia/pythia.py
--rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/pythia/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-08 03:40:18.174246 apollo-ai-0.0.47/setup.cfg
--rw-rw-rw-   0        0        0     1821 2024-05-08 03:28:10.000000 apollo-ai-0.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.653531 apollo-ai-0.0.48/
+-rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.48/LICENSE
+-rw-rw-rw-   0        0        0     9511 2024-05-10 20:31:59.652490 apollo-ai-0.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.48/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.361863 apollo-ai-0.0.48/apollo/
+drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.424573 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/
+-rw-rw-rw-   0        0        0     9511 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-10 20:31:58.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      596 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.528148 apollo-ai-0.0.48/apollo/argus/
+-rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.48/apollo/argus/__init__.py
+-rw-rw-rw-   0        0        0    12485 2024-05-08 03:26:33.000000 apollo-ai-0.0.48/apollo/argus/argus.py
+-rw-rw-rw-   0        0        0     6864 2024-05-08 03:20:05.000000 apollo-ai-0.0.48/apollo/argus/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.598050 apollo-ai-0.0.48/apollo/lyre/
+-rw-rw-rw-   0        0        0      149 2024-05-06 03:28:49.000000 apollo-ai-0.0.48/apollo/lyre/__init__.py
+-rw-rw-rw-   0        0        0     9151 2024-05-06 03:28:49.000000 apollo-ai-0.0.48/apollo/lyre/lyre.py
+-rw-rw-rw-   0        0        0     3140 2024-05-06 03:28:49.000000 apollo-ai-0.0.48/apollo/lyre/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.648151 apollo-ai-0.0.48/apollo/pythia/
+-rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.48/apollo/pythia/__init__.py
+-rw-rw-rw-   0        0        0    10484 2024-05-10 20:30:38.000000 apollo-ai-0.0.48/apollo/pythia/pythia.py
+-rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.48/apollo/pythia/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-10 20:31:59.653531 apollo-ai-0.0.48/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2024-05-10 20:31:51.000000 apollo-ai-0.0.48/setup.py
```

### Comparing `apollo-ai-0.0.47/LICENSE` & `apollo-ai-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/PKG-INFO` & `apollo-ai-0.0.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.47
+Version: 0.0.48
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.47/README.md` & `apollo-ai-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/apollo/apollo_ai.egg-info/PKG-INFO` & `apollo-ai-0.0.48/apollo/apollo_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.47
+Version: 0.0.48
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.47/apollo/apollo_ai.egg-info/requires.txt` & `apollo-ai-0.0.48/apollo/apollo_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/apollo/argus/argus.py` & `apollo-ai-0.0.48/apollo/argus/argus.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/apollo/argus/utils.py` & `apollo-ai-0.0.48/apollo/argus/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/apollo/lyre/lyre.py` & `apollo-ai-0.0.48/apollo/lyre/lyre.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/apollo/lyre/utils.py` & `apollo-ai-0.0.48/apollo/lyre/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/apollo/pythia/pythia.py` & `apollo-ai-0.0.48/apollo/pythia/pythia.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from epitran import Epitran
 from pyphen import Pyphen
 import re
 import jiwer
 import difflib
 import logging
 import time
+import json
 from faster_whisper import WhisperModel
 import multiprocessing
 import concurrent.futures
 import os
 
 from .utils import (
     transcribe_file,
@@ -27,20 +28,24 @@
     it only leaves tildes and double points on top of words without changing the case
 
     :param text:
     :return:
     """
     try:
         cleaned_text = re.sub(r'[^A-Za-z0-9áéíóúÁÉÍÓÚñÑüÜ]+', ' ', text)
-        return cleaned_text
+
+        data = {
+            "data": cleaned_text,
+        }
+        return json.dumps(data)
     except Exception as e:
         raise Exception("Error getting clean text: {0}".format(e))
 
 
-def sentences(text: str) -> list[str]:
+def sentences(text: str) -> str:
     """
     Extracts all the sentences in a text string conserving inner punctuation and case
 
     :param text:
     :return:
     """
     try:
@@ -60,21 +65,25 @@
             sentence = sentence.strip()
             if sentence and not sentence.startswith("–") and not sentence.startswith(
                     "-"):
                 sentence = sentence.strip(":")
                 sentence = sentence.strip(", ")
                 processed_sentences.append(sentence)
 
-        return processed_sentences
+        data = {
+            "data": processed_sentences,
+        }
+
+        return json.dumps(data)
 
     except Exception as e:
         raise Exception('Error getting sentences: {0}'.format(e))
 
 
-def word_checker(original_text: str, new_text: str) -> dict:
+def word_checker(original_text: str, new_text: str) -> str:
     """
     Compares two transcriptions and returns the correct words, incorrect
     words and omitted words
 
     word error rate (WER)
     match error rate (MER)
     word information lost (WIL)
@@ -103,17 +112,18 @@
                 new_words.remove(original_word)
                 correct_words.append(original_word)
             else:
                 omitted_words.append(original_word)
 
         incorrect_words = new_words
 
-        return {"correct_words": correct_words, "omitted_words": omitted_words, "incorrect_words": incorrect_words,
+        data = {"correct_words": correct_words, "omitted_words": omitted_words, "incorrect_words": incorrect_words,
                 "mer": mer, "wil": wil, "wip": wip, "wer": wer}
 
+        return json.dumps(data)
     except Exception as e:
         raise Exception("Error comparing words: {0}".format(e))
 
 
 def word_alignment(original_text: str, new_text: str) -> dict:
     """
     Compares two transcriptions and returns word by word the difference
@@ -145,35 +155,39 @@
                 residual_words.extend(original_words[a0:a1])
 
             elif opcode == 'insert' or opcode == 'replace':
                 # Original transcription does not include this words
                 alignment.extend('*' * len(word) for word in new_words[b0:b1])
                 extra_words.extend(new_words[b0:b1])
 
-        return {"alignment": alignment, "residual_words": residual_words, "extra_words": extra_words}
+        data = {"alignment": alignment, "residual_words": residual_words, "extra_words": extra_words}
+        return json.dumps(data)
     except Exception as e:
         raise Exception("Error on word alignment: {0}".format(e))
 
 
 def phonetic_transcription(text: str, lang='spa-Latn') -> str:
     """
     Cleans text and makes the phonetic following IPA
 
     :param text:
     :param lang:
     :return:
     """
     epi = Epitran(lang)
     try:
-        return epi.transliterate(clean_text(text))
+        data = {
+            "data": epi.transliterate(clean_text(text))
+        }
+        return json.dumps(data)
     except Exception as e:
         raise Exception("Error getting the phonetic transcription: {0}".format(e))
 
 
-def syllables(text: str, lang='es') -> list[str]:
+def syllables(text: str, lang='es') -> str:
     """
     Extracts all the syllables from a text string
 
     :param text:
     :param lang:
     :return:
     """
@@ -185,21 +199,24 @@
         list_words = [token.text for token in doc]
         list_syllables = []
 
         for word in list_words:
             syllables_ = py_instance.inserted(word).split('-')
             list_syllables.extend(syllables_)
 
-        return list_syllables
+        data = {
+            "data": list_syllables
+        }
 
+        return json.dumps(data)
     except Exception as e:
         raise Exception('Error getting syllables: {0}'.format(e))
 
 
-def words(text: str, lower=False, lang='es') -> list[str]:
+def words(text: str, lower=False, lang='es') -> str:
     """
     Extracts all the words from a corpus in lower case
 
     :param text:
     :param lower:
     :param lang:
     :return:
@@ -210,21 +227,26 @@
 
         if lower:
             doc = nlp(text.lower())
         else:
             doc = nlp(text)
 
         list_words = [token.text for token in doc]
-        return list_words
+
+        data = {
+            "data": list_words
+        }
+
+        return json.dumps(data)
     except Exception as e:
         raise Exception("Error on getting words: {0}".format(e))
 
 
 def transcriber_parallel(file: str, model_name='small', device='cpu', max_processes=0, compute_type='float16',
-                lang='es', silence_threshold: str = "-20dB", silence_duration: float = 2.0) -> dict:
+                lang='es', silence_threshold: str = "-20dB", silence_duration: float = 2.0) -> str:
     """
     Generates a transcription result from the given file
     it simplifies the audio loading and comes out of the box
     with all the timestamps of each word
 
     :param file: The name of the file
     :param model_name:
@@ -262,21 +284,23 @@
                     {"start": segment.start, "end": segment.end, "text": segment.text, "words": segment.words})
 
                 transcription += segment.text + " "
 
         for temp_file in temp_files_array:
             os.remove(temp_file)
 
-        return {"transcription": transcription, "segments": segments_output, "time_taken": time.time() - start_time}
+        data = {"transcription": transcription, "segments": segments_output, "time_taken": time.time() - start_time}
+
+        return json.dumps(data)
     except Exception as e:
         raise Exception("Error transcribing: {0}".format(e))
 
 
 def transcriber(file: str, model_name='large-v2', device='cuda', compute_type='float16', beam_size=5,
-                lang='es') -> dict:
+                lang='es') -> str:
     """
     Generates a transcription result from the given file
     it simplifies the audio loading and comes out of the box
     with all the timestamps of each word
 
     :param file: The name of the file
     :param model_name:
@@ -301,10 +325,11 @@
         for segment in segments:
             segments_output.append(
                 {"start": segment.start, "end": segment.end, "text": segment.text, "words": segment.words,
                  "tokens": segment.tokens})
 
             transcription += segment.text + " "
 
-        return {"transcription": transcription, "segments": segments_output, "info": info, "time_taken": time.time() - start_time}
+        data = {"transcription": transcription, "segments": segments_output, "info": info, "time_taken": time.time() - start_time}
+        return json.dumps(data)
     except Exception as e:
         raise Exception("Error transcribing: {0}".format(e))
```

### Comparing `apollo-ai-0.0.47/apollo/pythia/utils.py` & `apollo-ai-0.0.48/apollo/pythia/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.47/setup.py` & `apollo-ai-0.0.48/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="apollo-ai",
-    version="0.0.47",
+    version="0.0.48",
     description="Framework to process 3 channels in one: Video, Audio & Text",
     package_dir={"": "apollo"},
     packages=find_packages(where="apollo"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VerbaNexAI/APOLLO.AI",
     author="VerbaNex, Riddle",
```

