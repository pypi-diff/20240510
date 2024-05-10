# Comparing `tmp/zjbbintest-2.2.tar.gz` & `tmp/zjbbintest-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zjbbintest-2.2.tar", last modified: Thu May  9 13:41:34 2024, max compression
+gzip compressed data, was "dist/zjbbintest-2.3.tar", last modified: Fri May 10 11:42:07 2024, max compression
```

## Comparing `zjbbintest-2.2.tar` & `zjbbintest-2.3.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.335166 zjbbintest-2.2/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-09 13:41:34.334998 zjbbintest-2.2/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.2/README.md
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-09 13:41:34.335227 zjbbintest-2.2/setup.cfg
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      639 2024-05-09 13:41:23.000000 zjbbintest-2.2/setup.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.330587 zjbbintest-2.2/zjbbintest/
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.331566 zjbbintest-2.2/zjbbintest/Actuator/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.2/zjbbintest/Actuator/__init__.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.331780 zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    13185 2024-05-08 13:22:57.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/bin_test_case.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.332209 zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.333804 zjbbintest-2.2/zjbbintest/Actuator/utils/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-08 05:24:56.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/action_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6668 2024-05-08 10:50:18.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/assert_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3733 2024-05-08 06:54:26.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/format_check.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/processing_path.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     8016 2024-05-08 06:54:35.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/requestor.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    10872 2024-05-09 13:31:22.000000 zjbbintest-2.2/zjbbintest/Actuator/utils/string_dynamic_run.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.334249 zjbbintest-2.2/zjbbintest/Analysis/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 14:37:18.000000 zjbbintest-2.2/zjbbintest/Analysis/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     2596 2024-05-09 12:16:14.000000 zjbbintest-2.2/zjbbintest/Analysis/har2json.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      877 2024-05-09 12:22:22.000000 zjbbintest-2.2/zjbbintest/Analysis/replace_values.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.334583 zjbbintest-2.2/zjbbintest/Template/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.2/zjbbintest/Template/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1261 2024-05-07 09:04:47.000000 zjbbintest-2.2/zjbbintest/Template/bintest_template.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1172 2024-05-07 09:08:55.000000 zjbbintest-2.2/zjbbintest/Template/report_template.html
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.2/zjbbintest/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 02:26:46.000000 zjbbintest-2.2/zjbbintest/analysis.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9805 2024-05-08 12:19:43.000000 zjbbintest-2.2/zjbbintest/bintest.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.2/zjbbintest/bintest_data.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-09 13:41:34.331439 zjbbintest-2.2/zjbbintest.egg-info/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1042 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/SOURCES.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/dependency_links.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      720 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/requires.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-09 13:41:34.000000 zjbbintest-2.2/zjbbintest.egg-info/top_level.txt
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.546898 zjbbintest-2.3/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-10 11:42:07.546751 zjbbintest-2.3/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.3/README.md
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-10 11:42:07.546938 zjbbintest-2.3/setup.cfg
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      603 2024-05-10 11:41:56.000000 zjbbintest-2.3/setup.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.541760 zjbbintest-2.3/zjbbintest/
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.542825 zjbbintest-2.3/zjbbintest/Actuator/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.3/zjbbintest/Actuator/__init__.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.543067 zjbbintest-2.3/zjbbintest/Actuator/bin_test_case/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.3/zjbbintest/Actuator/bin_test_case/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    13665 2024-05-10 09:44:52.000000 zjbbintest-2.3/zjbbintest/Actuator/bin_test_case/bin_test_case.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.543609 zjbbintest-2.3/zjbbintest/Actuator/bin_test_exception/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.3/zjbbintest/Actuator/bin_test_exception/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.3/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.545442 zjbbintest-2.3/zjbbintest/Actuator/utils/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.3/zjbbintest/Actuator/utils/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-10 09:44:52.000000 zjbbintest-2.3/zjbbintest/Actuator/utils/action_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6643 2024-05-10 09:44:52.000000 zjbbintest-2.3/zjbbintest/Actuator/utils/assert_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3733 2024-05-08 06:54:26.000000 zjbbintest-2.3/zjbbintest/Actuator/utils/format_check.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.3/zjbbintest/Actuator/utils/processing_path.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     7608 2024-05-10 09:44:52.000000 zjbbintest-2.3/zjbbintest/Actuator/utils/requestor.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12193 2024-05-10 09:44:52.000000 zjbbintest-2.3/zjbbintest/Actuator/utils/string_dynamic_run.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.545910 zjbbintest-2.3/zjbbintest/Analysis/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 14:37:18.000000 zjbbintest-2.3/zjbbintest/Analysis/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     2596 2024-05-09 12:16:14.000000 zjbbintest-2.3/zjbbintest/Analysis/har2json.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3188 2024-05-10 11:05:40.000000 zjbbintest-2.3/zjbbintest/Analysis/replace_values.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.546460 zjbbintest-2.3/zjbbintest/Template/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.3/zjbbintest/Template/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1255 2024-05-10 08:40:52.000000 zjbbintest-2.3/zjbbintest/Template/bintest_template.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1172 2024-05-07 09:08:55.000000 zjbbintest-2.3/zjbbintest/Template/report_template.html
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.3/zjbbintest/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9805 2024-05-08 12:19:43.000000 zjbbintest-2.3/zjbbintest/bintest.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.3/zjbbintest/bintest_data.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:42:07.542708 zjbbintest-2.3/zjbbintest.egg-info/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-10 11:42:07.000000 zjbbintest-2.3/zjbbintest.egg-info/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1019 2024-05-10 11:42:07.000000 zjbbintest-2.3/zjbbintest.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-10 11:42:07.000000 zjbbintest-2.3/zjbbintest.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      720 2024-05-10 11:42:07.000000 zjbbintest-2.3/zjbbintest.egg-info/requires.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-10 11:42:07.000000 zjbbintest-2.3/zjbbintest.egg-info/top_level.txt
```

### Comparing `zjbbintest-2.2/README.md` & `zjbbintest-2.3/README.md`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.2/setup.py` & `zjbbintest-2.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 dependencies = []
 
 # 打开requirements.txt文件并读取内容
 with open('requirements.txt', 'r') as file:
     for line in file:
-        # 去除行尾的换行符并添加到列表中
         dependencies.append(line.strip())
 
+print(dependencies)
 
 setup(
     name='zjbbintest',
-    version='2.2',
+    version='2.3',
     author="zhangjiabin01",
     author_email="zhangjiabin01@baidu.com",
     description="bintest自动化框架",
     packages=find_packages(),
     package_data={
             'zjbbintest': ['Template/*'],  # 包含my_package中的templates文件夹下的所有文件
         },
```

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/bin_test_case/bin_test_case.py` & `zjbbintest-2.3/zjbbintest/Actuator/bin_test_case/bin_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,26 +60,26 @@
     2.case_desc: case详情
     3.case_steps: case执行步骤，主要逻辑都在里面
     4.case_var_dict: case执行过程中记录的变量
     """
 
     def __init__(self, case_name="", case_desc="", priority="", case_mack_labels=[], case_steps=[],
                  case_run_status=CaseRunStatus.NOT_RUNNING, case_run_msg="未执行",
-                 case_var_dict={}, req_list=[], resp_list=[]):
+                 case_var_dict={}, req_dict=[], resp_dict=[]):
         self.case_name = case_name
         self.case_desc = case_desc
         self.priority = priority
         self.case_mack_labels = case_mack_labels
         self.case_steps = case_steps
         # 下面四个是在创建之初没有的，在执行过程中会添加进去
         self.case_run_status = case_run_status
         self.case_run_msg = case_run_msg
         self.case_var_dict = case_var_dict
-        self.req_list = req_list
-        self.resp_list = resp_list
+        self.req_dict = req_dict
+        self.resp_dict = resp_dict
 
     @staticmethod
     def create_obj_by_dict(case_space_dict):
         """
         根据字典创建caseSpace对象
         :param case_space_dict:
         :return:
