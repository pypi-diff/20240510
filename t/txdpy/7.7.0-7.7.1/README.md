# Comparing `tmp/txdpy-7.7.0.tar.gz` & `tmp/txdpy-7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-onw_7asr\txdpy-7.7.0.tar", last modified: Wed May  8 01:17:17 2024, max compression
+gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-yb2on2wa\txdpy-7.7.1.tar", last modified: Fri May 10 08:33:56 2024, max compression
```

## Comparing `txdpy-7.7.0.tar` & `txdpy-7.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 01:17:17.000000 txdpy-7.7.0/
--rw-rw-rw-   0        0        0       71 2024-05-08 01:17:17.000000 txdpy-7.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 01:17:17.000000 txdpy-7.7.0/setup.cfg
--rw-rw-rw-   0        0        0      378 2024-05-08 01:16:47.000000 txdpy-7.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 01:17:17.000000 txdpy-7.7.0/txdpy/
--rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.7.0/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     2789 2024-05-08 01:15:10.000000 txdpy-7.7.0/txdpy/__init__.py
--rw-rw-rw-   0        0        0    28088 2024-05-07 08:06:01.000000 txdpy-7.7.0/txdpy/bk_179.py
--rw-rw-rw-   0        0        0     3855 2024-04-30 03:54:19.000000 txdpy-7.7.0/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     2403 2024-05-08 01:15:10.000000 txdpy-7.7.0/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.7.0/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.7.0/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.7.0/txdpy/lookup.py
--rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.7.0/txdpy/progress_display.py
--rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.7.0/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0    11855 2024-04-07 07:33:20.000000 txdpy-7.7.0/txdpy/read_data.py
--rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.7.0/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.7.0/txdpy/selenium_Firefox.py
--rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.7.0/txdpy/str_category.py
--rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.7.0/txdpy/text_similar.py
--rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.7.0/txdpy/translate.py
-drwxrwxrwx   0        0        0        0 2024-05-08 01:17:17.000000 txdpy-7.7.0/txdpy.egg-info/
--rw-rw-rw-   0        0        0       71 2024-05-08 01:17:17.000000 txdpy-7.7.0/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-05-08 01:17:17.000000 txdpy-7.7.0/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 01:17:17.000000 txdpy-7.7.0/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-08 01:17:17.000000 txdpy-7.7.0/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-08 01:17:17.000000 txdpy-7.7.0/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 08:33:56.000000 txdpy-7.7.1/
+-rw-rw-rw-   0        0        0       71 2024-05-10 08:33:56.000000 txdpy-7.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:33:56.000000 txdpy-7.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      378 2024-05-10 08:33:26.000000 txdpy-7.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy/
+-rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/URLjoin.py
+-rw-rw-rw-   0        0        0     2881 2024-05-10 08:31:02.000000 txdpy-7.7.1/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    28642 2024-05-10 07:26:22.000000 txdpy-7.7.1/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0     3855 2024-04-30 03:54:19.000000 txdpy-7.7.1/txdpy/easyreq.py
+-rw-rw-rw-   0        0        0     2403 2024-05-08 01:15:10.000000 txdpy-7.7.1/txdpy/excel_easy.py
+-rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.7.1/txdpy/get_key.py
+-rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/list_processing.py
+-rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/lookup.py
+-rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.7.1/txdpy/progress_display.py
+-rw-rw-rw-   0        0        0     9985 2024-05-10 08:32:05.000000 txdpy-7.7.1/txdpy/pytmysql.py
+-rw-rw-rw-   0        0        0    11855 2024-04-07 07:33:20.000000 txdpy-7.7.1/txdpy/read_data.py
+-rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.7.1/txdpy/requests_operation.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/selenium_Firefox.py
+-rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/str_category.py
+-rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.7.1/txdpy/text_similar.py
+-rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.7.1/txdpy/translate.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/
+-rw-rw-rw-   0        0        0       71 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-10 08:33:56.000000 txdpy-7.7.1/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-7.7.0/txdpy/URLjoin.py` & `txdpy-7.7.1/txdpy/URLjoin.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/__init__.py` & `txdpy-7.7.1/txdpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
            'is_num', 'is_Sletter', 'is_Bletter', 'is_letter', 'is_num_letter', 'is_chinese',
            'get_chinese', 'get_letter', 'get_Bletter', 'get_Sletter', 'get_Sletter', 'get_num', 'get_middle',
            'get_num_letter', 'webptablesl', 'req', 'dow_file', 'list_dupl', 'selenium_firefox', 'get_ssq','is_ssq',
            'prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdmin',
            'txdperc', 'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'prvadepl', 'read_excel',
            'ExtractEnrollmentLabels', 'sortedlbys', 'UpdateName', 'optstr','progbar','text_similar'
            'Recognit_Data_Process','gen_excel','translate','ReadData','get_major_name','GetSchoolName',
