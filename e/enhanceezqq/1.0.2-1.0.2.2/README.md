# Comparing `tmp/enhanceezqq-1.0.2.tar.gz` & `tmp/enhanceezqq-1.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanceezqq-1.0.2.tar", last modified: Sun Mar 17 12:38:08 2024, max compression
+gzip compressed data, was "enhanceezqq-1.0.2.2.tar", last modified: Fri May 10 09:13:53 2024, max compression
```

## Comparing `enhanceezqq-1.0.2.tar` & `enhanceezqq-1.0.2.2.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 12:38:08.569455 enhanceezqq-1.0.2/
--rw-rw-rw-   0        0        0      247 2024-03-17 12:38:08.568455 enhanceezqq-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1043 2024-03-02 05:37:12.000000 enhanceezqq-1.0.2/README.md
--rw-rw-rw-   0        0        0     2696 2024-03-02 05:37:12.000000 enhanceezqq-1.0.2/akpack.py
--rw-rw-rw-   0        0        0     5751 2024-03-17 12:33:24.000000 enhanceezqq-1.0.2/basefund.py
-drwxrwxrwx   0        0        0        0 2024-03-17 12:38:08.546450 enhanceezqq-1.0.2/config/
-drwxrwxrwx   0        0        0        0 2024-03-17 12:38:08.560453 enhanceezqq-1.0.2/config/enhanceezqq/
--rw-rw-rw-   0        0        0      464 2024-03-17 12:33:24.000000 enhanceezqq-1.0.2/config/enhanceezqq/enhanceezqq_config.json
-drwxrwxrwx   0        0        0        0 2024-03-17 12:38:08.566455 enhanceezqq-1.0.2/enhanceezqq.egg-info/
--rw-rw-rw-   0        0        0      247 2024-03-17 12:38:08.000000 enhanceezqq-1.0.2/enhanceezqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-03-17 12:38:08.000000 enhanceezqq-1.0.2/enhanceezqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 12:38:08.000000 enhanceezqq-1.0.2/enhanceezqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      299 2024-03-17 12:38:08.000000 enhanceezqq-1.0.2/enhanceezqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-03-17 12:38:08.000000 enhanceezqq-1.0.2/enhanceezqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18678 2024-03-17 12:33:24.000000 enhanceezqq-1.0.2/enhanceezqq.py
--rw-rw-rw-   0        0        0       42 2024-03-17 12:38:08.569455 enhanceezqq-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     6091 2024-03-17 12:37:54.000000 enhanceezqq-1.0.2/setup.py
--rw-rw-rw-   0        0        0     5674 2024-03-02 05:37:12.000000 enhanceezqq-1.0.2/ths.py
--rw-rw-rw-   0        0        0     5747 2024-03-17 12:33:24.000000 enhanceezqq-1.0.2/ttjj.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:13:53.979633 enhanceezqq-1.0.2.2/
+-rw-rw-rw-   0        0        0      249 2024-05-10 09:13:53.979633 enhanceezqq-1.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1043 2024-03-02 05:37:12.000000 enhanceezqq-1.0.2.2/README.md
+-rw-rw-rw-   0        0        0     5752 2024-04-14 23:08:56.000000 enhanceezqq-1.0.2.2/basefund.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:13:53.960585 enhanceezqq-1.0.2.2/config/
+drwxrwxrwx   0        0        0        0 2024-05-10 09:13:53.969587 enhanceezqq-1.0.2.2/config/enhanceezqq/
+-rw-rw-rw-   0        0        0      464 2024-03-17 12:33:24.000000 enhanceezqq-1.0.2.2/config/enhanceezqq/enhanceezqq_config.json
+drwxrwxrwx   0        0        0        0 2024-05-10 09:13:53.977589 enhanceezqq-1.0.2.2/enhanceezqq.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-05-10 09:13:53.000000 enhanceezqq-1.0.2.2/enhanceezqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-10 09:13:53.000000 enhanceezqq-1.0.2.2/enhanceezqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:13:53.000000 enhanceezqq-1.0.2.2/enhanceezqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      314 2024-05-10 09:13:53.000000 enhanceezqq-1.0.2.2/enhanceezqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-10 09:13:53.000000 enhanceezqq-1.0.2.2/enhanceezqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    20145 2024-05-10 08:39:43.000000 enhanceezqq-1.0.2.2/enhanceezqq.py
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:13:53.980635 enhanceezqq-1.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     6108 2024-05-10 09:12:19.000000 enhanceezqq-1.0.2.2/setup.py
```

### Comparing `enhanceezqq-1.0.2/README.md` & `enhanceezqq-1.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.2/basefund.py` & `enhanceezqq-1.0.2.2/basefund.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 DATABASE_TYPE_SQLITE = 'sqlite'
 DATABASE_TYPE_MYSQL = 'mysql'
 
 
 class BaseFund(basequotation.BaseQuotation):
     """
     同花顺免费行情获取
-    本class继承自basequotation.BaseQuotation，在本clss中，stock codes均表示基金代码，因此无需增加prefix
+    本class继承自basequotation.BaseQuotation，在本class中，stock codes均表示基金代码，因此无需增加prefix
     """
     def __init__(self, ip='', port: int = 8000, database='', user='', password='', select_limit=10000,
                  databasetype="mysql"):
         self.ip = ip.strip()
         self.port = port
         self.database = database.strip()
         self.user = user.strip()
