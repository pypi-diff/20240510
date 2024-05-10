# Comparing `tmp/zjbbintest-2.1.tar.gz` & `tmp/zjbbintest-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zjbbintest-2.1.tar", last modified: Wed May  8 07:48:46 2024, max compression
+gzip compressed data, was "dist/zjbbintest-2.2.tar", last modified: Thu May  9 13:41:34 2024, max compression
```

## Comparing `zjbbintest-2.1.tar` & `zjbbintest-2.2.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.466534 zjbbintest-2.1/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-08 07:48:46.466314 zjbbintest-2.1/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.1/README.md
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-08 07:48:46.466584 zjbbintest-2.1/setup.cfg
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      727 2024-05-08 07:48:45.000000 zjbbintest-2.1/setup.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.461414 zjbbintest-2.1/zjbbintest/
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.462513 zjbbintest-2.1/zjbbintest/Actuator/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.1/zjbbintest/Actuator/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      746 2024-04-21 08:57:59.000000 zjbbintest-2.1/zjbbintest/Actuator/actuator.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.462854 zjbbintest-2.1/zjbbintest/Actuator/bin_test_case/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.1/zjbbintest/Actuator/bin_test_case/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12749 2024-05-08 07:46:52.000000 zjbbintest-2.1/zjbbintest/Actuator/bin_test_case/bin_test_case.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.463259 zjbbintest-2.1/zjbbintest/Actuator/bin_test_exception/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.1/zjbbintest/Actuator/bin_test_exception/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.1/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.465531 zjbbintest-2.1/zjbbintest/Actuator/utils/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.1/zjbbintest/Actuator/utils/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-08 05:24:56.000000 zjbbintest-2.1/zjbbintest/Actuator/utils/action_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6391 2024-05-08 06:54:18.000000 zjbbintest-2.1/zjbbintest/Actuator/utils/assert_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3733 2024-05-08 06:54:26.000000 zjbbintest-2.1/zjbbintest/Actuator/utils/format_check.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.1/zjbbintest/Actuator/utils/processing_path.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     8016 2024-05-08 06:54:35.000000 zjbbintest-2.1/zjbbintest/Actuator/utils/requestor.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9046 2024-05-08 06:54:04.000000 zjbbintest-2.1/zjbbintest/Actuator/utils/string_dynamic_run.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.466120 zjbbintest-2.1/zjbbintest/Template/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.1/zjbbintest/Template/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1261 2024-05-07 09:04:47.000000 zjbbintest-2.1/zjbbintest/Template/bintest_template.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.1/zjbbintest/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9912 2024-05-08 06:57:05.000000 zjbbintest-2.1/zjbbintest/bintest.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.1/zjbbintest/bintest_data.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:48:46.462266 zjbbintest-2.1/zjbbintest.egg-info/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-08 07:48:46.000000 zjbbintest-2.1/zjbbintest.egg-info/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      908 2024-05-08 07:48:46.000000 zjbbintest-2.1/zjbbintest.egg-info/SOURCES.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-08 07:48:46.000000 zjbbintest-2.1/zjbbintest.egg-info/dependency_links.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      293 2024-05-08 07:48:46.000000 zjbbintest-2.1/zjbbintest.egg-info/requires.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-08 07:48:46.000000 zjbbintest-2.1/zjbbintest.egg-info/top_level.txt
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.335166 zjbbintest-2.2/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-09 13:41:34.334998 zjbbintest-2.2/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.2/README.md
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-09 13:41:34.335227 zjbbintest-2.2/setup.cfg
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      639 2024-05-09 13:41:23.000000 zjbbintest-2.2/setup.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.330587 zjbbintest-2.2/zjbbintest/
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.331566 zjbbintest-2.2/zjbbintest/Actuator/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.2/zjbbintest/Actuator/__init__.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.331780 zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    13185 2024-05-08 13:22:57.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/bin_test_case.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.332209 zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.333804 zjbbintest-2.2/zjbbintest/Actuator/utils/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-08 05:24:56.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/action_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6668 2024-05-08 10:50:18.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/assert_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3733 2024-05-08 06:54:26.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/format_check.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/processing_path.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     8016 2024-05-08 06:54:35.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/requestor.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    10872 2024-05-09 13:31:22.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/string_dynamic_run.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.334249 zjbbintest-2.2/zjbbintest/Analysis/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 14:37:18.000000 zjbbintest-2.2/zjbbintest/Analysis/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     2596 2024-05-09 12:16:14.000000 zjbbintest-2.2/zjbbintest/Analysis/har2json.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      877 2024-05-09 12:22:22.000000 zjbbintest-2.2/zjbbintest/Analysis/replace_values.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.334583 zjbbintest-2.2/zjbbintest/Template/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.2/zjbbintest/Template/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1261 2024-05-07 09:04:47.000000 zjbbintest-2.2/zjbbintest/Template/bintest_template.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1172 2024-05-07 09:08:55.000000 zjbbintest-2.2/zjbbintest/Template/report_template.html
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.2/zjbbintest/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 02:26:46.000000 zjbbintest-2.2/zjbbintest/analysis.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9805 2024-05-08 12:19:43.000000 zjbbintest-2.2/zjbbintest/bintest.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.2/zjbbintest/bintest_data.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.331439 zjbbintest-2.2/zjbbintest.egg-info/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1042 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      720 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/requires.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/top_level.txt
```

### Comparing `zjbbintest-2.1/README.md` & `zjbbintest-2.2/README.md`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/bin_test_case/bin_test_case.py` & `zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/bin_test_case.py`

 * *Files 11% similar despite different names*

