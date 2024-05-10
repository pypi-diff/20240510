# Comparing `tmp/taskgen_ai-2.0.1.tar.gz` & `tmp/taskgen_ai-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen_ai-2.0.1.tar", last modified: Thu May  9 02:33:35 2024, max compression
+gzip compressed data, was "taskgen_ai-2.1.0.tar", last modified: Fri May 10 09:46:57 2024, max compression
```

## Comparing `taskgen_ai-2.0.1.tar` & `taskgen_ai-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-09 02:33:35.822944 taskgen_ai-2.0.1/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.0.1/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21533 2024-05-09 02:33:35.822279 taskgen_ai-2.0.1/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    20924 2024-05-09 02:32:32.000000 taskgen_ai-2.0.1/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-05-09 02:32:31.000000 taskgen_ai-2.0.1/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-09 02:33:35.823159 taskgen_ai-2.0.1/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-05-09 02:32:36.000000 taskgen_ai-2.0.1/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-09 02:33:35.818533 taskgen_ai-2.0.1/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      213 2024-05-08 15:44:50.000000 taskgen_ai-2.0.1/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    32568 2024-05-08 15:59:25.000000 taskgen_ai-2.0.1/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    48888 2024-05-09 02:30:18.000000 taskgen_ai-2.0.1/taskgen/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-09 02:33:35.821468 taskgen_ai-2.0.1/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21533 2024-05-09 02:33:35.000000 taskgen_ai-2.0.1/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-05-09 02:33:35.000000 taskgen_ai-2.0.1/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-09 02:33:35.000000 taskgen_ai-2.0.1/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-05-09 02:33:35.000000 taskgen_ai-2.0.1/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-09 02:33:35.000000 taskgen_ai-2.0.1/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-10 09:46:57.640189 taskgen_ai-2.1.0/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.1.0/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21533 2024-05-10 09:46:57.639516 taskgen_ai-2.1.0/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    20924 2024-05-10 09:20:03.000000 taskgen_ai-2.1.0/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-05-10 09:20:09.000000 taskgen_ai-2.1.0/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-10 09:46:57.640379 taskgen_ai-2.1.0/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-05-10 09:19:58.000000 taskgen_ai-2.1.0/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-10 09:46:57.635994 taskgen_ai-2.1.0/taskgen/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      213 2024-05-08 15:44:50.000000 taskgen_ai-2.1.0/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    32859 2024-05-10 05:24:39.000000 taskgen_ai-2.1.0/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    51162 2024-05-10 09:33:28.000000 taskgen_ai-2.1.0/taskgen/base.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-10 09:46:57.638652 taskgen_ai-2.1.0/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21533 2024-05-10 09:46:57.000000 taskgen_ai-2.1.0/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-05-10 09:46:57.000000 taskgen_ai-2.1.0/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-10 09:46:57.000000 taskgen_ai-2.1.0/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-05-10 09:46:57.000000 taskgen_ai-2.1.0/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-10 09:46:57.000000 taskgen_ai-2.1.0/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen_ai-2.0.1/LICENSE` & `taskgen_ai-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen_ai-2.0.1/PKG-INFO` & `taskgen_ai-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.0.1
+Version: 2.1.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 
-# TaskGen v2.0.1
+# TaskGen v2.1.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

### Comparing `taskgen_ai-2.0.1/README.md` & `taskgen_ai-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TaskGen v2.0.1
+# TaskGen v2.1.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

### Comparing `taskgen_ai-2.0.1/taskgen/agent.py` & `taskgen_ai-2.1.0/taskgen/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,18 @@
 
         self.kwargs = kwargs
 
         # start with default of only llm as the function
         self.function_map = {}
         # stores all existing function descriptions - prevent duplicate assignment of functions
         self.fn_description_list = []
+        
+        # reset the memory bank
+        if 'Function' in self.memory_bank:
+            memory_bank['Function'].reset()
         # adds the use llm function
         if self.default_to_llm:
             self.assign_functions([Function(fn_name = 'use_llm', 
                                         fn_description = f'Used only when no other function can do the task', 
                                         is_compulsory = True,
                                         output_format = {"Output": "Output of LLM"})])
         # adds the end task function
@@ -301,16 +305,17 @@
     ## Functions for function calling ##
     def assign_functions(self, function_list: list):
         ''' Assigns a list of functions to be used in function_map '''
         if not isinstance(function_list, list):
             function_list = [function_list]
             
         for function in function_list:
