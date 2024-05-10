# Comparing `tmp/examon_core-1.4.2.tar.gz` & `tmp/examon_core-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.4.2.tar", max compression
+gzip compressed data, was "examon_core-1.5.0.tar", max compression
```

## Comparing `examon_core-1.4.2.tar` & `examon_core-1.5.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0        0 2023-09-15 21:39:37.592646 examon_core-1.4.2/examon_core/__init__.py
--rw-r--r--   0        0        0        0 2023-08-30 17:48:12.862794 examon_core-1.4.2/examon_core/code_execution/__init__.py
--rw-r--r--   0        0        0      179 2023-08-31 08:32:56.069951 examon_core-1.4.2/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1192 2023-08-30 17:48:12.863042 examon_core-1.4.2/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
--rw-r--r--   0        0        0     1558 2023-08-30 17:48:12.863145 examon_core-1.4.2/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
--rw-r--r--   0        0        0     1381 2023-08-31 08:32:56.070773 examon_core-1.4.2/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
--rw-r--r--   0        0        0      554 2023-08-30 17:48:12.863325 examon_core-1.4.2/examon_core/code_execution/print_collector.py
--rw-r--r--   0        0        0     1093 2023-08-30 17:48:12.863416 examon_core-1.4.2/examon_core/code_execution/restricted_python_driver.py
--rw-r--r--   0        0        0      665 2023-08-30 17:48:12.863539 examon_core-1.4.2/examon_core/code_execution/sandbox.py
--rw-r--r--   0        0        0      686 2023-08-30 17:48:12.863723 examon_core-1.4.2/examon_core/code_execution/unrestricted_driver.py
--rw-r--r--   0        0        0      192 2023-09-15 21:39:37.592836 examon_core-1.4.2/examon_core/examon_filter_options.py
--rwxr-xr-x   0        0        0     2011 2023-09-15 21:39:37.592973 examon_core-1.4.2/examon_core/examon_in_memory_db.py
--rwxr-xr-x   0        0        0      710 2023-09-15 21:39:37.593140 examon_core-1.4.2/examon_core/examon_item.py
--rw-r--r--   0        0        0      199 2023-08-30 17:48:12.864091 examon_core-1.4.2/examon_core/examon_serializer.py
--rw-r--r--   0        0        0        0 2023-08-31 06:10:13.104902 examon_core-1.4.2/examon_core/metrics/__init__.py
--rw-r--r--   0        0        0     9971 2023-09-16 07:20:42.962887 examon_core-1.4.2/examon_core/metrics/code_analysis_visitor.py
--rw-r--r--   0        0        0     1478 2023-10-14 12:32:50.056651 examon_core-1.4.2/examon_core/metrics/metrics_factory.py
--rw-r--r--   0        0        0        0 2023-08-30 17:48:12.864191 examon_core-1.4.2/examon_core/models/__init__.py
--rw-r--r--   0        0        0      171 2023-08-31 08:32:56.067693 examon_core-1.4.2/examon_core/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      558 2023-08-31 08:32:56.103106 examon_core-1.4.2/examon_core/models/__pycache__/question_response.cpython-39.pyc
--rw-r--r--   0        0        0      825 2023-09-15 21:39:37.593637 examon_core-1.4.2/examon_core/models/code_metrics.py
--rw-r--r--   0        0        0        0 2023-08-30 17:48:12.864768 examon_core-1.4.2/examon_core/models/factories/__init__.py
--rw-r--r--   0        0        0      542 2023-08-30 17:48:12.864919 examon_core-1.4.2/examon_core/models/factories/base_question_factory.py
--rwxr-xr-x   0        0        0     1883 2023-08-30 17:48:12.865027 examon_core-1.4.2/examon_core/models/factories/code_as_string_factory.py
--rw-r--r--   0        0        0      783 2023-08-30 17:48:12.865116 examon_core-1.4.2/examon_core/models/factories/input_param_question_factory.py
--rw-r--r--   0        0        0      408 2023-08-30 17:48:12.865219 examon_core-1.4.2/examon_core/models/factories/multi_choice_factory.py
--rw-r--r--   0        0        0      777 2023-08-30 17:48:12.865310 examon_core-1.4.2/examon_core/models/factories/multichoice_question_factory.py
--rwxr-xr-x   0        0        0      916 2023-08-31 10:04:30.240969 examon_core-1.4.2/examon_core/models/question.py
--rw-r--r--   0        0        0     2116 2023-08-31 08:34:06.692837 examon_core-1.4.2/examon_core/models/question_factory.py
--rwxr-xr-x   0        0        0      190 2023-08-30 17:48:12.865602 examon_core-1.4.2/examon_core/models/question_response.py
--rw-r--r--   0        0        0      476 2023-10-14 13:04:21.699676 examon_core-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 examon_core-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661414 examon_core-1.5.0/examon_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661649 examon_core-1.5.0/examon_core/code_execution/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-09 16:51:06.661857 examon_core-1.5.0/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1192 2024-05-09 16:51:06.661998 examon_core-1.5.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
+-rw-r--r--   0        0        0     1558 2024-05-09 16:51:06.662136 examon_core-1.5.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
+-rw-r--r--   0        0        0     1381 2024-05-09 16:51:06.662279 examon_core-1.5.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
+-rw-r--r--   0        0        0      320 2024-05-09 16:51:06.662408 examon_core-1.5.0/examon_core/code_execution/sandbox.py
+-rw-r--r--   0        0        0      899 2024-05-10 00:29:45.323471 examon_core-1.5.0/examon_core/code_execution/unrestricted_driver.py
+-rw-r--r--   0        0        0      192 2024-05-09 16:51:06.662652 examon_core-1.5.0/examon_core/examon_filter_options.py
+-rwxr-xr-x   0        0        0     2029 2024-05-09 16:51:06.662762 examon_core-1.5.0/examon_core/examon_in_memory_db.py
+-rwxr-xr-x   0        0        0     1343 2024-05-09 23:36:29.257714 examon_core-1.5.0/examon_core/examon_item.py
+-rw-r--r--   0        0        0      199 2024-05-09 16:51:06.663045 examon_core-1.5.0/examon_core/examon_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.664432 examon_core-1.5.0/examon_core/factories/__init__.py
+-rw-r--r--   0        0        0      592 2024-05-09 23:31:08.718261 examon_core-1.5.0/examon_core/factories/base_question.py
+-rwxr-xr-x   0        0        0     1845 2024-05-09 21:57:52.629036 examon_core-1.5.0/examon_core/factories/code_to_string.py
+-rw-r--r--   0        0        0      851 2024-05-09 23:31:08.719491 examon_core-1.5.0/examon_core/factories/input_param_question.py
+-rw-r--r--   0        0        0     4595 2024-05-10 00:59:57.509738 examon_core-1.5.0/examon_core/factories/item.py
+-rw-r--r--   0        0        0     1474 2024-05-10 00:29:38.872822 examon_core-1.5.0/examon_core/factories/metrics.py
+-rw-r--r--   0        0        0      796 2024-05-10 00:48:21.153689 examon_core-1.5.0/examon_core/factories/multi_choice.py
+-rw-r--r--   0        0        0     1160 2024-05-10 00:29:45.339058 examon_core-1.5.0/examon_core/factories/multi_choice_question.py
+-rw-r--r--   0        0        0      336 2024-05-10 00:56:12.636130 examon_core-1.5.0/examon_core/generate_unique_id.py
+-rw-r--r--   0        0        0      816 2024-05-10 00:59:57.509901 examon_core-1.5.0/examon_core/global_settings.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663463 examon_core-1.5.0/examon_core/metrics/__init__.py
+-rw-r--r--   0        0        0      740 2024-05-10 00:42:15.716582 examon_core-1.5.0/examon_core/metrics/calc_standard.py
+-rw-r--r--   0        0        0      568 2024-05-10 00:29:38.862117 examon_core-1.5.0/examon_core/metrics/categorize_difficulty.py
+-rw-r--r--   0        0        0     1399 2024-05-09 17:44:54.417048 examon_core-1.5.0/examon_core/metrics/code_analysis_visitor.py
+-rw-r--r--   0        0        0     1340 2024-05-09 16:51:06.663807 examon_core-1.5.0/examon_core/metrics/visit_methods.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663934 examon_core-1.5.0/examon_core/models/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-09 16:51:06.664099 examon_core-1.5.0/examon_core/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      558 2024-05-09 16:51:06.664204 examon_core-1.5.0/examon_core/models/__pycache__/question_response.cpython-39.pyc
+-rw-r--r--   0        0        0      824 2024-05-09 17:08:36.258277 examon_core-1.5.0/examon_core/models/code_metrics.py
+-rwxr-xr-x   0        0        0      926 2024-05-09 17:09:48.272669 examon_core-1.5.0/examon_core/models/question.py
+-rwxr-xr-x   0        0        0      191 2024-05-09 16:51:06.665480 examon_core-1.5.0/examon_core/models/question_response.py
+-rw-r--r--   0        0        0      463 2024-05-09 16:51:06.666697 examon_core-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-1.5.0/PKG-INFO
```

### Comparing `examon_core-1.4.2/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc` & `examon_core-1.5.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.4.2/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc` & `examon_core-1.5.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.4.2/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc` & `examon_core-1.5.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.4.2/examon_core/examon_in_memory_db.py` & `examon_core-1.5.0/examon_core/examon_in_memory_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class ExamonInMemoryDatabase:
     __registry = []
     __tags = []
 
     @classmethod
     def add(cls, examon_item):