```diff
@@ -116,79 +116,88 @@
         # 初始化case_var_dict
         self.case_var_dict = {}
         # 请求和响应的list
         self.req_list = []
         self.resp_list = []
         case_step_run_res = {}
         # print(self.case_steps)
+        exception_flag = False
+        # 执行case步骤
         try:
             for case_step in self.case_steps:
                 # TODO 执行case步骤的时候，需要把case_var_dict传进去，也需要请求和响应的list，这里需要补充一下
                 # DONE 2024-05-05
                 run_res, self.case_var_dict, self.req_list, self.resp_list = case_step.run(self.case_var_dict,
-                                                                                           self.req_list, self.resp_list)
+                                                                                           self.req_list,
+                                                                                           self.resp_list)
                 case_step_run_res[case_step.step_id] = run_res
 
         except (bt_exception.AssertFailException, AssertionError) as e:
             self.case_run_status = CaseRunStatus.FAIL
             self.case_run_msg = str(e.message)
+            exception_flag = True
         except bt_exception.RequestException as e:
             self.case_run_status = CaseRunStatus.REQUEST_EXCEPTION
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.FormatCheckException as e:
             self.case_run_status = CaseRunStatus.BT_STRING_FORMAT_ERROR
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.BTFuncNotFoundException as e:
             self.case_run_status = CaseRunStatus.BT_FUNC_NOT_FOUND
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.BTActionNotFoundException as e:
             self.case_run_status = CaseRunStatus.BT_ACTION_NOT_FOUND
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.BTAssertNotFoundException as e:
             self.case_run_status = CaseRunStatus.BT_ASSERT_NOT_FOUND
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.BTFuncFormatCheckException as e:
             self.case_run_status = CaseRunStatus.BT_FUNC_FORMAT_CHECK_ERROR
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.BTActionFormatCheckException as e:
             self.case_run_status = CaseRunStatus.BT_ACTION_FORMAT_CHECK_ERROR
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.BTAssertFormatCheckException as e:
             self.case_run_status = CaseRunStatus.BT_ASSERT_FORMAT_CHECK_ERROR
             self.case_run_msg = str(e.message)
-            return
+            exception_flag = True
         except bt_exception.BTAssertDictFormatException as e:
             self.case_run_status = CaseRunStatus.ASSERT_DICT_FORMAT_ERROR
             self.case_run_msg = str(e.message)
+            exception_flag = True
         except Exception as e:
+            exception_flag = True
             logging.exception(e)
             self.case_run_status = CaseRunStatus.OTHER_EXCEPTION
             self.case_run_msg = str(e)
-        if len(case_step_run_res.items()) == len(self.case_steps) and all(case_step_run_res.values()):
+        if exception_flag == False \
+                and len(case_step_run_res.items()) == len(self.case_steps) \
+                and all(case_step_run_res.values()):
             self.case_run_status = CaseRunStatus.PASS
             self.case_run_msg = "执行成功"
         else:
             self.case_run_status = CaseRunStatus.FAIL
             self.case_run_msg = "执行失败"
         return {
             "case_name": self.case_name,
             "case_desc": self.case_desc,
             "priority": self.priority,
             "mark": self.case_mack_labels,
             "run_status": self.case_run_status,
             "run_msg": self.case_run_msg
         }
 
+
 class CaseStep:
     """
     case单个步骤对象
     case单个步骤的内容有几部分
     1.请求:dict
     2.动作:list
     3.断言:list
```

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py` & `zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/utils/action_execution.py` & `zjbbintest-2.2/zjbbintest/Actuator/utils/action_execution.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/utils/assert_execution.py` & `zjbbintest-2.2/zjbbintest/Actuator/utils/assert_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,48 +35,51 @@
         self.assert_name = assert_name
 
     def execute(self):
         """
         执行单个断言
         :return:
         """