+            # do automatic conversion of function to Function class (this is in base.py)
             if not isinstance(function, Function):
-                raise Exception('Assigned function must be of class Function')
+                function = Function(external_fn = function)
                 
             # Do not assign a function already present
             if function.fn_description in self.fn_description_list:
                 continue
             
             stored_fn_name = function.__name__
             # if function name is already in use, change name to name + '_1'. E.g. summarise -> summarise_1
@@ -376,36 +381,36 @@
             for name in self.memory_bank.keys():
                 # Function is done separately
                 if name == 'Function': continue
                 # Do not need to add to context if the memory item is empty
                 if self.memory_bank[name].isempty(): continue
                 rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(subtask)}```\n'
 
-            res = self.query(query = f'{rag_info}Context:```{self.overall_task}\n{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\nGenerate a response for Assigned Subtask only - do not just state what has or can be done or apologise or repeat Assigned Subtask - actually generate the outcome of Assigned Subtask fully according to your Agent Capabilities.', 
+            res = self.query(query = f'{rag_info}Context:```{self.overall_task}\n{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\nGenerate a response for Assigned Subtask only - do not just state what has or can be done or apologise or repeat Assigned Subtask - actually generate the outcome of Assigned Subtask fully according to your Agent Capabilities. Any mention of `use_llm` function refers to you', 
                             output_format = {"Output": "Generate a full response to the Assigned Subtask"},
                             provide_function_list = False)
             
-            res = res["Output"]
+            # res = res["Output"]
             
             if self.verbose: 
-                print('>', res)
+                print('>', res["Output"])
                 print()
             
         elif function_name == "end_task":
             return
         
         else:
             if self.verbose: 
                 print(f'Calling function {function_name} with parameters {function_params}')
                 
             res = self.function_map[function_name](**function_params, shared_variables = self.shared_variables)
 
             # if only one Output key for the json, then omit the output key
-            if len(res) == 1 and "Output" in res:
-                res = res["Output"]
+            # if len(res) == 1 and "Output" in res:
+            #     res = res["Output"]
             
             if self.verbose and res != '': 
                 print('>', res)
                 print()
                 
         if stateful:
             if res == '':
@@ -433,16 +438,16 @@
             if name == 'Function': continue
             # Do not need to add to context if the memory item is empty
             if self.memory_bank[name].isempty(): continue
             else:
                 rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(task)}```\n'
                 
         # First select the Equipped Function
-        res = self.query(query = f'''{background_info}{rag_info}\nBased on Context and Subtasks Completed, provide the Current Subtask and Equipped Function to complete part of Assigned Task. If Assigned Task is completed, Current Subtask is End Task and Equipped Function is end_task''',
-                         output_format = {"Thoughts": "How to complete Assigned Task, End Task if completed", "Observation": "Reflect on what has been done so far for Assigned Task", "Current Subtask": "What to do now in detail, End Task if completed", "Equipped Function": "Name of Equipped Function to use for Current Subtask, end_task if completed"},
+        res = self.query(query = f'''{background_info}{rag_info}\nBased on Context and Subtasks Completed, provide the Current Subtask which can be done by a single Equipped Function to complete part of Assigned Task. If Assigned Task has been completed, Current Subtask must be End Task and Equipped Function must be end_task''',
+                         output_format = {"Thoughts": "How to complete Assigned Task in detail", "Observation": "Reflect on what has been done so far for Assigned Task", "Current Subtask": "What to do now in detail, End Task if completed", "Equipped Function": "Name of Equipped Function to use for Current Subtask, end_task if completed"},
                          provide_function_list = True,
                          task = task)
         
         # end task if equipped function is incorrect
         if res["Equipped Function"] not in self.function_map:
             res["Equipped Function"] = "end_task"
```

### Comparing `taskgen_ai-2.0.1/taskgen/base.py` & `taskgen_ai-2.1.0/taskgen/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -415,65 +415,112 @@
     if verbose:
         print('System prompt:', system_prompt)
         print('\nUser prompt:', user_prompt)
         print('\nGPT response:', res)
             
     return res
 