@@ -104,35 +104,41 @@
                            case_mack_labels=case_mack_labels, case_steps=case_step_list)
 
     def run(self):
         """
         执行case
         :return:
         """
+        logging.debug(f"开始执行case: {self.case_name}")
         # 判断case是否可以执行
         if self.case_run_status != CaseRunStatus.NOT_RUNNING:
             logging.info(f"case: {self.case_name} 已经执行过了，不能重复执行")
             # 不是未执行状态，说明执行过（有问题），不能重复执行
             return
         # 初始化case_var_dict
         self.case_var_dict = {}
         # 请求和响应的list
         self.req_list = []
         self.resp_list = []
         case_step_run_res = {}
         # print(self.case_steps)
         exception_flag = False
         # 执行case步骤
+        logging.debug(f"------------------开始执行case步骤-----------------------")
         try:
             for case_step in self.case_steps:
                 # TODO 执行case步骤的时候，需要把case_var_dict传进去，也需要请求和响应的list，这里需要补充一下
                 # DONE 2024-05-05
-                run_res, self.case_var_dict, self.req_list, self.resp_list = case_step.run(self.case_var_dict,
-                                                                                           self.req_list,
-                                                                                           self.resp_list)
+                run_res, self.case_var_dict, self.req_dict, self.resp_dict = case_step.run(self.case_var_dict,
+                                                                                           self.req_dict,
+                                                                                           self.resp_dict)
+                logging.debug(f"case_step: {case_step.step_id} 执行结果为：{run_res}")
+                logging.debug(f"case_var_dict: {self.case_var_dict}")
+                logging.debug(f"req_list: {self.req_dict}")
+                logging.debug(f"resp_list: {self.resp_dict}")
                 case_step_run_res[case_step.step_id] = run_res
 
         except (bt_exception.AssertFailException, AssertionError) as e:
             self.case_run_status = CaseRunStatus.FAIL
             self.case_run_msg = str(e.message)
             exception_flag = True
         except bt_exception.RequestException as e:
