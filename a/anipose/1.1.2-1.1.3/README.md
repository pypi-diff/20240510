# Comparing `tmp/anipose-1.1.2-py3-none-any.whl.zip` & `tmp/anipose-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 62089 bytes, number of entries: 30
--rw-r--r--  2.0 unx       81 b- defN 24-May-08 17:05 anipose/__init__.py
--rw-r--r--  2.0 unx    11071 b- defN 24-Apr-23 21:33 anipose/anipose.py
+Zip file size: 62088 bytes, number of entries: 30
+-rw-r--r--  2.0 unx       81 b- defN 24-May-10 17:58 anipose/__init__.py
+-rw-r--r--  2.0 unx    11056 b- defN 24-May-10 17:57 anipose/anipose.py
 -rw-rw-r--  2.0 unx     8201 b- defN 24-Jan-18 21:43 anipose/calibrate.py
 -rw-r--r--  2.0 unx    23543 b- defN 24-Jan-18 21:43 anipose/calibrate_extrinsics.py
 -rw-r--r--  2.0 unx    10564 b- defN 24-Jan-18 21:43 anipose/calibrate_intrinsics.py
 -rw-rw-r--  2.0 unx     6422 b- defN 24-Jan-18 21:43 anipose/calibration_errors.py
 -rw-r--r--  2.0 unx     6335 b- defN 24-Feb-02 17:45 anipose/common.py
 -rw-rw-r--  2.0 unx     5424 b- defN 24-Jan-18 21:43 anipose/compute_angles.py
 -rw-rw-r--  2.0 unx     2234 b- defN 24-Jan-18 21:43 anipose/convert_videos.py
@@ -19,14 +19,14 @@
 -rw-rw-r--  2.0 unx     2410 b- defN 24-Jan-18 21:43 anipose/pose_videos.py
 -rw-rw-r--  2.0 unx     5471 b- defN 24-Jan-18 21:43 anipose/project_2d.py
 -rw-rw-r--  2.0 unx    15061 b- defN 24-Jan-18 21:43 anipose/server.py
 -rw-r--r--  2.0 unx     4589 b- defN 24-Jan-18 21:43 anipose/summarize.py
 -rw-rw-r--  2.0 unx     6561 b- defN 24-Jan-18 21:43 anipose/tracking_errors.py
 -rw-rw-r--  2.0 unx     3275 b- defN 24-Jan-18 21:43 anipose/train_autoencoder.py
 -rw-rw-r--  2.0 unx    12392 b- defN 24-Jan-18 21:43 anipose/triangulate.py
--rw-r--r--  2.0 unx     1330 b- defN 24-May-08 17:12 anipose-1.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2424 b- defN 24-May-08 17:12 anipose-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 17:12 anipose-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 24-May-08 17:12 anipose-1.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-May-08 17:12 anipose-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2425 b- defN 24-May-08 17:12 anipose-1.1.2.dist-info/RECORD
-30 files, 202119 bytes uncompressed, 58247 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     1330 b- defN 24-May-10 17:58 anipose-1.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2424 b- defN 24-May-10 17:58 anipose-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 17:58 anipose-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 24-May-10 17:58 anipose-1.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-10 17:58 anipose-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2425 b- defN 24-May-10 17:58 anipose-1.1.3.dist-info/RECORD
+30 files, 202104 bytes uncompressed, 58246 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -66,26 +66,26 @@
 
 Filename: anipose/train_autoencoder.py
 Comment: 
 
 Filename: anipose/triangulate.py
 Comment: 
 
-Filename: anipose-1.1.2.dist-info/LICENSE
+Filename: anipose-1.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: anipose-1.1.2.dist-info/METADATA
+Filename: anipose-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: anipose-1.1.2.dist-info/WHEEL
+Filename: anipose-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: anipose-1.1.2.dist-info/entry_points.txt
+Filename: anipose-1.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: anipose-1.1.2.dist-info/top_level.txt
+Filename: anipose-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: anipose-1.1.2.dist-info/RECORD
+Filename: anipose-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anipose/__init__.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python3
 
 import sys
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 VERSION = __version__
```

## anipose/anipose.py

```diff
@@ -216,15 +216,15 @@
 @click.option('--scorer', default=None, type=str)
 @pass_config
 def extract_frames(config, nframes=200, mode='bad', no_pred=False, scorer=None):
     from .extract_frames import extract_frames_picked, extract_frames_random
     click.echo('Extracting frames...')
     if no_pred:
         mode = 'random'
-        extract_frames_random(config, nframes, scorer=scorer)
+        extract_frames_random(config, nframes)
     else:
         extract_frames_picked(config, mode, nframes, scorer=scorer)
 
 
 @cli.command()
 @pass_config
 def project_2d(config):
```

## Comparing `anipose-1.1.2.dist-info/LICENSE` & `anipose-1.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anipose-1.1.2.dist-info/METADATA` & `anipose-1.1.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipose
-Version: 1.1.2
+Version: 1.1.3
 Summary: Framework for scalable DeepLabCut based analysis including 3D tracking
 Home-page: https://github.com/lambdaloop/anipose
 Author: Lili Karashchuk
 Author-email: krchtchk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anipose Version: 1.1.2 Summary: Framework for