+def get_clean_typename(typ) -> str:
+    """Returns a clean, readable name for a type, including handling generics."""
+    if hasattr(typ, '__origin__'):  # Check for generic types
+        if typ.__origin__ is not None:  # Generic types, e.g., List, Dict
+            base_name = typ.__origin__.__name__
+            if hasattr(typ, '__args__') and typ.__args__ is not None:
+                args = [get_clean_typename(arg) for arg in typ.__args__]
+                return f"{base_name}[{', '.join(args)}]"
+            else:
+                return base_name  # Handle cases like `Dict` without specified parameters
+        else:  # Non-generic but special types, e.g., typing.List without parameters
+            return typ._name if hasattr(typ, '_name') else str(typ)
+    elif hasattr(typ, '__name__'):
+        return typ.__name__  # Simple types, e.g., int, str
+    else:
+        return str(typ)  # Fallback, should rarely be used
+
 def get_fn_description(my_function) -> (str, list):
     ''' Returns the modified docstring of my_function, that takes into account input variable names and types in angle brackets
     Also returns the list of input parameters to the function in sequence
     e.g.: Adds numbers x and y -> Adds numbers <x: int> and <y: int>
     Input variables that are optional (already assigned a default value) need not be in the docstring
     args and kwargs variables are not parsed '''
      
-    # Get the signature of the function
-    if my_function.__doc__ == None:
-        return '', []
+    if not callable(my_function):
+        raise Exception(f'{my_function} is not a Python function')
+        
+    # Get the signature and type hints of the function
+    # if my_function.__doc__ == None:
+    #     return '', []
 
     signature = inspect.signature(my_function)
-    my_fn_description = my_function.__doc__
+    full_type_hints = get_type_hints(my_function)
+    my_fn_description = my_function.__doc__ if my_function.__doc__ else ''
 
     param_list = []
     # Access parameters and their types
     parameters = signature.parameters
-    if len(parameters) > 0:
-        full_param = get_type_hints(my_function)
-        for param_name, param in parameters.items():
-            # skip the shared_variables, args and kwargs
-            if param_name in ['shared_variables', 'args', 'kwargs']:
-                continue
-            # then parse the types of the param
-            param_type = param.annotation.__name__ if param.annotation != inspect.Parameter.empty else "unannotated"
-            if param_type == "unannotated":
-                new_param = f'<{param_name}>'
-            else:
-                # check if there is typing
-                if param_name in full_param:
-                    hint_str = str(full_param[param_name])
-                    if hint_str[:7] == 'typing.':
-                        param_type = hint_str[7:]
-                new_param = f'<{param_name}: {param_type}>'
-
-            # Define the regular expression pattern to match 'x' as a whole word
-            pattern = re.compile(fr'\b({param_name})\b')
-                
-            # Check if param occurs as a whole word in the docstring
-            if pattern.search(my_fn_description):
-                # Substitute each input variable x with <x> or <x: type>
-                my_fn_description = pattern.sub(new_param, my_fn_description)
-                # add this variable to the param_list
-                param_list.append(param_name)
-            else:
-                # raise exception if the parameter is not already initialised (aka LLM needs to come up with the input)
-                if param.default == inspect.Parameter.empty:
-                    raise Exception(f'Input variable "{param_name}" not in docstring of "{my_function.__name__}"')
-    
+    for param_name, param in parameters.items():
+        # skip args and kwargs and shared variables
+        if param_name in ['shared_variables', 'args', 'kwargs']:
+            continue
+        
+        param_type = param.annotation.__name__ if param.annotation != inspect.Parameter.empty else "unannotated"
+        # Handle specific typing
+        if param_name in full_type_hints:
+            param_type = get_clean_typename(full_type_hints[param_name])
+
+        # Create new_param representation
+        new_param = f'<{param_name}: {param_type}>' if param_type != "unannotated" else f'<{param_name}>'
+
+        # Pattern to find the parameter in the docstring
+        pattern = re.compile(fr'\b({param_name})\b')
+        
+        # Substitute the parameter in the docstring
+        if pattern.search(my_fn_description):
+            my_fn_description = pattern.sub(new_param, my_fn_description)
+            param_list.append(param_name)
+            
+        # otherwise, function description will just be the function signature
+        else:
+            # add a continuation if description is current empty
+            if my_fn_description != '':
+                my_fn_description += ', '
+                
+            param_list.append(param_name)
+            print(f'Input variable "{param_name}" not in docstring of "{my_function.__name__}". Adding it to docstring')
+            my_fn_description += f'Input: {new_param}'
+            
+            if param.default != inspect.Parameter.empty:
+                my_fn_description += f', default: {param.default}'
+
     return my_fn_description, param_list
 