@@ -172,28 +178,28 @@
             self.case_run_msg = str(e.message)
             exception_flag = True
         except Exception as e:
             exception_flag = True
             logging.exception(e)
             self.case_run_status = CaseRunStatus.OTHER_EXCEPTION
             self.case_run_msg = str(e)
-        if exception_flag == False \
-                and len(case_step_run_res.items()) == len(self.case_steps) \
-                and all(case_step_run_res.values()):
-            self.case_run_status = CaseRunStatus.PASS
-            self.case_run_msg = "执行成功"
-        else:
-            self.case_run_status = CaseRunStatus.FAIL
-            self.case_run_msg = "执行失败"
+        if not exception_flag:
+            if len(case_step_run_res.items()) == len(self.case_steps) \
+                    and all(case_step_run_res.values()):
+                self.case_run_status = CaseRunStatus.PASS
+                self.case_run_msg = "执行成功"
+            else:
+                self.case_run_status = CaseRunStatus.FAIL
+                self.case_run_msg = "执行失败"
         return {
             "case_name": self.case_name,
             "case_desc": self.case_desc,
             "priority": self.priority,
             "mark": self.case_mack_labels,
-            "run_status": self.case_run_status,
+            "run_status": self.case_run_status.value,
             "run_msg": self.case_run_msg
         }
 
 
 class CaseStep:
     """
     case单个步骤对象
@@ -234,31 +240,31 @@
         request_obj = RequestObject.create_obj_by_dict(request_dict)
         actions = case_step_dict.get("action")
         action_list = BatchActionExecutor(actions)
         asserts = case_step_dict.get("assert")
         assert_list = BatchAssertExecutor(asserts)
         return CaseStep(step_id, request_obj, action_list, assert_list)
 
-    def run(self, case_var_dict, req_list, resp_list):
+    def run(self, case_var_dict, req_dict, resp_dict):
         """
         执行case步骤
         :return:
         """
         # 请求
-        bt_resp = self.request_obj.send(case_var_dict, req_list, resp_list)
+        bt_resp = self.request_obj.send(case_var_dict, req_dict, resp_dict)
         # 此时，self.request_obj已经完成了其中变量的替换，可以使用obj_to_dict()将其转为字典
-        req_list.append(self.request_obj.obj_to_dict())
-        resp_list.append(bt_resp.obj_to_dict())
+        req_dict[str(self.step_id)] = self.request_obj.obj_to_dict()
+        req_dict[str(self.step_id)] = bt_resp.obj_to_dict()
         # 动作
-        case_var_dict = self.action_list.execute(case_var_dict, req_list, resp_list)
+        case_var_dict = self.action_list.execute(case_var_dict, req_dict, resp_dict)
         # 断言
         # TODO 断言的执行也需要case_var_dict, req_list, resp_list
         # DONE 2024-05-05
-        step_run_res = self.assert_list.execute(case_var_dict, req_list, resp_list)
-        return step_run_res, case_var_dict, req_list, resp_list
+        step_run_res = self.assert_list.execute(case_var_dict, req_dict, resp_dict)
+        return step_run_res, case_var_dict, req_dict, resp_dict
 
 
 if __name__ == '__main__':
     # request = RequestObject("https://aiob-open.baidu.com", "/aiob-server/api/v2/getToken", "POST",
     #                         {'Content-Type': 'application/json'}, {}, {
     #                             "accessKey": "dfc272b758fb451cb5d409d6bf04b40e",
     #                             "secretKey": "561f119cea874a37a81a1e83c9e1b92d"
```

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py` & `zjbbintest-2.3/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/utils/action_execution.py` & `zjbbintest-2.3/zjbbintest/Actuator/utils/action_execution.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,17 +19,17 @@
         Init batch action executor.
         初始化批量动作执行器
         :param action_list: 动作列表
         :type action_list: list
         """
         self.__action_list = action_list
 