-        if self.assert_name in AssertDict.EQUALS:
-            assert self.expect_data == self.actual_data, f"进行'{self.assert_name}'断言失败" \
-                                                         f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        elif self.assert_name in AssertDict.NOT_EQUALS:
-            assert self.expect_data != self.actual_data, f"进行'{self.assert_name}'断言失败" \
-                                                         f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        elif self.assert_name in AssertDict.GREATER:
-            assert self.expect_data > self.actual_data, f"进行'{self.assert_name}'断言失败" \
-                                                        f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        elif self.assert_name in AssertDict.LESS:
-            assert self.expect_data < self.actual_data, f"进行'{self.assert_name}'断言失败" \
-                                                        f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        elif self.assert_name in AssertDict.GREATER_EQUALS:
-            assert self.expect_data >= self.actual_data, f"进行'{self.assert_name}'断言失败" \
-                                                         f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        elif self.assert_name in AssertDict.LESS_EQUALS:
-            assert self.expect_data <= self.actual_data, f"进行'{self.assert_name}'断言失败" \
-                                                         f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        elif self.assert_name in AssertDict.IN:
-            assert self.expect_data in self.actual_data, f"进行'{self.assert_name}'断言失败" \
-                                                         f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        elif self.assert_name in AssertDict.NOT_IN:
-            assert self.expect_data not in self.actual_data, f"进行'{self.assert_name}'断言失败" \
+        try:
+            if self.assert_name in AssertDict.EQUALS:
+                assert self.expect_data == self.actual_data, f"进行'{self.assert_name}'断言失败" \
                                                              f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
-        else:
-            try:
-                assert_res = BinTestData.assert_dict.get(self.assert_name)(self.expect_data, self.actual_data)
-                if not assert_res:
-                    raise AssertFailException(self.expect_data, self.actual_data, self.assert_name)
-                else:
-                    return assert_res
-            except TypeError as e:
-                raise BTAssertNotFoundException(self.assert_name)
-        return True
+            elif self.assert_name in AssertDict.NOT_EQUALS:
+                assert self.expect_data != self.actual_data, f"进行'{self.assert_name}'断言失败" \
+                                                             f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
+            elif self.assert_name in AssertDict.GREATER:
+                assert self.expect_data > self.actual_data, f"进行'{self.assert_name}'断言失败" \
+                                                            f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
+            elif self.assert_name in AssertDict.LESS:
+                assert self.expect_data < self.actual_data, f"进行'{self.assert_name}'断言失败" \
+                                                            f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
+            elif self.assert_name in AssertDict.GREATER_EQUALS:
+                assert self.expect_data >= self.actual_data, f"进行'{self.assert_name}'断言失败" \
+                                                             f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
+            elif self.assert_name in AssertDict.LESS_EQUALS:
+                assert self.expect_data <= self.actual_data, f"进行'{self.assert_name}'断言失败" \
+                                                             f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
+            elif self.assert_name in AssertDict.IN:
+                assert self.expect_data in self.actual_data, f"进行'{self.assert_name}'断言失败" \
+                                                             f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
+            elif self.assert_name in AssertDict.NOT_IN:
+                assert self.expect_data not in self.actual_data, f"进行'{self.assert_name}'断言失败" \
+                                                                 f"，期望值：{self.expect_data}，实际值：{self.actual_data}"
+            else:
+                try:
+                    assert_res = BinTestData.assert_dict.get(self.assert_name)(self.expect_data, self.actual_data)
+                    if not assert_res:
+                        raise AssertFailException(self.expect_data, self.actual_data, self.assert_name)
+                    else:
+                        return assert_res
+                except TypeError as e:
+                    raise BTAssertNotFoundException(self.assert_name)
+            return True
+        except AssertionError as e:
+            raise AssertFailException(self.expect_data, self.actual_data, self.assert_name)
 
     def __str__(self):
         """
         :return:
         """
         return f"expect: {self.expect_data}, actual: {self.actual_data}, assert: {self.assert_name}"
