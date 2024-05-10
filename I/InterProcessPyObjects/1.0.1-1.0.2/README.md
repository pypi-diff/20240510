# Comparing `tmp/interprocesspyobjects-1.0.1.tar.gz` & `tmp/interprocesspyobjects-1.0.2.tar.gz`

## Comparing `interprocesspyobjects-1.0.1.tar` & `interprocesspyobjects-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/ipc_py_objects/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/ipc_py_objects/versions/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/ipc_py_objects/versions/v_0/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/ipc_py_objects/versions/v_1/__init__.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/LICENSE.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/NOTICE
--rw-r--r--   0        0        0    34158 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/README.md
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    38774 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/versions/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_0/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_1/__init__.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/NOTICE
+-rw-r--r--   0        0        0    37439 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/README.md
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/PKG-INFO
```

### Comparing `interprocesspyobjects-1.0.1/ipc_py_objects/__init__.py` & `interprocesspyobjects-1.0.2/ipc_py_objects/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 """
 
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 __status__ = "Production"
 
 
 from .versions import *
```

### Comparing `interprocesspyobjects-1.0.1/ipc_py_objects/versions/__init__.py` & `interprocesspyobjects-1.0.2/ipc_py_objects/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.1/ipc_py_objects/versions/v_0/__init__.py` & `interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.1/ipc_py_objects/versions/v_1/__init__.py` & `interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.1/.gitignore` & `interprocesspyobjects-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.1/LICENSE.md` & `interprocesspyobjects-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.1/NOTICE` & `interprocesspyobjects-1.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.1/README.md` & `interprocesspyobjects-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -169,14 +169,64 @@
 ## Examples
 
 * An async examples (with asyncio):
     * [sender.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/sender.py)
     * [receiver.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/receiver.py)
     * [shared_objects__types.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/shared_objects__types.py)
 
+### Receiver.py performance measurements
+
+```python
+sso: SomeSharedObject = None  # variable for our shared object
+
+async with ashared_memory_context_manager.if_has_messages() as shared_memory:
+    sso = shared_memory.value.take_message()  # 5_833 iterations/seconds
+    company_metrics = sso.company_info.company_metrics  # 12_479 iterations/seconds
+    k = company_metrics[CompanyMetrics.in_a_good_state]  # 1_154_454 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = False  # 1_213_175 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = None  # 1_188_630 iterations/seconds
+    k = company_metrics[CompanyMetrics.employees]  # 1_498_278 iterations/seconds
+    company_metrics[CompanyMetrics.employees] = 20  # 1_352_799 iterations/seconds
+    company_metrics[CompanyMetrics.employees] += 1  # 247_476 iterations/seconds
+    k = company_metrics[CompanyMetrics.avg_salary]  # 1_535_267 iterations/seconds
+    company_metrics[CompanyMetrics.avg_salary] = 5_000.0  # 1_300_966 iterations/seconds
+    company_metrics[CompanyMetrics.avg_salary] += 1.1  # 299_415 iterations/seconds
+    k = sso.int_value  # 850_098 iterations/seconds
+    sso.int_value = 200  # 207_480 iterations/seconds
+    sso.int_value += 1  # 152_263 iterations/seconds
+    company_metrics[CompanyMetrics.annual_income] = 2_000_000.0  # 1_380_983 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = tuple()  # 55_335 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com',)  # 30_314 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com', 'support@company.com')  # 20_860 iterations/seconds
+    k = company_metrics[CompanyMetrics.websites]  # 380_258 iterations/seconds
+    company_metrics[CompanyMetrics.websites] = ['http://company.com', 'http://company.org']  # 10_465 iterations/seconds
+    k = sso.str_value  # 228_966 iterations/seconds
+    sso.str_value = 'Hello. '  # 52_390 iterations/seconds
+    sso.str_value += '!'  # 35_823 iterations/seconds
+    data_dict = sso.data_dict  # 16_362 iterations/seconds
+    k = data_dict['key1']  # 87_558 iterations/seconds
+    data_dict['key1'] = 200  # 86_744 iterations/seconds
+    data_dict['key1'] *= 1  # 40_927 iterations/seconds
+    data_dict['key1'] += 3  # 41_409 iterations/seconds
+    k = data_dict[('key', 2)]  # 49_338 iterations/seconds
+    data_dict[('key', 2)] = 'value2'  # 31_460 iterations/seconds
+    data_dict[('key', 2)] = data_dict[('key', 2)] + 'd'  # 18_972 iterations/seconds
+    data_dict[('key', 2)] = 'value2'  # 10_941 iterations/seconds
+    data_dict[('key', 2)] += 'd'  # 16_568 iterations/seconds
+    ndarray: np.ndarray = data_dict['key3']  # 26_223 iterations/seconds
+    ndarray += 10  # 403_246 iterations/seconds
+    data_dict['key3'] += 10  # 6_319 iterations/seconds
+    k = sso.company_info.income  # 20_445 iterations/seconds
+    sso.company_info.income = 3_000_000.0  # 13_899 iterations/seconds
+    sso.company_info.income *= 1.1  # 17_272 iterations/seconds 
+    sso.company_info.income += 500_000.0  # 18_376 iterations/seconds
+    sso.company_info.some_employee.increase_years_of_employment()  # 9_429 iterations/seconds
+    sso.some_processing_stage_control = True  # 298_968 iterations/seconds
+```
+
 ## Reference (and explaining examples line by line)
 
 Code for shared memory Creator side:
 ```python
 ashared_memory_manager: ASharedMemoryManager = ASharedMemoryManager(SharedMemory('shared_memory_identifier', create=True, size=200 * 1024**2))
 # declare creation and initiation of the shared memory instance with a size of 200 MiB.
 ```
```

### Comparing `interprocesspyobjects-1.0.1/pyproject.toml` & `interprocesspyobjects-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.1/PKG-INFO` & `interprocesspyobjects-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: InterProcessPyObjects
-Version: 1.0.1
+Version: 1.0.2
 Summary: This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency
 Project-URL: Homepage, https://github.com/FI-Mihej/InterProcessPyObjects
 Author-email: ButenkoMS <gtalk@butenkoms.space>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 License-File: NOTICE
 Keywords: Android,IPC,Linux,Windows,cengal,crossplatform,iOS,inter-process communication,macOS,multiprocessing,shared dict,shared memory,shared numpy ndarray,shared object,shared objects,shared set,shared torch Tensor
@@ -261,14 +261,64 @@
 ## Examples
 
 * An async examples (with asyncio):
     * [sender.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/sender.py)
     * [receiver.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/receiver.py)
     * [shared_objects__types.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/shared_objects__types.py)
 
+### Receiver.py performance measurements
+
+```python
+sso: SomeSharedObject = None  # variable for our shared object
+
+async with ashared_memory_context_manager.if_has_messages() as shared_memory:
+    sso = shared_memory.value.take_message()  # 5_833 iterations/seconds
+    company_metrics = sso.company_info.company_metrics  # 12_479 iterations/seconds
+    k = company_metrics[CompanyMetrics.in_a_good_state]  # 1_154_454 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = False  # 1_213_175 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = None  # 1_188_630 iterations/seconds
+    k = company_metrics[CompanyMetrics.employees]  # 1_498_278 iterations/seconds
+    company_metrics[CompanyMetrics.employees] = 20  # 1_352_799 iterations/seconds
+    company_metrics[CompanyMetrics.employees] += 1  # 247_476 iterations/seconds
+    k = company_metrics[CompanyMetrics.avg_salary]  # 1_535_267 iterations/seconds
+    company_metrics[CompanyMetrics.avg_salary] = 5_000.0  # 1_300_966 iterations/seconds
+    company_metrics[CompanyMetrics.avg_salary] += 1.1  # 299_415 iterations/seconds
+    k = sso.int_value  # 850_098 iterations/seconds
+    sso.int_value = 200  # 207_480 iterations/seconds
+    sso.int_value += 1  # 152_263 iterations/seconds
+    company_metrics[CompanyMetrics.annual_income] = 2_000_000.0  # 1_380_983 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = tuple()  # 55_335 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com',)  # 30_314 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com', 'support@company.com')  # 20_860 iterations/seconds
+    k = company_metrics[CompanyMetrics.websites]  # 380_258 iterations/seconds
+    company_metrics[CompanyMetrics.websites] = ['http://company.com', 'http://company.org']  # 10_465 iterations/seconds
+    k = sso.str_value  # 228_966 iterations/seconds
+    sso.str_value = 'Hello. '  # 52_390 iterations/seconds
+    sso.str_value += '!'  # 35_823 iterations/seconds
+    data_dict = sso.data_dict  # 16_362 iterations/seconds
+    k = data_dict['key1']  # 87_558 iterations/seconds
+    data_dict['key1'] = 200  # 86_744 iterations/seconds
+    data_dict['key1'] *= 1  # 40_927 iterations/seconds
+    data_dict['key1'] += 3  # 41_409 iterations/seconds
+    k = data_dict[('key', 2)]  # 49_338 iterations/seconds
+    data_dict[('key', 2)] = 'value2'  # 31_460 iterations/seconds
+    data_dict[('key', 2)] = data_dict[('key', 2)] + 'd'  # 18_972 iterations/seconds
+    data_dict[('key', 2)] = 'value2'  # 10_941 iterations/seconds
+    data_dict[('key', 2)] += 'd'  # 16_568 iterations/seconds
+    ndarray: np.ndarray = data_dict['key3']  # 26_223 iterations/seconds
+    ndarray += 10  # 403_246 iterations/seconds
+    data_dict['key3'] += 10  # 6_319 iterations/seconds
+    k = sso.company_info.income  # 20_445 iterations/seconds
+    sso.company_info.income = 3_000_000.0  # 13_899 iterations/seconds
+    sso.company_info.income *= 1.1  # 17_272 iterations/seconds 
+    sso.company_info.income += 500_000.0  # 18_376 iterations/seconds
+    sso.company_info.some_employee.increase_years_of_employment()  # 9_429 iterations/seconds
+    sso.some_processing_stage_control = True  # 298_968 iterations/seconds
+```
+
 ## Reference (and explaining examples line by line)
 
 Code for shared memory Creator side:
 ```python
 ashared_memory_manager: ASharedMemoryManager = ASharedMemoryManager(SharedMemory('shared_memory_identifier', create=True, size=200 * 1024**2))
 # declare creation and initiation of the shared memory instance with a size of 200 MiB.
 ```
```