-    def execute(self, case_var_dict, req_list, resp_list):
+    def execute(self, case_var_dict, req_dict, resp_dict):
         """
         Execute batch action.
         执行批量动作
         :return: 返回结果
         :rtype: list
         """
         for action in self.__action_list:
-            _, case_var_dict = StringDynamicRun(action, case_var_dict, req_list, resp_list).run()
+            _, case_var_dict = StringDynamicRun(action, case_var_dict, req_dict, resp_dict).run()
         return case_var_dict
```

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/utils/assert_execution.py` & `zjbbintest-2.3/zjbbintest/Actuator/utils/assert_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,25 +79,24 @@
 
     def __str__(self):
         """
         :return:
         """
         return f"expect: {self.expect_data}, actual: {self.actual_data}, assert: {self.assert_name}"
 
-    def replace(self, case_var_dict, req_list, resp_list):
+    def replace(self, case_var_dict, req_dict, resp_dict):
         """
         替换断言中的变量
-        :param obj_dict:
         :param case_var_dict:
-        :param req_list:
-        :param resp_list:
+        :param req_dict:
+        :param resp_dict:
         :return:
         """
-        self.expect_data, _ = StringDynamicRun(self.expect_data, case_var_dict, req_list, resp_list).run()
-        self.actual_data, _ = StringDynamicRun(self.actual_data, case_var_dict, req_list, resp_list).run()
+        self.expect_data, _ = StringDynamicRun(self.expect_data, case_var_dict, req_dict, resp_dict).run()
+        self.actual_data, _ = StringDynamicRun(self.actual_data, case_var_dict, req_dict, resp_dict).run()
         if self.expect_data is None:
             raise BTAssertDictFormatException(self, "expect")
         if self.assert_name is None:
             raise BTAssertDictFormatException(self, "operator")
         if self.actual_data is None:
             raise BTAssertDictFormatException(self, "actual")
 
@@ -125,23 +124,23 @@
     批量断言执行器
     处理一个测试用例中一个步骤里的多条断言
     """
 
     def __init__(self, assert_list):
         self.__assert_list = assert_list
 
-    def execute(self, case_var_dict, req_list, resp_list):
+    def execute(self, case_var_dict, req_dict, resp_dict):
         """
         批量执行断言
         :return:
         """
         execute_res_list = []
         for assert_dict in self.__assert_list:
             # 1.创建单个断言执行对象
             assert_executor = AssertExecutor.create_obj_by_dict(assert_dict)
             # 2.替换变量
-            assert_executor.replace(case_var_dict, req_list, resp_list)
+            assert_executor.replace(case_var_dict, req_dict, resp_dict)
             # 3.执行
             assert_res = assert_executor.execute()
             # 4.内容存放
             execute_res_list.append(assert_res)
         return all(execute_res_list)
```

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/utils/format_check.py` & `zjbbintest-2.3/zjbbintest/Actuator/utils/format_check.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/utils/processing_path.py` & `zjbbintest-2.3/zjbbintest/Actuator/utils/processing_path.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/utils/requestor.py` & `zjbbintest-2.3/zjbbintest/Actuator/utils/requestor.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,63 +37,63 @@
         path = request_dict.get("path")
         method = request_dict.get("method")
         headers = convert_to_str(request_dict.get("headers"))
         params = convert_to_str(request_dict.get("params"))
         body = request_dict.get("body")
         return RequestObject(url, path, method, headers, params, body)
 
