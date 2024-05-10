# Comparing `tmp/jzchatbot-59.83.90.tar.gz` & `tmp/jzchatbot-59.83.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.90.tar", last modified: Fri May 10 01:35:08 2024, max compression
+gzip compressed data, was "jzchatbot-59.83.91.tar", last modified: Fri May 10 01:39:42 2024, max compression
```

## Comparing `jzchatbot-59.83.90.tar` & `jzchatbot-59.83.91.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 01:35:08.238433 jzchatbot-59.83.90/
--rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.90/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-10 01:35:08.231270 jzchatbot-59.83.90/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 01:15:53.000000 jzchatbot-59.83.90/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 01:35:08.195824 jzchatbot-59.83.90/jzchatbot/
--rw-rw-rw-   0        0        0     4111 2024-05-10 01:33:48.000000 jzchatbot-59.83.90/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:35:08.231270 jzchatbot-59.83.90/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-10 01:35:08.000000 jzchatbot-59.83.90/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 01:35:08.239445 jzchatbot-59.83.90/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-10 01:34:57.000000 jzchatbot-59.83.90/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:39:42.020311 jzchatbot-59.83.91/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.91/LICENSE
+-rw-rw-rw-   0        0        0      343 2024-05-10 01:39:42.017908 jzchatbot-59.83.91/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 01:15:53.000000 jzchatbot-59.83.91/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 01:39:41.983720 jzchatbot-59.83.91/jzchatbot/
+-rw-rw-rw-   0        0        0     4109 2024-05-10 01:39:31.000000 jzchatbot-59.83.91/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:39:42.015488 jzchatbot-59.83.91/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-10 01:39:41.000000 jzchatbot-59.83.91/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-10 01:39:41.000000 jzchatbot-59.83.91/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 01:39:41.000000 jzchatbot-59.83.91/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-10 01:39:41.000000 jzchatbot-59.83.91/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 01:39:41.000000 jzchatbot-59.83.91/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 01:39:42.020311 jzchatbot-59.83.91/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-10 01:39:34.000000 jzchatbot-59.83.91/setup.py
```

### Comparing `jzchatbot-59.83.90/LICENSE` & `jzchatbot-59.83.91/LICENSE`

 * *Files identical despite different names*

### Comparing `jzchatbot-59.83.90/jzchatbot/__init__.py` & `jzchatbot-59.83.91/jzchatbot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,76 +3,15 @@
 import json
 import pyttsx3
 import speech_recognition as sr
 from nltk.tokenize import word_tokenize
 from nltk.corpus import stopwords
 from textblob import TextBlob
 
-class Bot:
-    def __init__(self, name, jsonfile):
-        self.name = name
-        self.conversations = self.load_conversations(jsonfile)
-        self.engine = pyttsx3.init()
-
-    def preprocess_text(self, text):
-        # Correct spelling mistakes using TextBlob
-        corrected_text = str(TextBlob(text).correct())
-
-        # Tokenization
-        tokens = word_tokenize(corrected_text)
-
-        # Stopword removal and remove non-alphabetic characters
-        stop_words = set(stopwords.words('english'))
-        tokens = [re.sub(r'[^a-zA-Z]', '', token).lower() for token in tokens if token.lower() not in stop_words]
-
-        # Remove empty tokens
-        tokens = [token for token in tokens if token]
-
-        return tokens
-
-    def generate_response(self, user_input):
-        max_similarity = 0
-        best_response = None
-        try:
-            for entry in self.conversations:
-                question = entry["question"]
-                question_tokens = self.preprocess_text(question)
-                user_input_tokens = self.preprocess_text(user_input)
-                common_tokens = set(question_tokens) & set(user_input_tokens)
-                similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens))
-
-                if similarity > max_similarity:
-                    max_similarity = similarity
-                    best_response = entry.get("answers", ["I'm sorry, I don't have a response for that."])
-
-            if best_response:
-                return random.choice(best_response)
-            else:
-                return "I'm sorry, I didn't understand your question."
-            
-        except ZeroDivisionError:
-            return "Minimum of 4 characters and/or numbers."
-        
-        except BaseException as e:
-            return f"Error: {e}"
-
-    def speak(self, text):
-        self.engine.say(text)
-        self.engine.runAndWait()
-
-    def load_conversations(self, file_path):
-        with open(file_path, 'r') as file:
-            return json.load(file)
-
-    def usrinput(self, cmd):
-        bot_response = self.generate_response(cmd)
-        print(f"{self.name}: {bot_response}")
-        self.speak(bot_response)
-        
-    def gencode(pyfilename, jsonfilename, botname):
+def gencode(pyfilename, jsonfilename, botname):
         with open(pyfilename, "w+") as file:
             file.write(f"""
 import jzchatbot as jz
                        
 ai = jz.Bot(name='{botname}',jsonfile='{jsonfilename}')
                        
 while True:
@@ -132,7 +71,70 @@
             """
             f"My name is {botname}""""
         ]
     }
 ]
                        
                        """)
+
+
+class Bot:
+    def __init__(self, name, jsonfile):
+        self.name = name
+        self.conversations = self.load_conversations(jsonfile)
+        self.engine = pyttsx3.init()
+
+    def preprocess_text(self, text):
+        # Correct spelling mistakes using TextBlob
+        corrected_text = str(TextBlob(text).correct())
+
+        # Tokenization
+        tokens = word_tokenize(corrected_text)
+
+        # Stopword removal and remove non-alphabetic characters
+        stop_words = set(stopwords.words('english'))
+        tokens = [re.sub(r'[^a-zA-Z]', '', token).lower() for token in tokens if token.lower() not in stop_words]
+
+        # Remove empty tokens
+        tokens = [token for token in tokens if token]
+
+        return tokens
+
+    def generate_response(self, user_input):
+        max_similarity = 0
+        best_response = None
+        try:
+            for entry in self.conversations:
+                question = entry["question"]
+                question_tokens = self.preprocess_text(question)
+                user_input_tokens = self.preprocess_text(user_input)
+                common_tokens = set(question_tokens) & set(user_input_tokens)
+                similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens))
+
+                if similarity > max_similarity:
+                    max_similarity = similarity
+                    best_response = entry.get("answers", ["I'm sorry, I don't have a response for that."])
+
+            if best_response:
+                return random.choice(best_response)
+            else:
+                return "I'm sorry, I didn't understand your question."
+            
+        except ZeroDivisionError:
+            return "Minimum of 4 characters and/or numbers."
+        
+        except BaseException as e:
+            return f"Error: {e}"
+
+    def speak(self, text):
+        self.engine.say(text)
+        self.engine.runAndWait()
+
+    def load_conversations(self, file_path):
+        with open(file_path, 'r') as file:
+            return json.load(file)
+
+    def usrinput(self, cmd):
+        bot_response = self.generate_response(cmd)
+        print(f"{self.name}: {bot_response}")
+        self.speak(bot_response)
+
```

### Comparing `jzchatbot-59.83.90/setup.py` & `jzchatbot-59.83.91/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.90", 
+	version="59.83.91", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

