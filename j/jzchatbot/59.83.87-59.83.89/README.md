# Comparing `tmp/jzchatbot-59.83.87.tar.gz` & `tmp/jzchatbot-59.83.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.87.tar", last modified: Thu May  9 01:18:31 2024, max compression
+gzip compressed data, was "jzchatbot-59.83.89.tar", last modified: Thu May  9 03:31:36 2024, max compression
```

## Comparing `jzchatbot-59.83.87.tar` & `jzchatbot-59.83.89.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 01:18:31.476604 jzchatbot-59.83.87/
--rw-rw-rw-   0        0        0        0 2024-05-09 01:16:02.000000 jzchatbot-59.83.87/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-09 01:18:31.475152 jzchatbot-59.83.87/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 01:15:53.000000 jzchatbot-59.83.87/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 01:18:31.415638 jzchatbot-59.83.87/jzchatbot/
--rw-rw-rw-   0        0        0     2186 2024-05-09 01:14:16.000000 jzchatbot-59.83.87/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 01:18:31.473133 jzchatbot-59.83.87/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-09 01:18:31.000000 jzchatbot-59.83.87/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-09 01:18:31.000000 jzchatbot-59.83.87/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 01:18:31.000000 jzchatbot-59.83.87/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-09 01:18:31.000000 jzchatbot-59.83.87/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 01:18:31.000000 jzchatbot-59.83.87/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 01:18:31.479125 jzchatbot-59.83.87/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-09 01:18:01.000000 jzchatbot-59.83.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 03:31:36.140287 jzchatbot-59.83.89/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.89/LICENSE
+-rw-rw-rw-   0        0        0      343 2024-05-09 03:31:36.137669 jzchatbot-59.83.89/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 01:15:53.000000 jzchatbot-59.83.89/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 03:31:36.099199 jzchatbot-59.83.89/jzchatbot/
+-rw-rw-rw-   0        0        0     2441 2024-05-09 03:31:14.000000 jzchatbot-59.83.89/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 03:31:36.132777 jzchatbot-59.83.89/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 03:31:36.140287 jzchatbot-59.83.89/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-09 03:26:03.000000 jzchatbot-59.83.89/setup.py
```

### Comparing `jzchatbot-59.83.87/jzchatbot/__init__.py` & `jzchatbot-59.83.89/jzchatbot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,36 @@
         tokens = [token for token in tokens if token]
 
         return tokens
 
     def generate_response(self, user_input):
         max_similarity = 0
         best_response = None
-
-        for entry in self.conversations:
-            question = entry["question"]
-            question_tokens = self.preprocess_text(question)
-            user_input_tokens = self.preprocess_text(user_input)
-            common_tokens = set(question_tokens) & set(user_input_tokens)
-            similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens))
-
-            if similarity > max_similarity:
-                max_similarity = similarity
-                best_response = entry.get("answers", ["I'm sorry, I don't have a response for that."])
-
-        if best_response:
-            return random.choice(best_response)
-        else:
-            return "I'm sorry, I didn't understand your question."
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
 
     def speak(self, text):
         self.engine.say(text)
         self.engine.runAndWait()
 
     def load_conversations(self, file_path):
         with open(file_path, 'r') as file:
```

### Comparing `jzchatbot-59.83.87/setup.py` & `jzchatbot-59.83.89/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.87", 
+	version="59.83.89", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