-        logging.debug(f'Adding {examon_item} to registry')
+        logging.debug(f"Adding {examon_item} to registry")
         cls.__registry.append(examon_item)
         for tag in examon_item.tags:
             if tag not in cls.__tags:
                 cls.__tags.append(tag)
 
     @classmethod
     def purge(cls):
@@ -51,18 +51,19 @@
                 for py_quiz_data in cls.__registry
                 if array_contains_all(examon_filter.tags_all, py_quiz_data.tags)
             ]
         if examon_filter.difficulty_category is not None:
             results = [
                 py_quiz_data
                 for py_quiz_data in cls.__registry
-                if examon_filter.difficulty_category == py_quiz_data.metrics.categorised_difficulty
+                if examon_filter.difficulty_category
+                == py_quiz_data.metrics.categorised_difficulty
             ]
 
         if examon_filter.max_questions is not None:
-            return results[0:examon_filter.max_questions]
+            return results[0 : examon_filter.max_questions]
         else:
             return results
 
     @classmethod
     def unique_tags(cls):
         return cls.__tags
```

### Comparing `examon_core-1.4.2/examon_core/models/__pycache__/question_response.cpython-39.pyc` & `examon_core-1.5.0/examon_core/models/__pycache__/question_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.4.2/examon_core/models/code_metrics.py` & `examon_core-1.5.0/examon_core/models/code_metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,22 @@
     loc: int = None
     lloc: int = None
     sloc: int = None
     difficulty: float = None
     categorised_difficulty: str = None
     imports: list[str] = None
     calls: list[str] = None