```

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/utils/format_check.py` & `zjbbintest-2.2/zjbbintest/Actuator/utils/format_check.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/utils/processing_path.py` & `zjbbintest-2.2/zjbbintest/Actuator/utils/processing_path.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/utils/requestor.py` & `zjbbintest-2.2/zjbbintest/Actuator/utils/requestor.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.1/zjbbintest/Actuator/utils/string_dynamic_run.py` & `zjbbintest-2.2/zjbbintest/Actuator/utils/string_dynamic_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 Authors: zhangjiabin01
 Date: 2024/4/12 19:18:00
 """
 import itertools
 
 from zjbbintest.Actuator.bin_test_exception.bin_test_exception import FormatBTStringException, BTFuncNotFoundException, BTActionNotFoundException
 from zjbbintest.bintest_data import BinTestData
+from jsonpath_rw import parse
+import logging
+
+
 
 
 class StringDynamicRun:
     """
     字符串动态执行方法
     主要处理$BT[]中的conf()、func()和var()，通过run方法将字符串变为单纯的纯文本字符串
     """
@@ -135,87 +139,119 @@
         """
         self.case_var_dict = case_var_dict
         self.req_list = req_list
         self.resp_list = resp_list
 
     def run(self, operable_str):
         """
-        传入可以执行的字符串如conf()、func()、var()、set()，执行具体动作，返回执行后的字符串和case级变量字典
+        传入可以执行的字符串如func()、var()、set()，执行具体动作，返回执行后的字符串和case级变量字典
         :param operable_str:
         :return:
         """
+        logging.debug(f'动态执行字符串：{operable_str}')
         if operable_str is None or operable_str == '':
             return ''
         operable_str = operable_str.strip()
-        if operable_str.startswith("conf(") and operable_str.endswith(")"):
-            new_str = operable_str[5:-1]
-            value_str = self.run(new_str)
-            value_path = value_str.split('.')
-            res_str = BinTestData.config_dict
-            for value_path_item in value_path:
-                res_str = res_str.get(value_path_item)
-            return res_str
-        elif operable_str.startswith("func(") and operable_str.endswith(")"):
+        # if operable_str.startswith("conf(") and operable_str.endswith(")"):
+        #     new_str = operable_str[5:-1]
+        #
+        #     value_str = self.run(new_str)
+        #     value_path = value_str.split('.')
+        #     res_str = BinTestData.config_dict
+        #     for value_path_item in value_path:
+        #         res_str = res_str.get(value_path_item)
+        #     return res_str
+        if operable_str.startswith("func(") and operable_str.endswith(")"):
             new_str = operable_str[5:-1]
             value_str = self.run(new_str)
             func_name = value_str.split('(')[0]
             func_args = value_str[len(func_name) + 1: len(value_str) - 1].split(',')
             func_args = [self.run(arg) for arg in func_args]
             try:
                 if func_args is None or func_args == [] or func_args == [""]:
+                    logging.debug(f'执行无参方法{func_name}')
                     res_str = BinTestData.func_dict.get(func_name)()
                 else:
+                    logging.debug(f'执行有参方法{func_name}，参数为:{func_args}')
                     res_str = BinTestData.func_dict.get(func_name)(*func_args)
             except TypeError:
                 raise BTFuncNotFoundException(func_name)
             return res_str
         elif operable_str.startswith("var(") and operable_str.endswith(")"):
+            # TODO 换成jsonpath的方式获取变量
+            # DONE 2024-5-9
             new_str = operable_str[4:-1]
             value_str = self.run(new_str)
             value_path = value_str.split('.')
             if len(value_path) == 0:
                 return None
             if value_path[0] == "$var":
                 # 获取用户自定义变量
                 data_source = self.case_var_dict
+                json_path = '$' + value_str[4:]
+                logging.debug(f'从变量中获取内容，jsonpath为:{json_path}；变量字典为:{data_source}')
             elif value_path[0] == "$req":
                 # 获取请求响应变量
                 data_source = self.req_list
+                json_path = '$' + value_str[4:]
+                logging.debug(f'从请求中获取内容，jsonpath为:{json_path}；请求字典为:{data_source}')
             elif value_path[0] == "$resp":
                 # 获取请求响应变量
                 data_source = self.resp_list
+                json_path = '$' + value_str[5:]
+                logging.debug(f'从响应中获取内容，jsonpath为:{json_path}；响应字典为:{data_source}')
+            elif value_path[0] == "$conf":
+                # 获取配置文件变量
+                data_source = BinTestData.config_dict
+                json_path = '$' + value_str[5:]
+                logging.debug(f'从配置文件中获取内容，jsonpath为:{json_path}；配置字典为:{data_source}')
             else:
                 return None
-            for value_path_item in value_path[1:]:
-                if value_path_item.isdigit():
-                    try:
-                        data_source = data_source[int(value_path_item)]
-                    except IndexError:
-                        return None
+            expr = parse(json_path)
+            result = expr.find(data_source)
+            if result:
+                res_list = []
+                for match in result:
+                    res_list.append(match.value)
+                if len(res_list) == 1:
+                    return res_list[0]
                 else:
-                    data_source = data_source.get(value_path_item)
-            return data_source
+                    return res_list
+            else:
+                return None
+            # for value_path_item in value_path[1:]:
+            #     if value_path_item.isdigit():
+            #         try:
+            #             data_source = data_source[int(value_path_item)]
+            #         except IndexError:
+            #             return None
+            #     else:
+            #         data_source = data_source.get(value_path_item)
+            # return data_source
         elif operable_str.startswith("set(") and operable_str.endswith(")"):
             new_str = operable_str[4:-1]
             # 获取变量名和值
             index = new_str.find(',')
             var_key = new_str[:index]
             var_value = new_str[index + 1:]
             var_value = self.run(var_value)
             self.case_var_dict[var_key] = var_value
+            logging.debug(f'设置变量{var_key}为{var_value}')
             return ''
         elif operable_str.startswith("action(") and operable_str.endswith(")"):
             new_str = operable_str[7:-1]
             value_str = self.run(new_str)
             action_name = value_str.split('(')[0]
             action_args = value_str[len(action_name) + 1: len(value_str) - 1].split(',')
             action_args = [self.run(arg) for arg in action_args]
             try:
                 if action_args is None or action_args == [] or action_args == [""]:
+                    logging.debug(f'执行无参动作{action_name}')
                     BinTestData.action_dict.get(action_name)()
                 else:
+                    logging.debug(f'执行有参动作{action_name}，参数为{action_args}')
                     BinTestData.action_dict.get(action_name)(*action_args)
             except TypeError as e:
                 raise BTActionNotFoundException(action_name)
             return ''
         else:
             return operable_str
```