-    def replace(self, case_var_dict, req_list, resp_list):
+    def replace(self, case_var_dict, req_dict, resp_dict):
         """
         替换url、path、headers、params、body中的动态变量
         :return: dict
         """
         # 执行url中的动态变量
-        executed_url, _ = StringDynamicRun(self.url, case_var_dict, req_list, resp_list).run()
+        executed_url, _ = StringDynamicRun(self.url, case_var_dict, req_dict, resp_dict).run()
         headers = self.headers
         # 执行headers中的动态变量
         executed_headers = {}
         for key, value in headers.items():
-            executed_key, _ = StringDynamicRun(key, case_var_dict, req_list, resp_list).run()
-            executed_value, _ = StringDynamicRun(value, case_var_dict, req_list, resp_list).run()
+            executed_key, _ = StringDynamicRun(key, case_var_dict, req_dict, resp_dict).run()
+            executed_value, _ = StringDynamicRun(value, case_var_dict, req_dict, resp_dict).run()
             executed_headers[executed_key] = executed_value
         params = self.params
         # 执行params中的动态变量
         executed_params = {}
         if params:
             for key, value in params.items():
-                executed_key, _ = StringDynamicRun(key, case_var_dict, req_list, resp_list).run()
-                executed_value, _ = StringDynamicRun(value, case_var_dict, req_list, resp_list).run()
+                executed_key, _ = StringDynamicRun(key, case_var_dict, req_dict, resp_dict).run()
+                executed_value, _ = StringDynamicRun(value, case_var_dict, req_dict, resp_dict).run()
                 executed_params[executed_key] = executed_value
         body = self.body
         # 执行body中的动态变量
         executed_body = {}
         if body:
             for key, value in body.items():
                 if isinstance(key, str):
-                    executed_key, _ = StringDynamicRun(key, case_var_dict, req_list, resp_list).run()
+                    executed_key, _ = StringDynamicRun(key, case_var_dict, req_dict, resp_dict).run()
                 else:
                     executed_key = key
                 if isinstance(value, str):
-                    executed_value, _ = StringDynamicRun(value, case_var_dict, req_list, resp_list).run()
+                    executed_value, _ = StringDynamicRun(value, case_var_dict, req_dict, resp_dict).run()
                 else:
                     executed_value = value
                 executed_body[executed_key] = executed_value
         self.url = executed_url
         self.path = self.path
         self.method = self.method
         self.headers = executed_headers
         self.params = executed_params
         self.body = executed_body
 
-    def send(self, case_var_dict, req_list, resp_list):
+    def send(self, case_var_dict, req_dict, resp_dict):
         """
         发送请求，返回响应对象
         :return: ResponseObject
         """
-        self.replace(case_var_dict, req_list, resp_list)
+        self.replace(case_var_dict, req_dict, resp_dict)
         url = urljoin(self.url, self.path)
         try:
             print(f"发起请求，请求信息为:{self}")
             response = requests.request(self.method, url, headers=self.headers,
                                         params=self.params, data=json.dumps(self.body))
         except Exception as e:
             raise RequestException(f"请求{self}失败，失败原因:{e}")
@@ -217,14 +217,8 @@
         发送请求，返回响应对象
         :param request_dict: 请求信息
         :return: ResponseObject
         """
 
 
 if __name__ == '__main__':
-    request = RequestObject("https://aiob-open.baidu.com", "/aiob-server/api/v2/getToken", "POST",
-                            {'Content-Type': 'application/json'}, {}, {
-                                "accessKey": "dfc272b758fb451cb5d409d6bf04b40e",
-                                "secretKey": "561f119cea874a37a81a1e83c9e1b92d"
-                            })
-    res = request.send().obj_to_dict()
-    print(res)
+    pass
```

### Comparing `zjbbintest-2.2/zjbbintest/Actuator/utils/string_dynamic_run.py` & `zjbbintest-2.3/zjbbintest/Actuator/utils/string_dynamic_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,40 +3,39 @@
 This module provide configigure file management service in i18n environment.
 
 Authors: zhangjiabin01
 Date: 2024/4/12 19:18:00
 """
 import itertools
 
