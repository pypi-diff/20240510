# Comparing `tmp/PerplexiPy-1.0.7-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12557 bytes, number of entries: 10
--rw-r--r--  2.0 unx     9961 b- defN 24-May-08 14:30 perplexipy/__init__.py
--rw-r--r--  2.0 unx    13411 b- defN 24-May-05 02:46 perplexipy/codex.py
+Zip file size: 13010 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9961 b- defN 24-May-08 14:36 perplexipy/__init__.py
+-rw-r--r--  2.0 unx    14793 b- defN 24-May-10 04:49 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6968 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      814 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/RECORD
-10 files, 33787 bytes uncompressed, 11165 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-10 04:50 PerplexiPy-1.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6968 b- defN 24-May-10 04:50 PerplexiPy-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 04:50 PerplexiPy-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-10 04:50 PerplexiPy-1.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-10 04:50 PerplexiPy-1.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      814 b- defN 24-May-10 04:50 PerplexiPy-1.0.8.dist-info/RECORD
+10 files, 35169 bytes uncompressed, 11618 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.7.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.7.dist-info/METADATA
+Filename: PerplexiPy-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.7.dist-info/WHEEL
+Filename: PerplexiPy-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.7.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.7.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.7.dist-info/RECORD
+Filename: PerplexiPy-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/codex.py

```diff
@@ -75,14 +75,15 @@
 
 class CodexREPL:
 
     def __init__(self):
         self._client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
         self._client.model = DEFAULT_MODEL_NAME
         self._queryCodeStyle = True
+        self._editingMode = EditingMode.VI
 
 
     def core(self, userQuery: str) -> str:
         """
         Send a user query to the model for processing.
 
         Arguments
@@ -91,14 +92,15 @@
         A string with the user query, most often a programming question.
 
         Returns
         -------
         The result of the query, or `None` if the query was empty.
         """
         result = None
+        userQuery = userQuery.strip()
         if userQuery:
             if not self._client:
                 self._client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
                 self._client.model = DEFAULT_MODEL_NAME
             result = self._client.query(userQuery)
 
         return result
@@ -113,45 +115,81 @@
             except:
                 click.secho('Invalid model ID = %s' % modelID, bg = 'red', fg = 'white')
         click.secho('Active model: %s\n' % self._client.model, fg = 'green', bold = True)
         return self._client.model
 
 
 
-    def _displayModels(self) -> list:
+    def displayModels(self) -> list:
         """
         Display the list of models supported by the API.
 
         Returns
         =======
         A list of strings, each corresponding to a model name.
         """
-        _activeModel()
+        self.activeModel()
         print('Available models:\n')
         n = 1
         for model in self._client.models.keys():
             print('%2d - %s' % (n, model))
             n += 1
         print()
 
         return list(self._client.models.keys())
 
 
-    def editingMode(self, session: PromptSession, mode = None) -> PromptSession:
+    def editingMode(self, session: PromptSession, mode: str = None) -> PromptSession:
+        """
+        Sets the editing mode to `vi` or `emacs`.
+
+        Arguments
+        =========
+            session
+        An instance of `PromptSession` from the current Click hosting.
+
+            mode
+        A string with the values of 'vi' or 'emacs'; any other value is
+        overriden with `vi`.
+
+        Returns
+        =======
+        An updated PromptSession instance that with the value of `mode`.
+        """
         if mode:
             mode = mode.lower()
-            newEditingMode = EditingMode.EMACS if mode == 'emacs' else EditingMode.VI
-            session = PromptSession(editing_mode = newEditingMode)
+            self._editingMode = EditingMode.EMACS if mode == 'emacs' else EditingMode.VI
+            session = PromptSession(editing_mode = self._editingMode)
 
         editingMode = str(session.editing_mode).replace('EditingMode.', '').lower()
         click.secho('Editing mode = %s' % editingMode, fg = 'bright_blue')
 
         return session
 
-    def _queryStyle(self, newStyle: str = None) -> bool:
+    def queryStyle(self, newStyle: str = None) -> bool:
+        """
+        Set the receiver query style to `newStyle`.  Code style queries generate
+        responses that include code snippets in Python or JavaScript, and URLs
+        to references that show how to address the query topic.  `human` style
+        queries produce textual, prose responses that address the query topic in
+        detail, and may or may not contain code, even if the query was about a
+        programming concept.
+
+        Arguments
+        =========
+            `newStyle`
+        A string with either value of 'code' or 'human'.
+
+        Returns
+        =======
+        `True` if the current style is code, `False` for human.  The object uses
+        this Boolean value to determine the type of query to execute.  Future
+        versions may use the words `code` or `human`, or perhaps an enum with
+        those values.
+        """
         if newStyle:
             self._queryCodeStyle = newStyle != 'human'
         click.secho('Coding query style = %s' % self._queryCodeStyle, fg = 'bright_blue')
         return self._queryCodeStyle
 
     def _makeQuery(self, userQuery: str) -> str:
         if self._queryCodeStyle:
```

## Comparing `PerplexiPy-1.0.7.dist-info/LICENSE.txt` & `PerplexiPy-1.0.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.7.dist-info/METADATA` & `PerplexiPy-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.7
+Version: 1.0.8
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.7 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.8 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.7 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.8 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.7 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.8 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
```

## Comparing `PerplexiPy-1.0.7.dist-info/RECORD` & `PerplexiPy-1.0.8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 perplexipy/__init__.py,sha256=Kw2CPH3DHV8ukgVaWXOLjPWQe8Y0KOJIC0abJCU7oo8,9961
-perplexipy/codex.py,sha256=ZVTXxNkxACxtqkbn3yGd2f-xVx2jhdWWtZBbgQZL2H8,13411
+perplexipy/codex.py,sha256=OxE-3-irXxZ4ReiqhywxjndTRSHP2AzZOrsXsy7PSTs,14793
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-1.0.7.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-1.0.7.dist-info/METADATA,sha256=b1QO73ooLp1OP-zK3CFlyy5dTrw-kuCC4DAwywfm7_s,6968
-PerplexiPy-1.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-1.0.7.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-1.0.7.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-1.0.7.dist-info/RECORD,,
+PerplexiPy-1.0.8.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.0.8.dist-info/METADATA,sha256=HYsdLo7qrHq6hPXtsXe-hWz2wJOlAPhs3Wsv7-dY2IY,6968
+PerplexiPy-1.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.0.8.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.0.8.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.0.8.dist-info/RECORD,,
```

