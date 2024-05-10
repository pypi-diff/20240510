# Comparing `tmp/mdxcanvas-0.1.5.tar.gz` & `tmp/mdxcanvas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxcanvas-0.1.5.tar", max compression
+gzip compressed data, was "mdxcanvas-0.1.6.tar", max compression
```

## Comparing `mdxcanvas-0.1.5.tar` & `mdxcanvas-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2024-04-08 01:39:54.971696 mdxcanvas-0.1.5/LICENSE
--rw-r--r--   0        0        0      156 2024-04-08 01:39:54.980858 mdxcanvas-0.1.5/mdxcanvas/__init__.py
--rw-r--r--   0        0        0    20789 2024-05-08 23:33:02.372283 mdxcanvas-0.1.5/mdxcanvas/canvas_creator.py
--rw-r--r--   0        0        0     1053 2024-05-09 01:17:42.872976 mdxcanvas-0.1.5/mdxcanvas/deploy.py
--rw-r--r--   0        0        0     3393 2024-05-08 23:33:02.371732 mdxcanvas-0.1.5/mdxcanvas/document_schema.py
--rw-r--r--   0        0        0      873 2024-04-08 01:39:54.981405 mdxcanvas-0.1.5/mdxcanvas/extensions.py
--rw-r--r--   0        0        0     2689 2024-04-22 22:03:40.203135 mdxcanvas-0.1.5/mdxcanvas/jinja_parser.py
--rw-r--r--   0        0        0    25451 2024-05-09 01:17:42.874201 mdxcanvas-0.1.5/mdxcanvas/parser.py
--rw-r--r--   0        0        0      559 2024-04-12 20:46:23.699994 mdxcanvas-0.1.5/mdxcanvas/question_schema.py
--rw-r--r--   0        0        0     1878 2024-04-09 16:04:59.850313 mdxcanvas-0.1.5/mdxcanvas/templating.py
--rw-r--r--   0        0        0    15263 2024-05-08 23:33:02.371585 mdxcanvas-0.1.5/mdxcanvas/yaml_parser.py
--rw-r--r--   0        0        0      651 2024-05-09 01:06:24.390161 mdxcanvas-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 mdxcanvas-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 01:39:54.971696 mdxcanvas-0.1.6/LICENSE
+-rw-r--r--   0        0        0      156 2024-04-08 01:39:54.980858 mdxcanvas-0.1.6/mdxcanvas/__init__.py
+-rw-r--r--   0        0        0    20789 2024-05-08 23:33:02.372283 mdxcanvas-0.1.6/mdxcanvas/canvas_creator.py
+-rw-r--r--   0        0        0     1053 2024-05-09 01:17:42.872976 mdxcanvas-0.1.6/mdxcanvas/deploy.py
+-rw-r--r--   0        0        0     3393 2024-05-08 23:33:02.371732 mdxcanvas-0.1.6/mdxcanvas/document_schema.py
+-rw-r--r--   0        0        0      873 2024-04-08 01:39:54.981405 mdxcanvas-0.1.6/mdxcanvas/extensions.py
+-rw-r--r--   0        0        0     2689 2024-04-22 22:03:40.203135 mdxcanvas-0.1.6/mdxcanvas/jinja_parser.py
+-rw-r--r--   0        0        0    25647 2024-05-10 02:26:22.791075 mdxcanvas-0.1.6/mdxcanvas/parser.py
+-rw-r--r--   0        0        0      559 2024-04-12 20:46:23.699994 mdxcanvas-0.1.6/mdxcanvas/question_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-09 16:04:59.850313 mdxcanvas-0.1.6/mdxcanvas/templating.py
+-rw-r--r--   0        0        0    15263 2024-05-08 23:33:02.371585 mdxcanvas-0.1.6/mdxcanvas/yaml_parser.py
+-rw-r--r--   0        0        0      651 2024-05-10 02:28:42.504528 mdxcanvas-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 mdxcanvas-0.1.6/PKG-INFO
```

### Comparing `mdxcanvas-0.1.5/LICENSE` & `mdxcanvas-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/canvas_creator.py` & `mdxcanvas-0.1.6/mdxcanvas/canvas_creator.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/deploy.py` & `mdxcanvas-0.1.6/mdxcanvas/deploy.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/document_schema.py` & `mdxcanvas-0.1.6/mdxcanvas/document_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/extensions.py` & `mdxcanvas-0.1.6/mdxcanvas/extensions.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/jinja_parser.py` & `mdxcanvas-0.1.6/mdxcanvas/jinja_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/parser.py` & `mdxcanvas-0.1.6/mdxcanvas/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,16 +201,20 @@
             question["incorrect_comments"] = get_incorrect_comments(question_tag)
         return question, resources
 
 
 class MultipleTrueFalseProcessor:
     @staticmethod
     def process(question_tag, markdown_processor: ResourceExtractor):
-        heading_question, resources = process(TextQuestionProcessor(), question_tag, markdown_processor)
-        questions = [heading_question]
+        header_question_text, resources = markdown_processor(get_text_contents(question_tag, ["correct", "incorrect", "correct-comments", "incorrect-comments"]))
+        header_question = {
+            "question_text": header_question_text,
+            "question_type": 'text_only_question',
+        }
+        questions = [header_question]
         for answer in get_answers(question_tag):
             tf_question, res = process(TFConverter(), answer, markdown_processor)
             questions.append(tf_question)
             resources.extend(res)
         return questions, resources
```

### Comparing `mdxcanvas-0.1.5/mdxcanvas/question_schema.py` & `mdxcanvas-0.1.6/mdxcanvas/question_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/templating.py` & `mdxcanvas-0.1.6/mdxcanvas/templating.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/mdxcanvas/yaml_parser.py` & `mdxcanvas-0.1.6/mdxcanvas/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.5/pyproject.toml` & `mdxcanvas-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdxcanvas"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Canvas LMS API wrapper for maintaining content in markdown"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Preston Raab <phr23@byu.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.1.2"
```

### Comparing `mdxcanvas-0.1.5/PKG-INFO` & `mdxcanvas-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxcanvas
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Canvas LMS API wrapper for maintaining content in markdown
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

