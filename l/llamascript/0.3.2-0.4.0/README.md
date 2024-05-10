# Comparing `tmp/llamascript-0.3.2.tar.gz` & `tmp/llamascript-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.3.2.tar", last modified: Sat May  4 19:00:43 2024, max compression
+gzip compressed data, was "llamascript-0.4.0.tar", last modified: Fri May 10 16:27:47 2024, max compression
```

## Comparing `llamascript-0.3.2.tar` & `llamascript-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:00:43.482303 llamascript-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-04 19:00:39.000000 llamascript-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-04 19:00:43.482303 llamascript-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-04 19:00:39.000000 llamascript-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:00:43.478303 llamascript-0.3.2/llamascript/
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-04 19:00:39.000000 llamascript-0.3.2/llamascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-04 19:00:39.000000 llamascript-0.3.2/llamascript/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:00:43.482303 llamascript-0.3.2/llamascript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-04 19:00:43.000000 llamascript-0.3.2/llamascript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-04 19:00:43.000000 llamascript-0.3.2/llamascript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:00:43.000000 llamascript-0.3.2/llamascript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 19:00:43.000000 llamascript-0.3.2/llamascript.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 19:00:43.000000 llamascript-0.3.2/llamascript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 19:00:43.000000 llamascript-0.3.2/llamascript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 19:00:43.482303 llamascript-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-04 19:00:39.000000 llamascript-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:47.251244 llamascript-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-10 16:27:42.000000 llamascript-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-10 16:27:47.251244 llamascript-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-10 16:27:42.000000 llamascript-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:47.251244 llamascript-0.4.0/llamascript/
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-10 16:27:42.000000 llamascript-0.4.0/llamascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-10 16:27:42.000000 llamascript-0.4.0/llamascript/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:47.251244 llamascript-0.4.0/llamascript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-10 16:27:47.000000 llamascript-0.4.0/llamascript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-10 16:27:47.000000 llamascript-0.4.0/llamascript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:27:47.000000 llamascript-0.4.0/llamascript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 16:27:47.000000 llamascript-0.4.0/llamascript.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 16:27:47.000000 llamascript-0.4.0/llamascript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 16:27:47.000000 llamascript-0.4.0/llamascript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:27:47.251244 llamascript-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-10 16:27:42.000000 llamascript-0.4.0/setup.py
```

### Comparing `llamascript-0.3.2/LICENSE` & `llamascript-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llamascript-0.3.2/PKG-INFO` & `llamascript-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.3.2
+Version: 0.4.0
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llamascript-0.3.2/README.md` & `llamascript-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `llamascript-0.3.2/llamascript/__init__.py` & `llamascript-0.4.0/llamascript/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import asyncio
 import ollama
 import logging
+import sys
+import subprocess
+import os
 
 # Set up logging
 logging.basicConfig(level=logging.WARNING)
 
 
 class llama:
     def __init__(self):
@@ -63,14 +66,44 @@
         if command == "SYSTEM":
             self.SYSTEM(p=input("Enter system prompt: "))
         elif command == "PROMPT":
             self.PROMPT(p=input("Enter prompt: "))
         else:
             raise ValueError("Invalid command for INPUT")
 
+    def CREATE_MODEL(self, filename, parameters, model_name):
+        try:
+            with open(filename, "w") as file:
+                file.write(
+                    f'FROM {parameters["model"]}\nPARAMETER temperature {parameters["temperature"]}\nSYSTEM """\n{parameters["system_message"]}\n"""\n'
+                )
+            print(f"Modelfile created.")
+            command = ["ollama", "create", model_name, "-f", "./Modelfile"]
+            process = subprocess.Popen(
+                command,
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+                creationflags=subprocess.CREATE_NO_WINDOW,
+            )
+            stdout, stderr = process.communicate()
+            print("Model created.")
+
+            if process.returncode != 0:
+                if stderr is not None:
+                    print(f"Error executing command: {stderr.decode()}")
+                else:
+                    if stdout is not None:
+                        print(stdout.decode())
+            print("Removing Modelfile...")
+            os.remove(filename)
+
+        except Exception as e:
+            logging.error("Error creating model file: %s", e)
+            print(f"Error creating model file {filename}.")
+
     async def read(self, filename):
         try:
             with open(filename, "r") as file:
                 for line in file:
                     line = line.strip()
                     if not line:
                         continue
@@ -81,14 +114,26 @@
                         self.USE(line)
                     elif len(command) > 1 and command[1] == "INPUT":
                         self.INPUT(command[0])
                     elif command[0] == "SYSTEM":
                         self.SYSTEM(line=line)
                     elif command[0] == "PROMPT":
                         self.PROMPT(line=line)
+                    elif command[0] == "SAVE":
+                        if len(command) < 2:
+                            logging.error("No filename provided")
+                            print("No filename provided")
+                            sys.exit(1)
+                        model_name = command[1]
+                        parameters = {
+                            "model": self.model,
+                            "temperature": command[2] if len(command) > 2 else 0.7,
+                            "system_message": self.system[0]["content"],
+                        }
+                        self.CREATE_MODEL("Modelfile", parameters, model_name)
                     elif command[0] == "CHAT":
                         if len(command) > 1 and command[1] == "STREAM":
                             stream = command[1] == True
                         else:
                             stream = False
                         if not self.ignore:
                             print(
@@ -108,12 +153,21 @@
 
 def run():
     parser = argparse.ArgumentParser(description="Run llama script.")
     parser.add_argument("file_name", type=str, help="The name of the file to run")
 
     args = parser.parse_args()
 
+    if not (args.file_name.endswith(".llama") or args.filename == "llama"):
+        logging.error("Invalid file type. Please provide a .llama or llama file.")
+        print("Invalid file type. Please provide a .llama or llama file.")
+        sys.exit(1)
+
     try:
         l = llama()
         asyncio.run(l.read(args.file_name))
     except KeyboardInterrupt:
         pass
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `llamascript-0.3.2/llamascript/test.py` & `llamascript-0.4.0/llamascript/test.py`

 * *Files identical despite different names*

### Comparing `llamascript-0.3.2/llamascript.egg-info/PKG-INFO` & `llamascript-0.4.0/llamascript.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.3.2
+Version: 0.4.0
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llamascript-0.3.2/setup.py` & `llamascript-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="llamascript",
-    version="0.3.2",
+    version="0.4.0",
     author="WolfTheDev",
     author_email="wolfthedev@gmail.com",
     description="No-code AI chatbot using Ollama.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/WolfTheDeveloper/llamascript",
     packages=setuptools.find_packages(),
```