```

### Comparing `enhanceezqq-1.0.2/enhanceezqq.py` & `enhanceezqq-1.0.2.2/enhanceezqq.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # -*- coding: utf-8 -*-
 
 """
 ###############################################################################################################
 # 封装 easyquotation 模块作为获取网络股票数据的工具
 #   -f 优先级最高， -s -c结合获取股票信息
 #   * -s -datasource 数据来源（sina，jsl， qq, tencent, boc, timekline, dayline, hkquote)
+#     datasourcelist = [
+#         'sina',             # sina： A股，sh， sz 000001
+#         'jsl',              # 集思录
+#         'qq',               # 腾讯： A股
+#         'tencent',          # 同上
+#         'boc',              # 中银 外汇牌价，目前只支持usa
+#         'timekline',        # A股 当天K线
+#         'daykline',         # 港股 1500天日K 00001
+#         'hkquote',          # 港股 00001
+#         'ttjj',             # 天天基金, 实时基金估值，如果his -y  则为获取基金历史数据
+#         'ths',              # 同花顺基金, 实时基金估值， 如果his -y 则为获取基金历史数据
+#         'akpack',           # akshare 实时基金估值，如果his -y 则为获取基金历史数据
+#         'funddb',           # 数据库基金历史数据
+#         'stockdb'           # 数据库股票历史数据
+#
+#     ]
 #   * -c -code stockcode1 stockcode2 ...... 股票代码列表, 可以多个
 #   * -p --prefix
 #   * -f -commandfile 使用指定json文件输入命令参数
 #   * -u -updatelist 根据网络数据更新本地stockcode缓冲清单
 #   * -g -getlist （realtime/nonrealtime) 获取stockcode清单，realtime(直接使用网络数据), nonrealtime（使用本地缓冲数据）
 #   * -o -outputfile (结果输出文件，json？ excel？)
 #   :return:
@@ -26,17 +42,17 @@
 import requests
 from df_excel_define import is_mem_virtual_file_name, save_object_to_virtual_file
 
 # 本程序调试时使用
 
 # 外部调用是使用
 import os
-import ttjj
-import ths
-import akpack
+import datasource_ttjj as ttjj
+import datasource_ths as ths
+import datasource_akpack as akpack
 STOCK_RESEARCH_CONFIG = "config/enhanceezqq/enhanceezqq_config.json"
 
 
 class myBoc:
     """中行美元最新汇率"""
 
     url = "http://www.boc.cn/sourcedb/whpj/"
@@ -75,15 +91,15 @@
         for key, value in kwargs.items():
             # 对于每个kwargs， 将key加上“-”， value按空格split为单个串，并且丢弃空串
             argvstr.append("-{}".format(key))
             argvstr += [x for x in value.split(" ") if x]
         # 现有的sys.argv[0]、argc（转换为字符串）、转换后的kwargs合并为完整的sys.argv供argparse模块使用
         sys.argv = [sys.argv[0]] + [str(x) for x in args] + argvstr
         print("内部调用, 将argc:{}, kwargs:{} 转化为argv".format(args, kwargs))
-    print("result sys.argv:{}".format(sys.argv))
+
 
     # 数据源
     datasourcedefault = 'sina'
     # 可用数据源
     datasourcelist = [
         'sina',             # sina： A股，sh， sz 000001
         'jsl',              # 集思录
@@ -141,39 +157,44 @@
     # 是否从网络股票代码信息
     getcodesflag = 'n'
     getcodechoice = ['real', 'local']
     # 输出结果配置文件
     resultconfigfile = 'nan'
     # 默认输出文件名
     resultfile = 'd:/temp/equotation_result.xlsx'
+    # 是否输出过程log到屏幕
+    printlogflag = 'y'
 
     try:
         with open(STOCK_RESEARCH_CONFIG, "r", encoding="utf-8") as fp:
             configdic = json.load(fp)
             databaseinfo = configdic["database"]
             fp.close()
     except Exception as err:
         print("读取配置文件：{}失败：{}".format(STOCK_RESEARCH_CONFIG, err))
         exit(-1)
-    
-    print("默认输入参数：{}".format(sys.argv[1:]))
+
     # 设置各个参数
     parser = argparse.ArgumentParser(description='easyquotation投资交易信息')
     # 获取股票信息来源
     parser.add_argument('-s', '-datasource', type=str,  default=datasourcedefault, choices=datasourcelist,
                         help='股票信息来源：{}, 默认值：{}'.format(datasourcelist, datasourcedefault))
 
     # 需要获取数据的标的代码
     parser.add_argument('-c', '-code', nargs="+", type=str,  default=stockcodesdefault,
                         help='需要获取数据的标的代码列表：[代码1，[代码2,......]], all表示所有, 默认值：{}'.format(
                             stockcodesdefault))
     # 是否增加代码前缀
     parser.add_argument('-p', '-prefixflag', type=str, choices=("y", "n", "Y", "N"), default=prefixflag,
                         help='是否增加代码前缀, 默认值：{}'.format(prefixflag))
 
+    # 是否打印log到屏幕
+    parser.add_argument('-l', '-printlog', type=str, choices=("y", "n", "Y", "N"), default=prefixflag,
+                        help='是否打印log到屏幕, 默认值：{}'.format(printlogflag))
+
     # 是否更新股票本地代码信息
     parser.add_argument('-u', '-updateflag', type=str, choices=("y", "n", "Y", "N"), default=updatecodesflag,
                         help='是否根据网络数据更新股票代码信息的本地缓冲, 默认值：{}'.format(updatecodesflag))
 
     # 是否更新基金或者股票的历史数据本地缓存
     parser.add_argument('-his', '-history', type=str, choices=("y", "n", "Y", "N"), default=historyflag,
                         help='是否根据网络数据更新股票数据的本地缓冲, 默认值：{}'.format(historyflag))
@@ -210,17 +231,21 @@
     myupdateflag = args.u.lower()
     myhistoryflag = args.his.lower()
     mygetcodesflag = args.g.lower()
     myresultconfig = args.f if args.f != resultconfigfile else None
     myresultfile = args.o
     myjsltype = args.j.lower()
     myjslparam = args.t
+    myprintlogflag = True if args.l.lower() == 'y' else False
 
-    print("数据源：{}，标的代码：{}，前缀：{}， 是否更新：{}，获取股票代码方式：{}，jsl: {}, jslparam: {}, 输出文件：{}".format(
-        mydatasource, mystockcodes, myprefixflag, myupdateflag, mygetcodesflag, myjsltype, myjslparam, myresultfile))
+    if myprintlogflag:
+        print("result sys.argv:{}".format(sys.argv))
+        print("默认输入参数：{}".format(sys.argv[1:]))
+        print("数据源：{}，标的代码：{}，前缀：{}， 是否更新：{}，获取股票代码方式：{}，jsl: {}, jslparam: {}, 输出文件：{}".format(
+            mydatasource, mystockcodes, myprefixflag, myupdateflag, mygetcodesflag, myjsltype, myjslparam, myresultfile))
     # 列名与数据对其显示
     pd.set_option('display.unicode.ambiguous_as_wide', True)
     pd.set_option('display.unicode.east_asian_width', True)
     # 显示所有列
     pd.set_option('display.max_columns', None)
     # 显示所有行
     pd.set_option('display.max_rows', None)
@@ -340,15 +365,16 @@
 
     # 当输出是多个df的list时，将输出文件带上序号（第一个不带），
     # 第二个从2开始输出多个输出数据文件，否则用原定义的文件；同时记录所有输出文件名，以便-j使用
     resultfilenameslist = []
     if not isinstance(resultdf, list):
         resultdf = [resultdf]
     for num, df in enumerate(resultdf):
-        print("处理输出结果{}：\n{}".format(num, df))
+        if myprintlogflag:
+            print("处理输出结果{}：\n{}".format(num, df))
         if num == 0:
             # 第一个文件使用原始定义的文件名
             currentoutputfile = myresultfile
         else:
             # 第二个文件开始加上数字序号1-n
             insertposition = myresultfile.rfind(".")
             currentoutputfile = "".join([myresultfile[0: insertposition], str(num), myresultfile[insertposition:]])
@@ -357,15 +383,16 @@
             if is_mem_virtual_file_name(currentoutputfile):
                 save_object_to_virtual_file(currentoutputfile, df)
             else:
                 df.to_excel(currentoutputfile, index=False)
         except Exception as err:
             print("输出到文件{}失败：{}".format(currentoutputfile, err))
             return -1
-        print("{}处理完成！".format(currentoutputfile))
+        if myprintlogflag:
+            print("{}处理完成！".format(currentoutputfile))
 
     # 判断是否产生输出配置文件
     if myresultconfig is not None:
         # 形成输出字典
         tempdict = {"resultfiles": resultfilenameslist}
         try:
             if is_mem_virtual_file_name(myresultconfig):
@@ -373,14 +400,15 @@
             else:
                 with open(myresultconfig, "w", encoding="utf-8") as fp:
                     json.dump(tempdict, fp, ensure_ascii=False, sort_keys=False, indent=4)
                     fp.close()
         except Exception as err:
             print("生成结果配置文件{}失败：{}".format(myresultconfig, err))
             return -1
-        print("结果配置文件{}处理完成！".format(myresultconfig))
+        if myprintlogflag:
+            print("结果配置文件{}处理完成！".format(myresultconfig))
 
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(enhanceezqq_main())
```

### Comparing `enhanceezqq-1.0.2/setup.py` & `enhanceezqq-1.0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,233 +149,234 @@
 00000940: 7269 6769 6e63 6f6e 6669 6764 6972 2c20  riginconfigdir, 
 00000950: 5b6f 7267 696e 636f 6e66 6967 6669 6c65  [orginconfigfile
 00000960: 5d29 2c0d 0a20 2020 2020 2020 205d 0d0a  ]),..        ]..
 00000970: 2020 2020 7265 7475 726e 2064 6174 615f      return data_
 00000980: 6669 6c65 730d 0a0d 0a0d 0a73 6574 7570  files......setup
 00000990: 280d 0a20 2020 206e 616d 653d 2765 6e68  (..    name='enh
 000009a0: 616e 6365 657a 7171 272c 0d0a 2020 2020  anceezqq',..    
-000009b0: 7665 7273 696f 6e3d 2731 2e30 2e32 272c  version='1.0.2',
-000009c0: 0d0a 2020 2020 6465 7363 7269 7074 696f  ..    descriptio
-000009d0: 6e3d 27e7 94a8 e4ba 8ee5 afb9 657a 7171  n='.........ezqq
-000009e0: e6a8 a1e5 9d97 e5a2 9ee5 bcba e58a 9fe8  ................
-000009f0: 83bd efbc 8ce8 83bd e5a4 9fe8 8eb7 e58f  ................
-00000a00: 96e5 8e86 e58f b2e6 95b0 e68d aee4 bf9d  ................
-00000a10: e5ad 98e5 88b0 e695 b0e6 8dae e5ba 93ef  ................
-00000a20: bc8c e5b9 b6e4 bb8e e695 b0e6 8dae e5ba  ................
-00000a30: 93e8 afbb e58f 96e5 8e86 e58f b2e6 95b0  ................
-00000a40: e68d ae27 2c0d 0a20 2020 2061 7574 686f  ...',..    autho
-00000a50: 723d 2746 7261 6e6b 2047 6f6e 6727 2c0d  r='Frank Gong',.
-00000a60: 0a20 2020 2061 7574 686f 725f 656d 6169  .    author_emai
-00000a70: 6c3d 2735 3833 3938 3337 3136 4071 712e  l='583983716@qq.
-00000a80: 636f 6d27 2c0d 0a20 2020 2070 6163 6b61  com',..    packa
-00000a90: 6765 733d 6669 6e64 5f70 6163 6b61 6765  ges=find_package
-00000aa0: 7328 292c 2020 2020 2020 2020 2320 e8a1  s(),        # ..
-00000ab0: a8e7 a4ba e4bd a0e8 a681 e5b0 81e8 a385  ................
-00000ac0: e79a 84e5 8c85 efbc 8c66 696e 645f 7061  .........find_pa
-00000ad0: 636b 6167 6573 e794 a8e4 ba8e e7b3 bbe7  ckages..........
-00000ae0: bb9f e887 aae5 8aa8 e4bb 8ee5 bd93 e589  ................
-00000af0: 8de7 9bae e5bd 95e5 bc80 e5a7 8be6 89be  ................
-00000b00: e58c 850d 0a20 2020 206c 6963 656e 7365  .....    license
-00000b10: 3d22 4253 4422 2c0d 0a20 2020 2070 795f  ="BSD",..    py_
-00000b20: 6d6f 6475 6c65 733d 5b27 656e 6861 6e63  modules=['enhanc
-00000b30: 6565 7a71 7127 2c20 2762 6173 6566 756e  eezqq', 'basefun
-00000b40: 6427 2c20 2774 6873 272c 2027 7474 6a6a  d', 'ths', 'ttjj
-00000b50: 272c 2027 616b 7061 636b 275d 2c0d 0a20  ', 'akpack'],.. 
-00000b60: 2020 2069 6e73 7461 6c6c 5f72 6571 7569     install_requi
-00000b70: 7265 733d 5b27 7061 6e64 6173 7e3d 312e  res=['pandas~=1.
-00000b80: 352e 3227 2c20 276e 756d 7079 7e3d 312e  5.2', 'numpy~=1.
-00000b90: 3234 2e31 272c 2027 6f70 656e 7079 786c  24.1', 'openpyxl
-00000ba0: 272c 2027 6172 6770 6172 7365 272c 2027  ', 'argparse', '
-00000bb0: 7061 7468 6c69 6227 2c0d 0a20 2020 2020  pathlib',..     
+000009b0: 7665 7273 696f 6e3d 2731 2e30 2e32 2e32  version='1.0.2.2
+000009c0: 272c 0d0a 2020 2020 6465 7363 7269 7074  ',..    descript
+000009d0: 696f 6e3d 27e7 94a8 e4ba 8ee5 afb9 657a  ion='.........ez
+000009e0: 7171 e6a8 a1e5 9d97 e5a2 9ee5 bcba e58a  qq..............
+000009f0: 9fe8 83bd efbc 8ce8 83bd e5a4 9fe8 8eb7  ................
+00000a00: e58f 96e5 8e86 e58f b2e6 95b0 e68d aee4  ................
+00000a10: bf9d e5ad 98e5 88b0 e695 b0e6 8dae e5ba  ................
+00000a20: 93ef bc8c e5b9 b6e4 bb8e e695 b0e6 8dae  ................
+00000a30: e5ba 93e8 afbb e58f 96e5 8e86 e58f b2e6  ................
+00000a40: 95b0 e68d ae27 2c0d 0a20 2020 2061 7574  .....',..    aut
+00000a50: 686f 723d 2746 7261 6e6b 2047 6f6e 6727  hor='Frank Gong'
+00000a60: 2c0d 0a20 2020 2061 7574 686f 725f 656d  ,..    author_em
+00000a70: 6169 6c3d 2735 3833 3938 3337 3136 4071  ail='583983716@q
+00000a80: 712e 636f 6d27 2c0d 0a20 2020 2070 6163  q.com',..    pac
+00000a90: 6b61 6765 733d 6669 6e64 5f70 6163 6b61  kages=find_packa
+00000aa0: 6765 7328 292c 2020 2020 2020 2020 2320  ges(),        # 
+00000ab0: e8a1 a8e7 a4ba e4bd a0e8 a681 e5b0 81e8  ................
+00000ac0: a385 e79a 84e5 8c85 efbc 8c66 696e 645f  ...........find_
+00000ad0: 7061 636b 6167 6573 e794 a8e4 ba8e e7b3  packages........
+00000ae0: bbe7 bb9f e887 aae5 8aa8 e4bb 8ee5 bd93  ................
+00000af0: e589 8de7 9bae e5bd 95e5 bc80 e5a7 8be6  ................
+00000b00: 89be e58c 850d 0a20 2020 206c 6963 656e  .......    licen
+00000b10: 7365 3d22 4253 4422 2c0d 0a20 2020 2070  se="BSD",..    p
+00000b20: 795f 6d6f 6475 6c65 733d 5b27 656e 6861  y_modules=['enha
+00000b30: 6e63 6565 7a71 7127 2c20 2762 6173 6566  nceezqq', 'basef
+00000b40: 756e 6427 2c20 2774 6873 272c 2027 7474  und', 'ths', 'tt
+00000b50: 6a6a 272c 2027 616b 7061 636b 275d 2c0d  jj', 'akpack'],.
+00000b60: 0a20 2020 2069 6e73 7461 6c6c 5f72 6571  .    install_req
+00000b70: 7569 7265 733d 5b27 7061 6e64 6173 7e3d  uires=['pandas~=
+00000b80: 312e 352e 3227 2c20 276e 756d 7079 7e3d  1.5.2', 'numpy~=
+00000b90: 312e 3234 2e31 272c 2027 6f70 656e 7079  1.24.1', 'openpy
+00000ba0: 786c 272c 2027 6172 6770 6172 7365 272c  xl', 'argparse',
+00000bb0: 2027 7061 7468 6c69 6227 2c0d 0a20 2020   'pathlib',..   
 00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 2027 7365 6c65 6e69 756d 272c 2027 7265   'selenium', 're
-00000be0: 7175 6573 7473 272c 2027 786c 7264 272c  quests', 'xlrd',
-00000bf0: 2027 626f 7474 6c65 272c 2027 5079 5369   'bottle', 'PySi
-00000c00: 6d70 6c65 4755 4927 2c0d 0a20 2020 2020  mpleGUI',..     
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 2027 6368 6172 6465 7427 2c20 276e 7569   'chardet', 'nui
-00000c30: 746b 6127 2c20 2750 7951 7435 272c 2027  tka', 'PyQt5', '
-00000c40: 7079 6372 7970 746f 646f 6d65 7827 2c20  pycryptodomex', 
-00000c50: 2764 6174 6163 6f6d 7079 272c 2027 616b  'datacompy', 'ak
-00000c60: 7368 6172 6527 2c0d 0a20 2020 2020 2020  share',..       
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000c80: 7368 6f72 7475 7569 6427 2c20 2773 716c  shortuuid', 'sql
-00000c90: 616c 6368 656d 793d 3d31 2e34 2e34 3627  alchemy==1.4.46'
-00000ca0: 2c20 276d 7973 716c 2d63 6f6e 6e65 6374  , 'mysql-connect
-00000cb0: 6f72 2d70 7974 686f 6e27 2c20 2769 7079  or-python', 'ipy
-00000cc0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00000cd0: 2020 2020 2020 2020 2020 2770 6174 686f            'patho
-00000ce0: 7327 2c20 2770 796d 7973 716c 272c 2027  s', 'pymysql', '
-00000cf0: 636f 6c6f 726c 6f67 272c 2027 6d61 7470  colorlog', 'matp
-00000d00: 6c6f 746c 6962 272c 2027 7079 7069 6e79  lotlib', 'pypiny
-00000d10: 696e 272c 0d0a 2020 2020 2020 2020 2020  in',..          
-00000d20: 2020 2020 2020 2020 2020 2020 2770 7978              'pyx
-00000d30: 6c73 6227 2c20 276a 736f 6e6c 696e 6573  lsb', 'jsonlines
-00000d40: 272c 2027 6561 7379 7175 6f74 6174 696f  ', 'easyquotatio
-00000d50: 6e27 2c20 274a 696e 6a61 3227 2c20 2762  n', 'Jinja2', 'b
-00000d60: 7334 272c 2027 4446 5472 616e 7327 5d2c  s4', 'DFTrans'],
-00000d70: 0d0a 2020 2020 6461 7461 5f66 696c 6573  ..    data_files
-00000d80: 3d69 6e69 745f 6461 7461 5f66 696c 6573  =init_data_files
-00000d90: 2829 2c0d 0a20 2020 2023 2063 6c61 7373  (),..    # class
-00000da0: 6966 6965 7273 3d5b 0d0a 2020 2020 2320  ifiers=[..    # 
-00000db0: 2020 2020 2320 e58f 91e5 b195 e697 b6e6      # ..........
-00000dc0: 9c9f 2ce5 b8b8 e8a7 81e7 9a84 e5a6 82e4  ..,.............
-00000dd0: b88b 0d0a 2020 2020 2320 2020 2020 2320  ....    #     # 
-00000de0: 2020 3320 2d20 416c 7068 610d 0a20 2020    3 - Alpha..   
-00000df0: 2023 2020 2020 2023 2020 2034 202d 2042   #     #   4 - B
-00000e00: 6574 610d 0a20 2020 2023 2020 2020 2023  eta..    #     #
-00000e10: 2020 2035 202d 2050 726f 6475 6374 696f     5 - Productio
-00000e20: 6e2f 5374 6162 6c65 0d0a 2020 2020 2320  n/Stable..    # 
-00000e30: 2020 2020 2744 6576 656c 6f70 6d65 6e74      'Development
-00000e40: 2053 7461 7475 7320 3a3a 2035 202d 2053   Status :: 5 - S
-00000e50: 7461 626c 6527 2c0d 0a20 2020 2023 2020  table',..    #  
-00000e60: 2020 2023 20e5 bc80 e58f 91e7 9a84 e79b     # ...........
-00000e70: aee6 a087 e794 a8e6 88b7 0d0a 2020 2020  ............    
-00000e80: 2320 2020 2020 2749 6e74 656e 6465 6420  #     'Intended 
-00000e90: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000ea0: 6c6f 7065 7273 272c 0d0a 2020 2020 2320  lopers',..    # 
-00000eb0: 2020 2020 2320 e5b1 9ee4 ba8e e4bb 80e4      # ..........
-00000ec0: b988 e7b1 bbe5 9e8b 0d0a 2020 2020 2320  ..........    # 
-00000ed0: 2020 2020 2754 6f70 6963 203a 3a20 536f      'Topic :: So
-00000ee0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-00000ef0: 6e74 203a 3a20 546f 6f6c 7327 2c0d 0a20  nt :: Tools',.. 
-00000f00: 2020 2023 2020 2020 2023 20e8 aeb8 e58f     #     # .....
-00000f10: afe8 af81 e4bf a1e6 81af 0d0a 2020 2020  ............    
-00000f20: 2320 2020 2020 274c 6963 656e 7365 203a  #     'License :
-00000f30: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000f40: 3a20 4253 4420 4c69 6365 6e73 6527 2c0d  : BSD License',.
-00000f50: 0a20 2020 2023 2020 2020 2023 20e7 9bae  .    #     # ...
-00000f60: e6a0 8720 5079 7468 6f6e 20e7 8988 e69c  ... Python .....
-00000f70: ac0d 0a20 2020 2023 2020 2020 2027 5072  ...    #     'Pr
-00000f80: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000f90: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000fa0: 3327 2c0d 0a20 2020 2023 2020 2020 2027  3',..    #     '
-00000fb0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000fc0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000fd0: 3a20 332e 3627 2c0d 0a20 2020 2023 2020  : 3.6',..    #  
-00000fe0: 2020 2027 5072 6f67 7261 6d6d 696e 6720     'Programming 
-00000ff0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00001000: 6f6e 203a 3a20 332e 3727 2c0d 0a20 2020  on :: 3.7',..   
-00001010: 2023 2020 2020 2027 5072 6f67 7261 6d6d   #     'Programm
-00001020: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00001030: 5079 7468 6f6e 203a 3a20 332e 3827 2c0d  Python :: 3.8',.
-00001040: 0a20 2020 2023 2020 2020 2027 5072 6f67  .    #     'Prog
-00001050: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00001060: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00001070: 3927 2c0d 0a20 2020 2023 205d 0d0a 290d  9',..    # ]..).
-00001080: 0a27 2727 0d0a 6e61 6d65 203a 20e6 8993  .'''..name : ...
-00001090: e58c 85e5 908e e58c 85e7 9a84 e696 87e4  ................
-000010a0: bbb6 e590 8d0d 0a76 6572 7369 6f6e 203a  .......version :
-000010b0: 20e7 8988 e69c ace5 8fb7 0d0a 6175 7468   ...........auth
-000010c0: 6f72 203a 20e4 bd9c e880 850d 0a61 7574  or : ........aut
-000010d0: 686f 725f 656d 6169 6c20 3a20 e4bd 9ce8  hor_email : ....
-000010e0: 8085 e79a 84e9 82ae e7ae b10d 0a70 795f  .............py_
-000010f0: 6d6f 6475 6c65 7320 3a20 e8a6 81e6 8993  modules : ......
-00001100: e58c 85e7 9a84 2e70 79e6 9687 e4bb b60d  .......py.......
-00001110: 0a70 6163 6b61 6765 733a 20e6 8993 e58c  .packages: .....
-00001120: 85e7 9a84 7079 7468 6f6e e696 87e4 bbb6  ....python......
-00001130: e5a4 b90d 0a69 6e63 6c75 6465 5f70 6163  .....include_pac
-00001140: 6b61 6765 5f64 6174 6120 3a20 e9a1 b9e7  kage_data : ....
-00001150: 9bae e987 8ce4 bc9a e69c 89e4 b880 e4ba  ................
-00001160: 9be9 9d9e 7079 e696 87e4 bbb6 2ce6 af94  ....py......,...
-00001170: e5a6 8268 746d 6ce5 928c 6a73 e7ad 892c  ...html...js...,
-00001180: e8bf 99e6 97b6 e580 99e5 b0b1 e8a6 81e9  ................
-00001190: 9da0 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-000011a0: 655f 6461 7461 20e5 928c 2070 6163 6b61  e_data ... packa
-000011b0: 6765 5f64 6174 6120 e69d a5e6 8c87 e5ae  ge_data ........
-000011c0: 9ae4 ba86 e380 8270 6163 6b61 6765 5f64  .......package_d
-000011d0: 6174 613a e4b8 80e8 88ac e586 99e6 8890  ata:............
-000011e0: 7be2 8098 796f 7572 5f70 6163 6b61 6765  {...your_package
-000011f0: 5f6e 616d 65e2 8099 3a20 5be2 809c 6669  _name...: [...fi
-00001200: 6c65 73e2 809d 5d7d 2c20 696e 636c 7564  les...]}, includ
-00001210: 655f 7061 636b 6167 655f 6461 7461 e8bf  e_package_data..
-00001220: 98e6 b2a1 e5ae 8c2c e8bf 98e9 9c80 e8a6  .......,........
-00001230: 81e4 bfae e694 b94d 414e 4946 4553 542e  .......MANIFEST.
-00001240: 696e e696 87e4 bbb6 2e4d 414e 4946 4553  in.......MANIFES
-00001250: 542e 696e e696 87e4 bbb6 e79a 84e8 afad  T.in............
-00001260: e6b3 95e4 b8ba 3a20 696e 636c 7564 6520  ......: include 
-00001270: 7878 782f 7878 782f 7878 782f 2e69 6e69  xxx/xxx/xxx/.ini
-00001280: 2f28 e689 80e6 9c89 e4bb a52e 696e 69e7  /(..........ini.
-00001290: bb93 e5b0 bee7 9a84 e696 87e4 bbb6 2ce4  ..............,.
-000012a0: b99f e58f afe4 bba5 e79b b4e6 8ea5 e68c  ................
-000012b0: 87e5 ae9a e696 87e4 bbb6 e590 8d29 0d0a  .............)..
-000012c0: 6c69 6365 6e73 6520 3a20 e694 afe6 8c81  license : ......
-000012d0: e79a 84e5 bc80 e6ba 90e5 8d8f e8ae ae0d  ................
-000012e0: 0a64 6573 6372 6970 7469 6f6e 203a 20e5  .description : .
-000012f0: afb9 e9a1 b9e7 9bae e7ae 80e7 9fad e79a  ................
-00001300: 84e4 b880 e4b8 aae5 bda2 e5ae b90d 0a65  ...............e
-00001310: 7874 5f6d 6f64 756c 6573 203a 20e6 98af  xt_modules : ...
-00001320: e4b8 80e4 b8aa e58c 85e5 90ab 4578 7465  ............Exte
-00001330: 6e73 696f 6ee5 ae9e e4be 8be7 9a84 e588  nsion...........
-00001340: 97e8 a1a8 2c45 7874 656e 7369 6f6e e79a  ....,Extension..
-00001350: 84e5 ae9a e4b9 89e4 b99f e69c 89e4 b880  ................
-00001360: e4ba 9be5 8f82 e695 b0e3 8082 0d0a 6578  ..............ex
-00001370: 745f 7061 636b 6167 6520 3a20 e5ae 9ae4  t_package : ....
-00001380: b989 6578 7465 6e73 696f 6ee7 9a84 e79b  ..extension.....
-00001390: b8e5 afb9 e8b7 afe5 be84 0d0a 7265 7175  ............requ
-000013a0: 6972 6573 203a 20e5 ae9a e4b9 89e4 be9d  ires : .........
-000013b0: e8b5 96e5 93aa e4ba 9be6 a8a1 e59d 970d  ................
-000013c0: 0a70 726f 7669 6465 7320 3a20 e5ae 9ae4  .provides : ....
-000013d0: b989 e58f afe4 bba5 e4b8 bae5 93aa e4ba  ................
-000013e0: 9be6 a8a1 e59d 97e6 8f90 e4be 9be4 be9d  ................
-000013f0: e8b5 960d 0a64 6174 615f 6669 6c65 7320  .....data_files 
-00001400: 3ae6 8c87 e5ae 9ae5 85b6 e4bb 96e7 9a84  :...............
-00001410: e4b8 80e4 ba9b e696 87e4 bbb6 28e5 a682  ............(...
-00001420: e985 8de7 bdae e696 87e4 bbb6 292c e8a7  ............),..
-00001430: 84e5 ae9a e4ba 86e5 93aa e4ba 9be6 9687  ................
-00001440: e4bb b6e8 a2ab e5ae 89e8 a385 e588 b0e5  ................
-00001450: 93aa e4ba 9be7 9bae e5bd 95e4 b8ad e380  ................
-00001460: 82e5 a682 e69e 9ce7 9bae e5bd 95e5 908d  ................
-00001470: e698 afe7 9bb8 e5af b9e8 b7af e5be 842c  ...............,
-00001480: e588 99e6 98af e79b b8e5 afb9 e4ba 8e73  ...............s
-00001490: 7973 2e70 7265 6669 78e6 8896 7379 732e  ys.prefix...sys.
-000014a0: 6578 6563 5f70 7265 6669 78e7 9a84 e8b7  exec_prefix.....
-000014b0: afe5 be84 e380 82e5 a682 e69e 9ce6 b2a1  ................
-000014c0: e69c 89e6 8f90 e4be 9be6 a8a1 e69d bf2c  ...............,
-000014d0: e4bc 9ae8 a2ab e6b7 bbe5 8aa0 e588 b04d  ...............M
-000014e0: 414e 4946 4553 54e6 9687 e4bb b6e4 b8ad  ANIFEST.........
-000014f0: e380 820d 0a20 2020 2023 20e5 b88c e69c  .....    # .....
-00001500: 9be8 a2ab e689 93e5 8c85 e79a 84e6 9687  ................
-00001510: e4bb b60d 0a20 2020 2070 6163 6b61 6765  .....    package
-00001520: 5f64 6174 613d 7b0d 0a20 2020 2020 2020  _data={..       
-00001530: 2027 273a 5b27 2a2e 7478 7427 5d2c 0d0a   '':['*.txt'],..
-00001540: 2020 2020 2020 2020 2762 616e 6477 6964          'bandwid
-00001550: 7468 5f72 6570 6f72 7465 7227 3a5b 272a  th_reporter':['*
-00001560: 2e74 7874 275d 0d0a 2020 2020 2020 2020  .txt']..        
-00001570: 2020 2020 2020 207d 2c0d 0a20 2020 2023         },..    #
-00001580: 20e4 b88d e689 93e5 8c85 e69f 90e4 ba9b   ...............
-00001590: e696 87e4 bbb6 0d0a 2020 2020 6578 636c  ........    excl
-000015a0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-000015b0: 3d7b 0d0a 2020 2020 2020 2020 2762 616e  ={..        'ban
-000015c0: 6477 6964 7468 5f72 6570 6f72 7465 7227  dwidth_reporter'
-000015d0: 3a5b 272a 2e74 7874 275d 0d0a 2020 2020  :['*.txt']..    
-000015e0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-000015f0: 2020 2020 2320 e794 a8e6 9da5 e694 afe6      # ..........
-00001600: 8c81 e887 aae5 8aa8 e794 9fe6 8890 e884  ................
-00001610: 9ae6 9cac efbc 8ce5 ae89 e8a3 85e5 908e  ................
-00001620: e4bc 9ae8 87aa e58a a8e7 949f e688 9020  ............... 
-00001630: 2f75 7372 2f62 696e 2f66 6f6f 20e7 9a84  /usr/bin/foo ...
-00001640: e58f afe6 89a7 e8a1 8ce6 9687 e4bb b60d  ................
-00001650: 0a20 2020 2023 20e8 afa5 e696 87e4 bbb6  .    # .........
-00001660: e585 a5e5 8fa3 e68c 87e5 9091 2066 6f6f  ............ foo
-00001670: 2f6d 6169 6e2e 7079 20e7 9a84 6d61 696e  /main.py ...main
-00001680: 20e5 87bd e695 b00d 0a20 2020 2065 6e74   ........    ent
-00001690: 7279 5f70 6f69 6e74 733d 7b0d 0a20 2020  ry_points={..   
-000016a0: 2020 2020 2027 636f 6e73 6f6c 655f 7363       'console_sc
-000016b0: 7269 7074 7327 3a20 5b0d 0a20 2020 2020  ripts': [..     
-000016c0: 2020 2020 2020 2027 666f 6f20 3d20 666f         'foo = fo
-000016d0: 6f2e 6d61 696e 3a6d 6169 6e27 0d0a 2020  o.main:main'..  
-000016e0: 2020 2020 2020 5d0d 0a20 2020 207d 2c0d        ]..    },.
-000016f0: 0a0d 0a20 2020 2023 20e5 b086 2062 696e  ...    # ... bin
-00001700: 2f66 6f6f 2e73 6820 e592 8c20 6261 722e  /foo.sh ... bar.
-00001710: 7079 20e8 849a e69c acef bc8c e794 9fe6  py .............
-00001720: 8890 e588 b0e7 b3bb e7bb 9f20 5041 5448  ........... PATH
-00001730: e4b8 ad0d 0a20 2020 2023 20e6 89a7 e8a1  .....    # .....
-00001740: 8c20 7079 7468 6f6e 2073 6574 7570 2e70  . python setup.p
-00001750: 7920 696e 7374 616c 6c20 e590 8e0d 0a20  y install ..... 
-00001760: 2020 2023 20e4 bc9a e794 9fe6 8890 20e5     # ......... .
-00001770: a682 202f 7573 722f 6269 6e2f 666f 6f2e  .. /usr/bin/foo.
-00001780: 7368 20e5 928c 20e5 a682 202f 7573 722f  sh ... ... /usr/
-00001790: 6269 6e2f 6261 722e 7079 0d0a 2020 2020  bin/bar.py..    
-000017a0: 7363 7269 7074 733d 5b27 6269 6e2f 666f  scripts=['bin/fo
-000017b0: 6f2e 7368 272c 2027 6261 722e 7079 275d  o.sh', 'bar.py']
-000017c0: 0d0a 2727 270d 0a0d 0a0d 0a              ..'''......
+00000bd0: 2020 2027 7365 6c65 6e69 756d 272c 2027     'selenium', '
+00000be0: 7265 7175 6573 7473 272c 2027 786c 7264  requests', 'xlrd
+00000bf0: 272c 2027 626f 7474 6c65 272c 2027 5079  ', 'bottle', 'Py
+00000c00: 5369 6d70 6c65 4755 497e 3d34 2e36 302e  SimpleGUI~=4.60.
+00000c10: 3527 2c0d 0a20 2020 2020 2020 2020 2020  5',..           
+00000c20: 2020 2020 2020 2020 2020 2027 6368 6172             'char
+00000c30: 6465 7427 2c20 276e 7569 746b 6127 2c20  det', 'nuitka', 
+00000c40: 2750 7951 7435 272c 2027 7079 6372 7970  'PyQt5', 'pycryp
+00000c50: 746f 646f 6d65 7827 2c20 2764 6174 6163  todomex', 'datac
+00000c60: 6f6d 7079 272c 2027 616b 7368 6172 6527  ompy', 'akshare'
+00000c70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000c80: 2020 2020 2020 2020 2027 7368 6f72 7475           'shortu
+00000c90: 7569 6427 2c20 2773 716c 616c 6368 656d  uid', 'sqlalchem
+00000ca0: 793d 3d31 2e34 2e34 3627 2c20 276d 7973  y==1.4.46', 'mys
+00000cb0: 716c 2d63 6f6e 6e65 6374 6f72 2d70 7974  ql-connector-pyt
+00000cc0: 686f 6e27 2c20 2769 7079 272c 0d0a 2020  hon', 'ipy',..  
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 2020 2020 2770 6174 686f 7327 2c20 2770      'pathos', 'p
+00000cf0: 796d 7973 716c 272c 2027 636f 6c6f 726c  ymysql', 'colorl
+00000d00: 6f67 272c 2027 6d61 7470 6c6f 746c 6962  og', 'matplotlib
+00000d10: 7e3d 332e 372e 3227 2c20 2770 7970 696e  ~=3.7.2', 'pypin
+00000d20: 7969 6e27 2c0d 0a20 2020 2020 2020 2020  yin',..         
+00000d30: 2020 2020 2020 2020 2020 2020 2027 7079               'py
+00000d40: 786c 7362 272c 2027 6a73 6f6e 6c69 6e65  xlsb', 'jsonline
+00000d50: 7327 2c20 2765 6173 7971 756f 7461 7469  s', 'easyquotati
+00000d60: 6f6e 272c 2027 4a69 6e6a 6132 272c 2027  on', 'Jinja2', '
+00000d70: 6273 3427 2c20 2744 4654 7261 6e73 275d  bs4', 'DFTrans']
+00000d80: 2c0d 0a20 2020 2064 6174 615f 6669 6c65  ,..    data_file
+00000d90: 733d 696e 6974 5f64 6174 615f 6669 6c65  s=init_data_file
+00000da0: 7328 292c 0d0a 2020 2020 2320 636c 6173  s(),..    # clas
+00000db0: 7369 6669 6572 733d 5b0d 0a20 2020 2023  sifiers=[..    #
+00000dc0: 2020 2020 2023 20e5 8f91 e5b1 95e6 97b6       # .........
+00000dd0: e69c 9f2c e5b8 b8e8 a781 e79a 84e5 a682  ...,............
+00000de0: e4b8 8b0d 0a20 2020 2023 2020 2020 2023  .....    #     #
+00000df0: 2020 2033 202d 2041 6c70 6861 0d0a 2020     3 - Alpha..  
+00000e00: 2020 2320 2020 2020 2320 2020 3420 2d20    #     #   4 - 
+00000e10: 4265 7461 0d0a 2020 2020 2320 2020 2020  Beta..    #     
+00000e20: 2320 2020 3520 2d20 5072 6f64 7563 7469  #   5 - Producti
+00000e30: 6f6e 2f53 7461 626c 650d 0a20 2020 2023  on/Stable..    #
+00000e40: 2020 2020 2027 4465 7665 6c6f 706d 656e       'Developmen
+00000e50: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
+00000e60: 5374 6162 6c65 272c 0d0a 2020 2020 2320  Stable',..    # 
+00000e70: 2020 2020 2320 e5bc 80e5 8f91 e79a 84e7      # ..........
+00000e80: 9bae e6a0 87e7 94a8 e688 b70d 0a20 2020  .............   
+00000e90: 2023 2020 2020 2027 496e 7465 6e64 6564   #     'Intended
+00000ea0: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000eb0: 656c 6f70 6572 7327 2c0d 0a20 2020 2023  elopers',..    #
+00000ec0: 2020 2020 2023 20e5 b19e e4ba 8ee4 bb80       # .........
+00000ed0: e4b9 88e7 b1bb e59e 8b0d 0a20 2020 2023  ...........    #
+00000ee0: 2020 2020 2027 546f 7069 6320 3a3a 2053       'Topic :: S
+00000ef0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000f00: 656e 7420 3a3a 2054 6f6f 6c73 272c 0d0a  ent :: Tools',..
+00000f10: 2020 2020 2320 2020 2020 2320 e8ae b8e5      #     # ....
+00000f20: 8faf e8af 81e4 bfa1 e681 af0d 0a20 2020  .............   
+00000f30: 2023 2020 2020 2027 4c69 6365 6e73 6520   #     'License 
+00000f40: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000f50: 3a3a 2042 5344 204c 6963 656e 7365 272c  :: BSD License',
+00000f60: 0d0a 2020 2020 2320 2020 2020 2320 e79b  ..    #     # ..
+00000f70: aee6 a087 2050 7974 686f 6e20 e789 88e6  .... Python ....
+00000f80: 9cac 0d0a 2020 2020 2320 2020 2020 2750  ....    #     'P
+00000f90: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000fa0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000fb0: 2033 272c 0d0a 2020 2020 2320 2020 2020   3',..    #     
+00000fc0: 2750 726f 6772 616d 6d69 6e67 204c 616e  'Programming Lan
+00000fd0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000fe0: 3a3a 2033 2e36 272c 0d0a 2020 2020 2320  :: 3.6',..    # 
+00000ff0: 2020 2020 2750 726f 6772 616d 6d69 6e67      'Programming
+00001000: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00001010: 686f 6e20 3a3a 2033 2e37 272c 0d0a 2020  hon :: 3.7',..  
+00001020: 2020 2320 2020 2020 2750 726f 6772 616d    #     'Program
+00001030: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00001040: 2050 7974 686f 6e20 3a3a 2033 2e38 272c   Python :: 3.8',
+00001050: 0d0a 2020 2020 2320 2020 2020 2750 726f  ..    #     'Pro
+00001060: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00001070: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00001080: 2e39 272c 0d0a 2020 2020 2320 5d0d 0a29  .9',..    # ]..)
+00001090: 0d0a 2727 270d 0a6e 616d 6520 3a20 e689  ..'''..name : ..
+000010a0: 93e5 8c85 e590 8ee5 8c85 e79a 84e6 9687  ................
+000010b0: e4bb b6e5 908d 0d0a 7665 7273 696f 6e20  ........version 
+000010c0: 3a20 e789 88e6 9cac e58f b70d 0a61 7574  : ...........aut
+000010d0: 686f 7220 3a20 e4bd 9ce8 8085 0d0a 6175  hor : ........au
+000010e0: 7468 6f72 5f65 6d61 696c 203a 20e4 bd9c  thor_email : ...
+000010f0: e880 85e7 9a84 e982 aee7 aeb1 0d0a 7079  ..............py
+00001100: 5f6d 6f64 756c 6573 203a 20e8 a681 e689  _modules : .....
+00001110: 93e5 8c85 e79a 842e 7079 e696 87e4 bbb6  ........py......
+00001120: 0d0a 7061 636b 6167 6573 3a20 e689 93e5  ..packages: ....
+00001130: 8c85 e79a 8470 7974 686f 6ee6 9687 e4bb  .....python.....
+00001140: b6e5 a4b9 0d0a 696e 636c 7564 655f 7061  ......include_pa
+00001150: 636b 6167 655f 6461 7461 203a 20e9 a1b9  ckage_data : ...
+00001160: e79b aee9 878c e4bc 9ae6 9c89 e4b8 80e4  ................
+00001170: ba9b e99d 9e70 79e6 9687 e4bb b62c e6af  .....py......,..
+00001180: 94e5 a682 6874 6d6c e592 8c6a 73e7 ad89  ....html...js...
+00001190: 2ce8 bf99 e697 b6e5 8099 e5b0 b1e8 a681  ,...............
+000011a0: e99d a069 6e63 6c75 6465 5f70 6163 6b61  ...include_packa
+000011b0: 6765 5f64 6174 6120 e592 8c20 7061 636b  ge_data ... pack
+000011c0: 6167 655f 6461 7461 20e6 9da5 e68c 87e5  age_data .......
+000011d0: ae9a e4ba 86e3 8082 7061 636b 6167 655f  ........package_
+000011e0: 6461 7461 3ae4 b880 e888 ace5 8699 e688  data:...........
+000011f0: 907b e280 9879 6f75 725f 7061 636b 6167  .{...your_packag
+00001200: 655f 6e61 6d65 e280 993a 205b e280 9c66  e_name...: [...f
+00001210: 696c 6573 e280 9d5d 7d2c 2069 6e63 6c75  iles...]}, inclu
+00001220: 6465 5f70 6163 6b61 6765 5f64 6174 61e8  de_package_data.
+00001230: bf98 e6b2 a1e5 ae8c 2ce8 bf98 e99c 80e8  ........,.......
+00001240: a681 e4bf aee6 94b9 4d41 4e49 4645 5354  ........MANIFEST
+00001250: 2e69 6ee6 9687 e4bb b62e 4d41 4e49 4645  .in.......MANIFE
+00001260: 5354 2e69 6ee6 9687 e4bb b6e7 9a84 e8af  ST.in...........
+00001270: ade6 b395 e4b8 ba3a 2069 6e63 6c75 6465  .......: include
+00001280: 2078 7878 2f78 7878 2f78 7878 2f2e 696e   xxx/xxx/xxx/.in
+00001290: 692f 28e6 8980 e69c 89e4 bba5 2e69 6e69  i/(..........ini
+000012a0: e7bb 93e5 b0be e79a 84e6 9687 e4bb b62c  ...............,
+000012b0: e4b9 9fe5 8faf e4bb a5e7 9bb4 e68e a5e6  ................
+000012c0: 8c87 e5ae 9ae6 9687 e4bb b6e5 908d 290d  ..............).
+000012d0: 0a6c 6963 656e 7365 203a 20e6 94af e68c  .license : .....
+000012e0: 81e7 9a84 e5bc 80e6 ba90 e58d 8fe8 aeae  ................
+000012f0: 0d0a 6465 7363 7269 7074 696f 6e20 3a20  ..description : 
+00001300: e5af b9e9 a1b9 e79b aee7 ae80 e79f ade7  ................
+00001310: 9a84 e4b8 80e4 b8aa e5bd a2e5 aeb9 0d0a  ................
+00001320: 6578 745f 6d6f 6475 6c65 7320 3a20 e698  ext_modules : ..
+00001330: afe4 b880 e4b8 aae5 8c85 e590 ab45 7874  .............Ext
+00001340: 656e 7369 6f6e e5ae 9ee4 be8b e79a 84e5  ension..........
+00001350: 8897 e8a1 a82c 4578 7465 6e73 696f 6ee7  .....,Extension.
+00001360: 9a84 e5ae 9ae4 b989 e4b9 9fe6 9c89 e4b8  ................
+00001370: 80e4 ba9b e58f 82e6 95b0 e380 820d 0a65  ...............e
+00001380: 7874 5f70 6163 6b61 6765 203a 20e5 ae9a  xt_package : ...
+00001390: e4b9 8965 7874 656e 7369 6f6e e79a 84e7  ...extension....
+000013a0: 9bb8 e5af b9e8 b7af e5be 840d 0a72 6571  .............req
+000013b0: 7569 7265 7320 3a20 e5ae 9ae4 b989 e4be  uires : ........
+000013c0: 9de8 b596 e593 aae4 ba9b e6a8 a1e5 9d97  ................
+000013d0: 0d0a 7072 6f76 6964 6573 203a 20e5 ae9a  ..provides : ...
+000013e0: e4b9 89e5 8faf e4bb a5e4 b8ba e593 aae4  ................
+000013f0: ba9b e6a8 a1e5 9d97 e68f 90e4 be9b e4be  ................
+00001400: 9de8 b596 0d0a 6461 7461 5f66 696c 6573  ......data_files
+00001410: 203a e68c 87e5 ae9a e585 b6e4 bb96 e79a   :..............
+00001420: 84e4 b880 e4ba 9be6 9687 e4bb b628 e5a6  .............(..
+00001430: 82e9 858d e7bd aee6 9687 e4bb b629 2ce8  .............),.
+00001440: a784 e5ae 9ae4 ba86 e593 aae4 ba9b e696  ................
+00001450: 87e4 bbb6 e8a2 abe5 ae89 e8a3 85e5 88b0  ................
+00001460: e593 aae4 ba9b e79b aee5 bd95 e4b8 ade3  ................
+00001470: 8082 e5a6 82e6 9e9c e79b aee5 bd95 e590  ................
+00001480: 8de6 98af e79b b8e5 afb9 e8b7 afe5 be84  ................
+00001490: 2ce5 8899 e698 afe7 9bb8 e5af b9e4 ba8e  ,...............
+000014a0: 7379 732e 7072 6566 6978 e688 9673 7973  sys.prefix...sys
+000014b0: 2e65 7865 635f 7072 6566 6978 e79a 84e8  .exec_prefix....
+000014c0: b7af e5be 84e3 8082 e5a6 82e6 9e9c e6b2  ................
+000014d0: a1e6 9c89 e68f 90e4 be9b e6a8 a1e6 9dbf  ................
+000014e0: 2ce4 bc9a e8a2 abe6 b7bb e58a a0e5 88b0  ,...............
+000014f0: 4d41 4e49 4645 5354 e696 87e4 bbb6 e4b8  MANIFEST........
+00001500: ade3 8082 0d0a 2020 2020 2320 e5b8 8ce6  ......    # ....
+00001510: 9c9b e8a2 abe6 8993 e58c 85e7 9a84 e696  ................
+00001520: 87e4 bbb6 0d0a 2020 2020 7061 636b 6167  ......    packag
+00001530: 655f 6461 7461 3d7b 0d0a 2020 2020 2020  e_data={..      
+00001540: 2020 2727 3a5b 272a 2e74 7874 275d 2c0d    '':['*.txt'],.
+00001550: 0a20 2020 2020 2020 2027 6261 6e64 7769  .        'bandwi
+00001560: 6474 685f 7265 706f 7274 6572 273a 5b27  dth_reporter':['
+00001570: 2a2e 7478 7427 5d0d 0a20 2020 2020 2020  *.txt']..       
+00001580: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
+00001590: 2320 e4b8 8de6 8993 e58c 85e6 9f90 e4ba  # ..............
+000015a0: 9be6 9687 e4bb b60d 0a20 2020 2065 7863  .........    exc
+000015b0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+000015c0: 613d 7b0d 0a20 2020 2020 2020 2027 6261  a={..        'ba
+000015d0: 6e64 7769 6474 685f 7265 706f 7274 6572  ndwidth_reporter
+000015e0: 273a 5b27 2a2e 7478 7427 5d0d 0a20 2020  ':['*.txt']..   
+000015f0: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+00001600: 0a20 2020 2023 20e7 94a8 e69d a5e6 94af  .    # .........
+00001610: e68c 81e8 87aa e58a a8e7 949f e688 90e8  ................
+00001620: 849a e69c acef bc8c e5ae 89e8 a385 e590  ................
+00001630: 8ee4 bc9a e887 aae5 8aa8 e794 9fe6 8890  ................
+00001640: 202f 7573 722f 6269 6e2f 666f 6f20 e79a   /usr/bin/foo ..
+00001650: 84e5 8faf e689 a7e8 a18c e696 87e4 bbb6  ................
+00001660: 0d0a 2020 2020 2320 e8af a5e6 9687 e4bb  ..    # ........
+00001670: b6e5 85a5 e58f a3e6 8c87 e590 9120 666f  ............. fo
+00001680: 6f2f 6d61 696e 2e70 7920 e79a 846d 6169  o/main.py ...mai
+00001690: 6e20 e587 bde6 95b0 0d0a 2020 2020 656e  n ........    en
+000016a0: 7472 795f 706f 696e 7473 3d7b 0d0a 2020  try_points={..  
+000016b0: 2020 2020 2020 2763 6f6e 736f 6c65 5f73        'console_s
+000016c0: 6372 6970 7473 273a 205b 0d0a 2020 2020  cripts': [..    
+000016d0: 2020 2020 2020 2020 2766 6f6f 203d 2066          'foo = f
+000016e0: 6f6f 2e6d 6169 6e3a 6d61 696e 270d 0a20  oo.main:main'.. 
+000016f0: 2020 2020 2020 205d 0d0a 2020 2020 7d2c         ]..    },
+00001700: 0d0a 0d0a 2020 2020 2320 e5b0 8620 6269  ....    # ... bi
+00001710: 6e2f 666f 6f2e 7368 20e5 928c 2062 6172  n/foo.sh ... bar
+00001720: 2e70 7920 e884 9ae6 9cac efbc 8ce7 949f  .py ............
+00001730: e688 90e5 88b0 e7b3 bbe7 bb9f 2050 4154  ............ PAT
+00001740: 48e4 b8ad 0d0a 2020 2020 2320 e689 a7e8  H.....    # ....
+00001750: a18c 2070 7974 686f 6e20 7365 7475 702e  .. python setup.
+00001760: 7079 2069 6e73 7461 6c6c 20e5 908e 0d0a  py install .....
+00001770: 2020 2020 2320 e4bc 9ae7 949f e688 9020      # ......... 
+00001780: e5a6 8220 2f75 7372 2f62 696e 2f66 6f6f  ... /usr/bin/foo
+00001790: 2e73 6820 e592 8c20 e5a6 8220 2f75 7372  .sh ... ... /usr
+000017a0: 2f62 696e 2f62 6172 2e70 790d 0a20 2020  /bin/bar.py..   
+000017b0: 2073 6372 6970 7473 3d5b 2762 696e 2f66   scripts=['bin/f
+000017c0: 6f6f 2e73 6827 2c20 2762 6172 2e70 7927  oo.sh', 'bar.py'
+000017d0: 5d0d 0a27 2727 0d0a 0d0a 0d0a            ]..'''......
```

