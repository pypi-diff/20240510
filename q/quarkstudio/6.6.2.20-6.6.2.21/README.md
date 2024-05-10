# Comparing `tmp/quarkstudio-6.6.2.20-cp312-none-win_amd64.whl.zip` & `tmp/quarkstudio-6.6.2.21-cp312-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,10 @@
-Zip file size: 264177 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-26 05:22 quarkstudio-6.6.2.20.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3211 b- defN 24-Apr-26 05:22 quarkstudio-6.6.2.20.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-26 05:22 quarkstudio-6.6.2.20.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       37 b- defN 24-Apr-26 05:22 quarkstudio-6.6.2.20.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-26 05:22 quarkstudio-6.6.2.20.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      523 b- defN 24-Apr-26 05:22 quarkstudio-6.6.2.20.dist-info/RECORD
--rw-rw-rw-  2.0 fat   192000 b- defN 24-Apr-26 05:22 quark/__init__.pyd
--rw-rw-rw-  2.0 fat   314368 b- defN 24-Apr-26 05:22 quark/cloud.pyd
--rw-rw-rw-  2.0 fat    77312 b- defN 24-Apr-26 05:22 quark/setting.pyd
--rw-rw-rw-  2.0 fat    18944 b- defN 24-Apr-26 05:22 quark/token.pyd
-10 files, 607581 bytes uncompressed, 262783 bytes compressed:  56.7%
+Zip file size: 120049 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     1084 b- defN 24-May-10 12:17 quarkstudio-6.6.2.21.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3202 b- defN 24-May-10 12:17 quarkstudio-6.6.2.21.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-10 12:17 quarkstudio-6.6.2.21.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       37 b- defN 24-May-10 12:17 quarkstudio-6.6.2.21.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-10 12:17 quarkstudio-6.6.2.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      523 b- defN 24-May-10 12:17 quarkstudio-6.6.2.21.dist-info/RECORD
+-rw-rw-rw-  2.0 fat   190976 b- defN 24-May-10 12:17 quark/__init__.pyd
+-rw-rw-rw-  2.0 fat    76800 b- defN 24-May-10 12:17 quark/setting.pyd
+8 files, 272723 bytes uncompressed, 118867 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,31 +1,25 @@
-Filename: quarkstudio-6.6.2.20.dist-info/LICENSE
+Filename: quarkstudio-6.6.2.21.dist-info/LICENSE
 Comment: 
 
-Filename: quarkstudio-6.6.2.20.dist-info/METADATA
+Filename: quarkstudio-6.6.2.21.dist-info/METADATA
 Comment: 
 
-Filename: quarkstudio-6.6.2.20.dist-info/WHEEL
+Filename: quarkstudio-6.6.2.21.dist-info/WHEEL
 Comment: 
 
-Filename: quarkstudio-6.6.2.20.dist-info/entry_points.txt
+Filename: quarkstudio-6.6.2.21.dist-info/entry_points.txt
 Comment: 
 
-Filename: quarkstudio-6.6.2.20.dist-info/top_level.txt
+Filename: quarkstudio-6.6.2.21.dist-info/top_level.txt
 Comment: 
 
-Filename: quarkstudio-6.6.2.20.dist-info/RECORD
+Filename: quarkstudio-6.6.2.21.dist-info/RECORD
 Comment: 
 
 Filename: quark/__init__.pyd
 Comment: 
 
-Filename: quark/cloud.pyd
-Comment: 
-
 Filename: quark/setting.pyd
 Comment: 
 
-Filename: quark/token.pyd
-Comment: 
-
 Zip file comment:
```

## Comparing `quarkstudio-6.6.2.20.dist-info/LICENSE` & `quarkstudio-6.6.2.21.dist-info/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `quarkstudio-6.6.2.20.dist-info/METADATA` & `quarkstudio-6.6.2.21.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: quarkstudio
-Version: 6.6.2.20
+Version: 6.6.2.21
 Summary: description
 Author-email: YL <fengyl@pku.edu.cn>
 License: MIT License
         
         Copyright (c) 2021 YL Feng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
         
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: homepage, https://gitee.com
 Project-URL: documentation, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `quarkstudio-6.6.2.20.dist-info/RECORD` & `quarkstudio-6.6.2.21.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-quarkstudio-6.6.2.20.dist-info/LICENSE,sha256=C3Kj30P434KPtlRtTmqw8y310egFxXCp0sXadioePRs,1085
-quarkstudio-6.6.2.20.dist-info/METADATA,sha256=gKTdWkR4Vv1XlklHeWL2fVEX-gOnpRKacFjXg33ZlWo,3211
-quarkstudio-6.6.2.20.dist-info/WHEEL,sha256=vLgnepztXPsaByH9QO8ZgGMjYc7001FVO4ktiG-h8c0,100
-quarkstudio-6.6.2.20.dist-info/entry_points.txt,sha256=FeCgtGnAYHTU1GLSewHuHpp2BtExfrjz72bSRGWGfAc,37
-quarkstudio-6.6.2.20.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-quarkstudio-6.6.2.20.dist-info/RECORD,,
+quarkstudio-6.6.2.21.dist-info/LICENSE,sha256=kYK8AINBBnuUY-tXKz9wHOoNoLzg9ZmAAYbM82WJykE,1084
+quarkstudio-6.6.2.21.dist-info/METADATA,sha256=cLikbi4E08yzlqHNNbjDS35EF3PNMwHsxgqFUc4EuZw,3202
+quarkstudio-6.6.2.21.dist-info/WHEEL,sha256=b561VlO0FFA36s33ZiAcL1tul3l99V87_PXMBl3xyiU,100
+quarkstudio-6.6.2.21.dist-info/entry_points.txt,sha256=FeCgtGnAYHTU1GLSewHuHpp2BtExfrjz72bSRGWGfAc,37
+quarkstudio-6.6.2.21.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+quarkstudio-6.6.2.21.dist-info/RECORD,,
```