-           'get_code_name','unify_keys'
+           'get_code_name','unify_keys','school_ljdm','MysqlConn'
            # 'PyBloomFilter'
            ]
 
 from .URLjoin import urljoin
 from .requests_operation import headers_dict
 from .requests_operation import param_dict
 from .requests_operation import webptablesl
 from .pytmysql import PyMySQL
+from .pytmysql import MysqlConn
 # from .PyReBf import PyBloomFilter
 from .list_processing import si
 from .list_processing import rl
 from .list_processing import list_dupl
 from .list_processing import liduel
 from .str_category import is_num
 from .str_category import is_Sletter
@@ -55,13 +56,14 @@
 from .bk_179 import UpdateName
 from .bk_179 import sortedlbys
 from .bk_179 import optstr
 from .bk_179 import get_major_name
 from .bk_179 import GetSchoolName
 from .bk_179 import get_code_name
 from .bk_179 import unify_keys
+from .bk_179 import school_ljdm
 from .excel_easy import read_excel
 from .excel_easy import gen_excel
 from .translate import translate
 from .read_data import ReadData
 from .progress_display import progbar
 from .text_similar import text_similar
```

### Comparing `txdpy-7.7.0/txdpy/bk_179.py` & `txdpy-7.7.1/txdpy/bk_179.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,8 +547,23 @@
     key_dict={x[0]: x[1] for x in ReadData('读取数据时表头字段统一化参考表').data[1:]}
     for i,k1 in enumerate(ks):
         for k2,ys in key_dict.items():
             for y in ys.split(','):
                 if y==k1:
                     ks[i]=k2
                     break
-    return ks
+    return ks
+
+def school_ljdm():
+    """
+    返回院校逻辑代码
+    """
+    schools = [x[0] for x in ReadData('院校名称').data[1:]]
+    school_dict = {}
+    for x in ReadData('院校库', ['院校逻辑代码', '院校名称']).data[1:]:
+        school_name = optstr(x[1])
+        x_0_re = re.search('\((.+?)\)', school_name)
+        if x_0_re:
+            if x_0_re.group(1).strip('原') in schools:
+                school_name = school_name.replace(f'({x_0_re.group(1)})', '')
+        school_dict[school_name] = x[0]
+    return school_dict
```

### Comparing `txdpy-7.7.0/txdpy/easyreq.py` & `txdpy-7.7.1/txdpy/easyreq.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/excel_easy.py` & `txdpy-7.7.1/txdpy/excel_easy.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/get_key.py` & `txdpy-7.7.1/txdpy/get_key.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/list_processing.py` & `txdpy-7.7.1/txdpy/list_processing.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/lookup.py` & `txdpy-7.7.1/txdpy/lookup.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/progress_display.py` & `txdpy-7.7.1/txdpy/progress_display.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/read_data.py` & `txdpy-7.7.1/txdpy/read_data.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/requests_operation.py` & `txdpy-7.7.1/txdpy/requests_operation.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/selenium_Firefox.py` & `txdpy-7.7.1/txdpy/selenium_Firefox.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/str_category.py` & `txdpy-7.7.1/txdpy/str_category.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/text_similar.py` & `txdpy-7.7.1/txdpy/text_similar.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.7.0/txdpy/translate.py` & `txdpy-7.7.1/txdpy/translate.py`

 * *Files identical despite different names*

