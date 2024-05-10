# Comparing `tmp/CUCMLib-0.1.7-py3-none-any.whl.zip` & `tmp/CUCMLib-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 311075 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat   834720 b- defN 24-Feb-23 10:54 CUCMLib/AXLAPI.wsdl
 -rw-rw-rw-  2.0 fat   141548 b- defN 24-Feb-23 10:54 CUCMLib/AXLEnums.xsd
 -rw-rw-rw-  2.0 fat  3700703 b- defN 24-Feb-23 10:54 CUCMLib/AXLSoap.xsd
 -rw-rw-rw-  2.0 fat     1357 b- defN 24-Feb-28 08:11 CUCMLib/__init__.py
--rw-rw-rw-  2.0 fat     7988 b- defN 24-Feb-28 08:06 CUCMLib/partition.py
--rw-rw-rw-  2.0 fat    13892 b- defN 24-Feb-28 08:06 CUCMLib/phone.py
--rw-rw-rw-  2.0 fat      696 b- defN 24-Mar-20 10:45 CUCMLib-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-20 10:45 CUCMLib-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-20 10:45 CUCMLib-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      759 b- defN 24-Mar-20 10:45 CUCMLib-0.1.7.dist-info/RECORD
-10 files, 4701763 bytes uncompressed, 309811 bytes compressed:  93.4%
+-rw-rw-rw-  2.0 fat     8004 b- defN 24-May-10 13:44 CUCMLib/partition.py
+-rw-rw-rw-  2.0 fat    13894 b- defN 24-May-10 13:44 CUCMLib/phone.py
+-rw-rw-rw-  2.0 fat      696 b- defN 24-May-10 14:05 CUCMLib-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 14:05 CUCMLib-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-10 14:05 CUCMLib-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      759 b- defN 24-May-10 14:05 CUCMLib-0.1.8.dist-info/RECORD
+10 files, 4701781 bytes uncompressed, 309811 bytes compressed:  93.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: CUCMLib/partition.py
 Comment: 
 
 Filename: CUCMLib/phone.py
 Comment: 
 
-Filename: CUCMLib-0.1.7.dist-info/METADATA
+Filename: CUCMLib-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: CUCMLib-0.1.7.dist-info/WHEEL
+Filename: CUCMLib-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: CUCMLib-0.1.7.dist-info/top_level.txt
+Filename: CUCMLib-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: CUCMLib-0.1.7.dist-info/RECORD
+Filename: CUCMLib-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## CUCMLib/partition.py

```diff
@@ -1,7 +1,9 @@
+
+
 from requests import Session
 from zeep import Client
 from zeep.transports import Transport
 from urllib3 import disable_warnings
 from urllib3.exceptions import InsecureRequestWarning
 from zeep.cache import SqliteCache
 from zeep.plugins import HistoryPlugin
@@ -207,8 +209,11 @@
     print("""
     Bu kütüphane ile CUCM'da bulunan partition bilgilerini, bulunduğu klasöre CSV formatında kaydetmektedir.
     
     Kaydedilen bilgiler : Name  -  Description
           
     Bu bilgiler haricinde bulunan bilgiler yazılmamaktadır.
     
-    """)
+    """)
+    
+
+
```

## CUCMLib/phone.py

```diff
@@ -1,7 +1,8 @@
+
 from requests import Session
 from zeep import Client
 from zeep.transports import Transport
 from urllib3 import disable_warnings
 from urllib3.exceptions import InsecureRequestWarning
 from zeep.cache import SqliteCache
 from zeep.plugins import HistoryPlugin
```

## Comparing `CUCMLib-0.1.7.dist-info/METADATA` & `CUCMLib-0.1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUCMLib
-Version: 0.1.7
+Version: 0.1.8
 Summary: CUCM ile etkileşim için bir kütüphane
 Author: SafaBasdemir
 Author-email: safabasdemir@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

## Comparing `CUCMLib-0.1.7.dist-info/RECORD` & `CUCMLib-0.1.8.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 CUCMLib/AXLAPI.wsdl,sha256=gPqFmncX240OedlZirYSWcR_HIdFsHas2dIRvaqed1s,834720
 CUCMLib/AXLEnums.xsd,sha256=LT8ESfu2PAPa1ZfzGELJP4P-uScGO9uQF3dQeH6kVBA,141548
 CUCMLib/AXLSoap.xsd,sha256=h-oWyJ7NVgkNcsceufrULsd-_RmJUZut08EW6YXf_tQ,3700703
 CUCMLib/__init__.py,sha256=pVr6upBQO3sMKvXdh71ztxBhwFJvKjfO5L52EBujVe4,1357
-CUCMLib/partition.py,sha256=8nrxqUuBx3aZSKuvIwpWPuCMff-rewpMdPVYPKDkF-o,7988
-CUCMLib/phone.py,sha256=-M3LJOGmjwg3c2m8JSqLIUofRdUd2LHroCUmk8P3LEQ,13892
-CUCMLib-0.1.7.dist-info/METADATA,sha256=WbislZnaGOxM-Odcnkz4S-ADP_LfrLILTlpbZP4jg20,696
-CUCMLib-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-CUCMLib-0.1.7.dist-info/top_level.txt,sha256=_rcYt5-3coRlGMzaEcbkEoI89IBM2CuO5ZUhLrR44CE,8
-CUCMLib-0.1.7.dist-info/RECORD,,
+CUCMLib/partition.py,sha256=Fc7biIYh5xYfWToxSwh3lB28K68JUfkG02y75C3s8jE,8004
+CUCMLib/phone.py,sha256=poHBb9Bgk7SUeKNsC3TKnbi1rd2hi53696WTJ6WvFqg,13894
+CUCMLib-0.1.8.dist-info/METADATA,sha256=2WwZlwHwgm27bRs4qQnQSqWLZD1ZnJJqI7VsfWZBxAw,696
+CUCMLib-0.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+CUCMLib-0.1.8.dist-info/top_level.txt,sha256=_rcYt5-3coRlGMzaEcbkEoI89IBM2CuO5ZUhLrR44CE,8
+CUCMLib-0.1.8.dist-info/RECORD,,
```