-from zjbbintest.Actuator.bin_test_exception.bin_test_exception import FormatBTStringException, BTFuncNotFoundException, BTActionNotFoundException
+from zjbbintest.Actuator.bin_test_exception.bin_test_exception import FormatBTStringException, BTFuncNotFoundException, \
+    BTActionNotFoundException
 from zjbbintest.bintest_data import BinTestData
 from jsonpath_rw import parse
 import logging
 
 
-
-
 class StringDynamicRun:
     """
     字符串动态执行方法
     主要处理$BT[]中的conf()、func()和var()，通过run方法将字符串变为单纯的纯文本字符串
     """
 
-    def __init__(self, source_str, case_var_dict={}, req_list=[], resp_list=[]):
+    def __init__(self, source_str, case_var_dict={}, req_dict={}, resp_dict={}):
         """
         :param source_str: 源字符串
         """
         # 源字符串，类似https://$BT[conf(ip)]:$BT[conf(host)]/$BT[conf(path)]?name=$BT[func(var(rebotId))]
         self.source_str = source_str if source_str else ''
         # case执行过程中的变量都存在这个字典中
         self.case_var_dict = case_var_dict
         # case执行过程中的请求列表
-        self.req_list = req_list
+        self.req_dict = req_dict
         # case执行过程中的响应列表
-        self.resp_list = resp_list
+        self.resp_dict = resp_dict
         # 不可执行字符串list
         self.__inoperable_str_list = []
         # 可执行字符串list
         self.__operable_str_list = []
         # 执行后的字符串list
         self.__operated_str_list = []
         # 最后的结果字符串，我们需要的是这个
@@ -82,15 +81,15 @@
             raise FormatBTStringException(f'字符串"{self.source_str}"格式存在问题，请检查括号[]是否匹配')
 
     def __batch_replace(self):
         """
         批量替换字符串
         :return:
         """
-        str_dynamic_run_tool = StringDynamicRunTool(self.case_var_dict, self.req_list, self.resp_list)
+        str_dynamic_run_tool = StringDynamicRunTool(self.case_var_dict, self.req_dict, self.resp_dict)
         self.__operated_str_list = [str_dynamic_run_tool.run(operable_str)
                                     for operable_str in self.__operable_str_list]
 
     def __restore_str(self):
         """
 
         :return:
@@ -125,25 +124,25 @@
 
 
 class StringDynamicRunTool:
     """
     字符串动态执行工具类
     初始化时需要传入一个
     字典类型case_var_dict，代表该条case的变量