+def get_fn_output(my_function) -> (dict):
+    ''' Returns the dictionary of output parameters and types of the form {"Output 1": "Type", "Output 2": "Type"}'''
+     
+    if not callable(my_function):
+        raise Exception(f'{my_function} is not a Python function')
+        
+    # Initialize the output format dictionary
+    output_format = {}
+
+    full_type_hints = get_type_hints(my_function)
+    my_fn_description = my_function.__doc__
+
+    # Check for return annotation
+    if 'return' in full_type_hints:
+        return_type = full_type_hints['return']
+        # Adjust dictionary according to the return type
+        if isinstance(return_type, tuple):
+            for idx, type_hint in enumerate(return_type):
+                output_format[f"output_{idx + 1}"] = get_clean_typename(type_hint)
+        else:
+            output_format["output_1"] = get_clean_typename(return_type)
+
+    return output_format
+
 ### Main Functions ###
                 
 def strict_json(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = dict(), check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
     ''' Ensures that OpenAI will always adhere to the desired output JSON format defined in output_format. 
     Uses rule-based iterative feedback to ask GPT to self-correct.
     Keeps trying up to num_tries it it does not. Returns empty JSON if unable to after num_tries iterations.
     
@@ -712,36 +759,42 @@
         ## Example
         fn_description = 'Output the sum of <num1> and <num2>'
         output_format = {'output': 'sum of two numbers'}
         examples = [{'num1': 5, 'num2': 6, 'output': 11}, {'num1': 2, 'num2': 4, 'output': 6}]
         '''
         
         self.fn_description = ''
+        self.output_format = {}
+        
         # this is only for external functions
         self.external_param_list = [] 
         if external_fn is not None:
             # add in code to warn user if type is defined for external function
             type_check = False
             for value in output_format.values():
                 if 'type:' in str(value):
                     type_check = True
             if type_check:
                 print('Note: Type checking (type:) not done for External Functions')
-            # take function description from external_fn if provided and default fn_description not provided
+            
+            # get details from docstring of external function only if fn_description is not given
             if fn_description == '':
                 self.fn_description, self.external_param_list = get_fn_description(external_fn)
             
+            # get the output format from the function signature
+            self.output_format = get_fn_output(external_fn)             
+            
         # if function description provided, use it to update the function description
         if fn_description != '':
             self.fn_description = fn_description
-        # if there is no external function docstring provided, raise an error
-        elif self.fn_description == '':
-            raise Exception('Input variable "fn_description" (or docstring for External Functions) not provided')
 
-        self.output_format = output_format
+        # if output format is provided, use it to update the function output format
+        if output_format != {}:
+            self.output_format = output_format
+            
         self.examples = examples
         self.external_fn = external_fn
         self.is_compulsory = is_compulsory
         self.fn_name = fn_name
         self.llm = llm
         self.llm_async = llm_async
         self.kwargs = kwargs
@@ -848,15 +901,18 @@
             if fn_output is not None:
                 output_keys = list(self.output_format.keys())
                 # convert the external function into a tuple format to parse it through the JSON dictionary output format
                 if not isinstance(fn_output, tuple):
                     fn_output = [fn_output]
 
                 for i in range(len(fn_output)):
-                    res[output_keys[i]] = fn_output[i]
+                    if len(output_keys) > i:
+                        res[output_keys[i]] = fn_output[i]
+                    else:
+                        res[f'output_{i+1}'] = fn_output[i]
         
         # check if any of the output variables have a s_, which means we update the shared_variables and not output it
         keys = list(res.keys())
         for each in keys:
             if each[:2] == 's_':
                 shared_variables[each] = res[each]
                 del res[each]
@@ -922,15 +978,18 @@
             if fn_output is not None:
                 output_keys = list(self.output_format.keys())
                 # convert the external function into a tuple format to parse it through the JSON dictionary output format
                 if not isinstance(fn_output, tuple):
                     fn_output = [fn_output]
 
                 for i in range(len(fn_output)):
-                    res[output_keys[i]] = fn_output[i]
+                    if len(output_keys) > i:
+                        res[output_keys[i]] = fn_output[i]
+                    else:
+                        res[f'output_{i+1}'] = fn_output[i]
         
         # check if any of the output variables have a s_, which means we update the shared_variables and not output it
         keys = list(res.keys())
         for each in keys:
             if each[:2] == 's_':
                 shared_variables[each] = res[each]
                 del res[each]
```

### Comparing `taskgen_ai-2.0.1/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-2.1.0/taskgen_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.0.1
+Version: 2.1.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 
-# TaskGen v2.0.1
+# TaskGen v2.1.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