+Metadata-Version: 2.1 Name: anipose Version: 1.1.3 Summary: Framework for
 scalable DeepLabCut based analysis including 3D tracking Home-page: https://
 github.com/lambdaloop/anipose Author: Lili Karashchuk Author-email:
 krchtchk@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering Classifier: Topic
 :: Scientific/Engineering :: Image Recognition Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: deeplabcut >=2.0.4.1 Requires-
```

## Comparing `anipose-1.1.2.dist-info/RECORD` & `anipose-1.1.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-anipose/__init__.py,sha256=k05a336MZhVzb7XxLnBeI8gwDNQYKByndTFry70PdzQ,81
-anipose/anipose.py,sha256=cvoaaPQCRdckePt8je-KkAhYVZZi1et11Z0zX5CKK60,11071
+anipose/__init__.py,sha256=Q83v7sIIbnq5md2uKAUfqBX2xym1W9Bvwccr2rzB3M8,81
+anipose/anipose.py,sha256=JLUNXoPrgmasD-rqh9QnY9eJRLF6K1IjwJ6YRimLaMs,11056
 anipose/calibrate.py,sha256=VL0IdTZNNQm5K5vS7lBgEs3wmwI8nSSYwRybfpeUunI,8201
 anipose/calibrate_extrinsics.py,sha256=hbRzSigVDduo6011AMcur7gtLKjahC1AuKzurM-r6Ls,23543
 anipose/calibrate_intrinsics.py,sha256=tJfPctDMRDxdRPWBsxvqMquT57UH0IdrtXxgK3fAnxc,10564
 anipose/calibration_errors.py,sha256=7-n1CbFFl_LbXVB9eTuvKWtQy2MggMqjS7WGJPTqlm0,6422
 anipose/common.py,sha256=m7zHopwsHUjgIKhNCJJ8Zx_dZgiPj5NwDp4ZPeEsz2s,6335
 anipose/compute_angles.py,sha256=ctg79yAy4-c4-JfFlFx8m8heUUak7aYeIJ9Nt5gFDQw,5424
 anipose/convert_videos.py,sha256=QrNQyIIulQJ66Fju4QyC7LZ7WiK_SOvjFK5zErfjdlg,2234
@@ -18,13 +18,13 @@
 anipose/pose_videos.py,sha256=CFl-dOknV-_vM9naEfXfI13HVu8Hiz6tXXSnzQrTtqc,2410
 anipose/project_2d.py,sha256=i3lKolt6BNma0zSSjkvfEUIEglJDiU_IzAi25xovcRM,5471
 anipose/server.py,sha256=avIUsoFW6SOtTUOuWxTiimfVRkRKMXe3-r_0uZWnRY4,15061
 anipose/summarize.py,sha256=B5eqGnCepW0EzX0mAnq42j3ScQZUj8JgwWt5ovznKkE,4589
 anipose/tracking_errors.py,sha256=3ks1lvXNK-IcE51MOkjijclGNqPlgIQE_X54Bcn4ecI,6561
 anipose/train_autoencoder.py,sha256=cSkwCAswADh8ZGkBujWI9-eohMCab5tJqgtEAoXX8AI,3275
 anipose/triangulate.py,sha256=l2Y4EbnRfKBMGrZPuo1jKNs3Vf-hMOvJT5Tj7s2Ycos,12392
-anipose-1.1.2.dist-info/LICENSE,sha256=AfvLrmS8RH6Isfu5u7W5lzQkUVBfk7aCJD8PoyZkcds,1330
-anipose-1.1.2.dist-info/METADATA,sha256=z2Bq85gEweVoHrC2blutigQWwcpE76JCh--8nAlPk04,2424
-anipose-1.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-anipose-1.1.2.dist-info/entry_points.txt,sha256=9U_1s6jd3fJsRKzlsdIXJIa9DtM0e2_PgiHbVBVYCKk,48
-anipose-1.1.2.dist-info/top_level.txt,sha256=stUtz0rFsogmTXteoL99dNEgerWeBJ6O5MagnO_O2NQ,8
-anipose-1.1.2.dist-info/RECORD,,
+anipose-1.1.3.dist-info/LICENSE,sha256=AfvLrmS8RH6Isfu5u7W5lzQkUVBfk7aCJD8PoyZkcds,1330
+anipose-1.1.3.dist-info/METADATA,sha256=7wMsC1DWF9jMtjEOmpbIyBLDk4JkEFTIORpy_WdcEHY,2424
+anipose-1.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+anipose-1.1.3.dist-info/entry_points.txt,sha256=9U_1s6jd3fJsRKzlsdIXJIa9DtM0e2_PgiHbVBVYCKk,48
+anipose-1.1.3.dist-info/top_level.txt,sha256=stUtz0rFsogmTXteoL99dNEgerWeBJ6O5MagnO_O2NQ,8
+anipose-1.1.3.dist-info/RECORD,,
```