-    list类型req_list，表示该条case的请求信息
-    list类型resp_list，表示该条case的响应信息
+    dict类型req_dict，表示该条case的请求信息
+    dict类型resp_dict，表示该条case的响应信息
     """
 
-    def __init__(self, case_var_dict, req_list, resp_list):
+    def __init__(self, case_var_dict, req_dict, resp_dict):
         """
         :param case_var_dict: case级变量字典
         """
         self.case_var_dict = case_var_dict
-        self.req_list = req_list
-        self.resp_list = resp_list
+        self.req_dict = req_dict
+        self.resp_dict = resp_dict
 
     def run(self, operable_str):
         """
         传入可以执行的字符串如func()、var()、set()，执行具体动作，返回执行后的字符串和case级变量字典
         :param operable_str:
         :return:
         """
@@ -177,39 +176,61 @@
                 raise BTFuncNotFoundException(func_name)
             return res_str
         elif operable_str.startswith("var(") and operable_str.endswith(")"):
             # TODO 换成jsonpath的方式获取变量
             # DONE 2024-5-9
             new_str = operable_str[4:-1]
             value_str = self.run(new_str)
-            value_path = value_str.split('.')
-            if len(value_path) == 0:
-                return None
-            if value_path[0] == "$var":
+            if value_str.startswith("$var"):
                 # 获取用户自定义变量
                 data_source = self.case_var_dict
                 json_path = '$' + value_str[4:]
                 logging.debug(f'从变量中获取内容，jsonpath为:{json_path}；变量字典为:{data_source}')
-            elif value_path[0] == "$req":
+            elif value_str.startswith("$req"):
                 # 获取请求响应变量
-                data_source = self.req_list
+                data_source = self.req_dict
                 json_path = '$' + value_str[4:]
                 logging.debug(f'从请求中获取内容，jsonpath为:{json_path}；请求字典为:{data_source}')
-            elif value_path[0] == "$resp":
+            elif value_str.startswith("$resp"):
                 # 获取请求响应变量
-                data_source = self.resp_list
+                data_source = self.resp_dict
                 json_path = '$' + value_str[5:]
                 logging.debug(f'从响应中获取内容，jsonpath为:{json_path}；响应字典为:{data_source}')
-            elif value_path[0] == "$conf":
+            elif value_str.startswith("$conf"):
                 # 获取配置文件变量
                 data_source = BinTestData.config_dict
                 json_path = '$' + value_str[5:]
                 logging.debug(f'从配置文件中获取内容，jsonpath为:{json_path}；配置字典为:{data_source}')
             else:
                 return None
+            # value_path = value_str.split('.')
+            # if len(value_path) == 0:
+            #     return None
+            # if value_path[0] == "$var":
+            #     # 获取用户自定义变量
+            #     data_source = self.case_var_dict
+            #     json_path = '$' + value_str[4:]
+            #     logging.debug(f'从变量中获取内容，jsonpath为:{json_path}；变量字典为:{data_source}')
+            # elif value_path[0] == "$req":
+            #     # 获取请求响应变量
+            #     data_source = self.req_list
+            #     json_path = '$' + value_str[4:]
+            #     logging.debug(f'从请求中获取内容，jsonpath为:{json_path}；请求字典为:{data_source}')
+            # elif value_path[0] == "$resp":
+            #     # 获取请求响应变量
+            #     data_source = self.resp_list
+            #     json_path = '$' + value_str[5:]
+            #     logging.debug(f'从响应中获取内容，jsonpath为:{json_path}；响应字典为:{data_source}')
+            # elif value_path[0] == "$conf":
+            #     # 获取配置文件变量
+            #     data_source = BinTestData.config_dict
+            #     json_path = '$' + value_str[5:]
+            #     logging.debug(f'从配置文件中获取内容，jsonpath为:{json_path}；配置字典为:{data_source}')
+            # else:
+            #     return None
             expr = parse(json_path)
             result = expr.find(data_source)
             if result:
                 res_list = []
                 for match in result:
                     res_list.append(match.value)
                 if len(res_list) == 1:
```

### Comparing `zjbbintest-2.2/zjbbintest/Analysis/har2json.py` & `zjbbintest-2.3/zjbbintest/Analysis/har2json.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.2/zjbbintest/Template/bintest_template.py` & `zjbbintest-2.3/zjbbintest/Template/bintest_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from jinja2 import Environment, FileSystemLoader
 
 
 def render_report(cases, test_time, report_path):
     # 计算数据
     total_cases = len(cases)
-    passed_cases = len([case for case in cases if case['run_status'].value == 200])
+    passed_cases = len([case for case in cases if case['run_status'] == 200])
 
     path = os.path.dirname(os.path.abspath(__file__))
     # 加载模板文件
     file_loader = FileSystemLoader(path)
     env = Environment(loader=file_loader)
 
     # 选择模板
```

### Comparing `zjbbintest-2.2/zjbbintest/Template/report_template.html` & `zjbbintest-2.3/zjbbintest/Template/report_template.html`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.2/zjbbintest/bintest.py` & `zjbbintest-2.3/zjbbintest/bintest.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.2/zjbbintest.egg-info/SOURCES.txt` & `zjbbintest-2.3/zjbbintest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.py
 zjbbintest/__init__.py
-zjbbintest/analysis.py
 zjbbintest/bintest.py
 zjbbintest/bintest_data.py
 zjbbintest.egg-info/PKG-INFO
 zjbbintest.egg-info/SOURCES.txt
 zjbbintest.egg-info/dependency_links.txt
 zjbbintest.egg-info/requires.txt
 zjbbintest.egg-info/top_level.txt
```

### Comparing `zjbbintest-2.2/zjbbintest.egg-info/requires.txt` & `zjbbintest-2.3/zjbbintest.egg-info/requires.txt`

 * *Files identical despite different names*