### Comparing `zjbbintest-2.1/zjbbintest/Template/bintest_template.py` & `zjbbintest-2.2/zjbbintest/Template/bintest_template.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.1/zjbbintest/bintest.py` & `zjbbintest-2.2/zjbbintest/bintest.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,21 +238,20 @@
     now_time = datetime.now()
     # 初始化日志
     if not os.path.exists(log_path):
         # 创建文件所在的目录
         dir_path = os.path.dirname(log_path)
         if not os.path.exists(dir_path):
             os.makedirs(dir_path)
-            print(f"目录 {dir_path} 已创建。")
         # 创建文件
         with open(log_path, 'w') as f:
             pass
         print(f"文件 {log_path} 已创建。")
     else:
-        print(f"文件 {log_path} 已存在，不进行创建。")
+        pass
     logging.basicConfig(filename=log_path, filemode='a', level=logging.DEBUG,
                         format='%(asctime)s - %(pathname)s - %(lineno)s - %(message)s')
     case_res_list = []
     if BinTestData.case_load_flag:
         # 执行测试用例
         for bin_case in BinTestData.run_case_list:
             case_res = bin_case.run()
```

### Comparing `zjbbintest-2.1/zjbbintest.egg-info/SOURCES.txt` & `zjbbintest-2.2/zjbbintest.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 README.md
 setup.py
 zjbbintest/__init__.py
+zjbbintest/analysis.py
 zjbbintest/bintest.py
 zjbbintest/bintest_data.py
 zjbbintest.egg-info/PKG-INFO
 zjbbintest.egg-info/SOURCES.txt
 zjbbintest.egg-info/dependency_links.txt
 zjbbintest.egg-info/requires.txt
 zjbbintest.egg-info/top_level.txt
 zjbbintest/Actuator/__init__.py
-zjbbintest/Actuator/actuator.py
 zjbbintest/Actuator/bin_test_case/__init__.py
 zjbbintest/Actuator/bin_test_case/bin_test_case.py
 zjbbintest/Actuator/bin_test_exception/__init__.py
 zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
 zjbbintest/Actuator/utils/__init__.py
 zjbbintest/Actuator/utils/action_execution.py
 zjbbintest/Actuator/utils/assert_execution.py
 zjbbintest/Actuator/utils/format_check.py
 zjbbintest/Actuator/utils/processing_path.py
 zjbbintest/Actuator/utils/requestor.py
 zjbbintest/Actuator/utils/string_dynamic_run.py
+zjbbintest/Analysis/__init__.py
+zjbbintest/Analysis/har2json.py
+zjbbintest/Analysis/replace_values.py
 zjbbintest/Template/__init__.py
-zjbbintest/Template/bintest_template.py
+zjbbintest/Template/bintest_template.py
+zjbbintest/Template/report_template.html
```