-    counts: dict = None
+    counts: dict[str, int] = None
 
     def __repr__(self):
-        return f'CodeMetrics(difficulty: {self.difficulty},' \
-               f'no_of_functions: {self.no_of_functions}, ' \
-               f'loc: {self.loc}, ' \
-               f'lloc: {self.lloc}, ' \
-               f'sloc: {self.sloc}' \
-               f'difficulty: {self.difficulty}' \
-               f'categorised_difficulty: {self.categorised_difficulty}' \
-               f'imports: {self.imports}' \
-               f'calls: {self.calls}' \
-               f'counts: {self.counts})'
+        return (
+            f"CodeMetrics(difficulty: {self.difficulty},"
+            f"no_of_functions: {self.no_of_functions}, "
+            f"loc: {self.loc}, "
+            f"lloc: {self.lloc}, "
+            f"sloc: {self.sloc}, "
+            f"difficulty: {self.difficulty}, "
+            f"categorised_difficulty: {self.categorised_difficulty}, "
+            f"imports: {self.imports}, "
+            f"calls: {self.calls}, "
+            f"counts: {self.counts})"
+        )
```

### Comparing `examon_core-1.4.2/examon_core/models/factories/code_as_string_factory.py` & `examon_core-1.5.0/examon_core/factories/code_to_string.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import inspect
 import logging
 
 
 class CodeAsStringFactory:
-    @staticmethod
-    def build(function, decorators=[]):
+    def __init__(self, decorators=None):
+        self.decorators = [] if decorators is None else decorators
+
+    def build(self, function):
         src_code = CodeAsStringFactory.function_src(function)
-        for decorator in decorators:
-            logging.debug(f'CodeAsStringFactory.build: {decorator}')
+        for decorator in self.decorators:
+            logging.debug(f"CodeAsStringFactory.build: {decorator}")
             src_code = decorator.decorate(src_code)
-            logging.debug(f'CodeAsStringFactory.build: {src_code}')
+            logging.debug(f"CodeAsStringFactory.build: {src_code}")
 
-        logging.debug(f'CodeAsStringFactory.build: {src_code}')
+        logging.debug(f"CodeAsStringFactory.build: {src_code}")
         return src_code
 
     @staticmethod
     def function_src(function):
