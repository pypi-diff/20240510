# Comparing `tmp/libhum-1.1.3-py3-none-any.whl.zip` & `tmp/libhum-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 63657 bytes, number of entries: 15
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-13 11:02 libhum/__init__.py
+Zip file size: 63761 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       22 b- defN 24-May-10 14:10 libhum/__init__.py
 -rw-r--r--  2.0 unx    19661 b- defN 23-Nov-09 14:38 libhum/analysis.py
--rw-r--r--  2.0 unx     9843 b- defN 24-Mar-13 11:02 libhum/io.py
+-rw-r--r--  2.0 unx    10039 b- defN 24-May-10 14:09 libhum/io.py
 -rw-r--r--  2.0 unx     4632 b- defN 24-Jan-11 21:30 libhum/main.py
 -rw-r--r--  2.0 unx     6878 b- defN 23-Oct-07 22:24 libhum/match.kernel
 -rw-r--r--  2.0 unx    18405 b- defN 24-Jan-08 15:10 libhum/match.py
 -rw-r--r--  2.0 unx   112707 b- defN 24-Jan-08 14:36 libhum/match_score_regressor.pickle
 -rw-r--r--  2.0 unx     3684 b- defN 23-May-05 22:58 libhum/merge.py
 -rw-r--r--  2.0 unx     8381 b- defN 23-Dec-02 21:18 libhum/types.py
--rw-r--r--  2.0 unx     7652 b- defN 24-Mar-13 11:04 libhum-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    11957 b- defN 24-Mar-13 11:04 libhum-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-13 11:04 libhum-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-Mar-13 11:04 libhum-1.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-13 11:04 libhum-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1151 b- defN 24-Mar-13 11:04 libhum-1.1.3.dist-info/RECORD
-15 files, 205116 bytes uncompressed, 61787 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx     7652 b- defN 24-May-10 14:12 libhum-1.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11957 b- defN 24-May-10 14:12 libhum-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 14:12 libhum-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-10 14:12 libhum-1.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-May-10 14:12 libhum-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1152 b- defN 24-May-10 14:12 libhum-1.1.4.dist-info/RECORD
+15 files, 205313 bytes uncompressed, 61891 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: libhum/merge.py
 Comment: 
 
 Filename: libhum/types.py
 Comment: 
 
-Filename: libhum-1.1.3.dist-info/LICENSE
+Filename: libhum-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: libhum-1.1.3.dist-info/METADATA
+Filename: libhum-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: libhum-1.1.3.dist-info/WHEEL
+Filename: libhum-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: libhum-1.1.3.dist-info/entry_points.txt
+Filename: libhum-1.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: libhum-1.1.3.dist-info/top_level.txt
+Filename: libhum-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: libhum-1.1.3.dist-info/RECORD
+Filename: libhum-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libhum/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.3"
+__version__ = "1.1.4"
```

## libhum/io.py

```diff
@@ -108,15 +108,21 @@
 
     See https://www.swissgrid.ch/en/home/operation/grid-data/current-data.html
     """
 
     swiss_tz = ZoneInfo("Europe/Zurich")
     network_frequency = 50.0
 
-    resp = requests.get(url)
+    # Makes the request as Firefox
+    headers = {
+        "User-Agent":
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:124.0) Gecko/20100101 Firefox/124.0"
+    }
+
+    resp = requests.get(url, headers=headers)
     resp.raise_for_status()
 
     values = resp.json()["data"]["series"][0]["data"]
 
     def parse_swiss_grid_value(timestamp: int, enf: float):
         local_dt = datetime.utcfromtimestamp(timestamp / 1000).replace(tzinfo=swiss_tz)
         utc_dt = local_dt.astimezone(timezone.utc)
```

## Comparing `libhum-1.1.3.dist-info/LICENSE` & `libhum-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libhum-1.1.3.dist-info/METADATA` & `libhum-1.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libhum
-Version: 1.1.3
+Version: 1.1.4
 Summary: Libhum is a Python GPU-accelerated library to extract and compare Electricity Frequency Signals (ENF)
 Author-email: Raphael Javaux <raphael@noisycamp.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

## Comparing `libhum-1.1.3.dist-info/RECORD` & `libhum-1.1.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-libhum/__init__.py,sha256=u9ExJqoMv3fQc8WmLTw4I2FnQo6u4xRrBc6DLy6G1IE,22
+libhum/__init__.py,sha256=XxXhu8-QnuD9hA8Ah0WX5rgpt_DwOQmAwcK-FtpngyQ,22
 libhum/analysis.py,sha256=wrg-cjA3ey7dCTfrx3yQnbgXvS3O4Qc2fJKTYFPoSdw,19661
-libhum/io.py,sha256=5hQeP_h87UCM-5xxyD4rykiCBrCZ0WvpGq29DrmzOkw,9843
+libhum/io.py,sha256=pzFzE4m5OXOte4iaoypmxAVWi1S14GYqjDm1rO2vX30,10039
 libhum/main.py,sha256=iML71NkPIQMNnKB8Y37gIQBpATgUTUYOaKOkLMJK1pE,4632
 libhum/match.kernel,sha256=-FK2Erl95NQo2sLKILMnS4MeBb3MXuL7hIaiOvecVR0,6878
 libhum/match.py,sha256=etP-eV6pWinxe7zjY5-SLyOWPg_X_ShQWUJutCOgIv4,18405
 libhum/match_score_regressor.pickle,sha256=YW2o2XWSgbZ5BDQOIwG5npRfwFlU1rWx7UsCnRDpD6E,112707
 libhum/merge.py,sha256=KkvmWxKc8E27b0aVoh1-5o29en-Lm76B4_m1htcKixw,3684
 libhum/types.py,sha256=b_eFkik4awgukXbw1rEcwc7yHJYBSTmhIWN84eURwUo,8381
-libhum-1.1.3.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
-libhum-1.1.3.dist-info/METADATA,sha256=_B6XW5VPKF6Bj2guj9XYuL4isONO058Jmqn2F8CJ0fk,11957
-libhum-1.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-libhum-1.1.3.dist-info/entry_points.txt,sha256=xfYDpMbZnq673DPqXfaUkmzoErHhkTnoZAOXE6phyxs,44
-libhum-1.1.3.dist-info/top_level.txt,sha256=7Fp6N-Myc79I4TnhFhqgY2FXFb7UbK86oFPIdtLktBM,7
-libhum-1.1.3.dist-info/RECORD,,
+libhum-1.1.4.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
+libhum-1.1.4.dist-info/METADATA,sha256=cjx-NBvfOT2bXkgCYaV0fPMePca80v8hn-ZBZUerRFo,11957
+libhum-1.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libhum-1.1.4.dist-info/entry_points.txt,sha256=xfYDpMbZnq673DPqXfaUkmzoErHhkTnoZAOXE6phyxs,44
+libhum-1.1.4.dist-info/top_level.txt,sha256=7Fp6N-Myc79I4TnhFhqgY2FXFb7UbK86oFPIdtLktBM,7
+libhum-1.1.4.dist-info/RECORD,,
```