-        logging.debug(f'CodeAsStringFactory.function_src: {function}')
+        logging.debug(f"CodeAsStringFactory.function_src: {function}")
         return inspect.getsource(function).strip()
 
 
 class SourceCodeCommentsDecorator:
     def __init__(self, hints):
         self.hints = hints
 
     def decorate(self, src_code):
-        all_hints = ''
+        all_hints = ""
         if self.hints is None:
             return all_hints
         else:
             for hint in self.hints:
-                all_hints += f'# {hint}\n'
-        all_hints = f'# Hints:\n{all_hints}\n\n'
+                all_hints += f"# {hint}\n"
+        all_hints = f"# Hints:\n{all_hints}\n\n"
         return all_hints + src_code
 
 
 class RemoveQuizItemDecorator:
     def decorate(self, src_code):
-        return src_code[src_code.find('def'):]
+        return src_code[src_code.find("def") :]
 
 
 class AppendPrintDecorator:
-    def __init__(self, function_name, param=''):
+    def __init__(self, function_name, param=""):
         self.function_name = function_name
         self.param = param
 
     def decorate(self, src_code):
-        if isinstance(self.param, str) and self.param != '':
+        if isinstance(self.param, str) and self.param != "":
             self.param = f"'{self.param}'"
-        println = f'\n\nprint({self.function_name}({self.param}))'
+        println = f"\n\nprint({self.function_name}({self.param}))"
         return src_code + println
 
 
-def default_code_as_string_factory(function, param=''):
-    append_print_decorator = AppendPrintDecorator(function.__name__, param)
-    remove_quiz_item_decorator = RemoveQuizItemDecorator()
-    decorators = [remove_quiz_item_decorator, append_print_decorator]
-    return CodeAsStringFactory.build(function, decorators)
+def default_code_as_string_factory(function, param=""):
+    return CodeAsStringFactory(
+        [RemoveQuizItemDecorator(), AppendPrintDecorator(function.__name__, param)]
+    ).build(function)
```

### Comparing `examon_core-1.4.2/examon_core/models/factories/multichoice_question_factory.py` & `examon_core-1.5.0/examon_core/factories/input_param_question.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from .multi_choice_factory import MultiChoiceFactory
-from ..question import MultiChoiceQuestion
-from .code_as_string_factory import default_code_as_string_factory
-from ...code_execution.sandbox import Sandbox
+import random
 
+from ..models.question import InputParameterQuestion
+from .code_to_string import default_code_as_string_factory
 
-class MultichoiceQuestionFactory:
-    @staticmethod
-    def build(function, choice_list):
-        function_src = default_code_as_string_factory(function)
-        print_logs = Sandbox.run_function(function_src)
-        question = MultiChoiceQuestion(
-            correct_answer=print_logs[-1],
+
+class InputParamQuestionFactory:
+    def __init__(self, code_execution_sandbox):
+        self.code_execution_sandbox = code_execution_sandbox
+
+    def build(self, function, param_one):
+        selected_input_param = random.choice(param_one)
+        function_src = default_code_as_string_factory(function, selected_input_param)
+        print_logs = self.code_execution_sandbox.execute(function_src)
+        return_value = print_logs[-1]
+        question = InputParameterQuestion(
+            selected_param=selected_input_param,
+            param_one_choices=param_one,
             function_src=function_src,
             print_logs=print_logs,
-            choices=(
-                MultiChoiceFactory.build(
-                    print_logs[-1],
-                    choice_list
-                )
-            )
         )
-
+        question.return_value = return_value
         return question
```

### Comparing `examon_core-1.4.2/examon_core/models/question.py` & `examon_core-1.5.0/examon_core/models/question.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from dataclasses import dataclass
 from typing import Any
 
 
 @dataclass
 class BaseQuestion:
+    function_src: str = None
     unique_id: str = None
     internal_id: str = None
-    function_src: str = None
-    repository: str = None
     tags: list = None
+    repository: str = None
     hints: list = None
     print_logs: list = None
     correct_answer: str = None
     metrics: Any = None
 
-    def answer(self, given_answer):
+    def answer(self, given_answer: str):
         return str(self.correct_answer) == str(given_answer)
 
 
 @dataclass
 class MultiChoiceQuestion(BaseQuestion):
     choices: dict = None
 
 
 @dataclass
 class InputParameterQuestion(BaseQuestion):
     return_value: str = None
     param_one_choices: dict = None
     selected_param: str = None
 
-    def answer(self, choice):
+    def answer(self, choice: str):
         return choice == self.selected_param
 
 
 @dataclass
 class InputParameterQuestionV2(BaseQuestion):
     result_matrix: dict[Any, Any] = None
```

