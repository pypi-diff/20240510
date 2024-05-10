# Comparing `tmp/a2y_ats-1.2.1-cp38-cp38-win_amd64.whl.zip` & `tmp/a2y_ats-1.2.2-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 355008 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   925184 b- defN 24-May-07 16:01 a2y_ats.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat      718 b- defN 24-May-07 16:01 a2y_ats-1.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1097 b- defN 24-May-07 16:01 a2y_ats-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-07 16:01 a2y_ats-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-07 16:01 a2y_ats-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      470 b- defN 24-May-07 16:01 a2y_ats-1.2.1.dist-info/RECORD
-6 files, 927577 bytes uncompressed, 354160 bytes compressed:  61.8%
+Zip file size: 377600 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat  1007616 b- defN 24-May-10 14:37 a2y_ats.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      704 b- defN 24-May-10 14:37 a2y_ats-1.2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1168 b- defN 24-May-10 14:37 a2y_ats-1.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-10 14:37 a2y_ats-1.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-10 14:37 a2y_ats-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      471 b- defN 24-May-10 14:37 a2y_ats-1.2.2.dist-info/RECORD
+6 files, 1010067 bytes uncompressed, 376752 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: a2y_ats.cp38-win_amd64.pyd
 Comment: 
 
-Filename: a2y_ats-1.2.1.dist-info/LICENSE
+Filename: a2y_ats-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: a2y_ats-1.2.1.dist-info/METADATA
+Filename: a2y_ats-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: a2y_ats-1.2.1.dist-info/WHEEL
+Filename: a2y_ats-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: a2y_ats-1.2.1.dist-info/top_level.txt
+Filename: a2y_ats-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: a2y_ats-1.2.1.dist-info/RECORD
+Filename: a2y_ats-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `a2y_ats-1.2.1.dist-info/LICENSE` & `a2y_ats-1.2.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-This is private software.
-
-Anyone without authorization is NOT allowed to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
+This is private software.
+
+Anyone without authorization is NOT allowed to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `a2y_ats-1.2.1.dist-info/METADATA` & `a2y_ats-1.2.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: a2y-ats
-Version: 1.2.1
+Version: 1.2.2
 Summary: A module that implements an Auto Test System.
 Home-page: http://www.sorobust.com/a2y/ats.html
 Author: Yu Han
 Author-email: hanjunyu@163.com
 License: Private
 Platform: Windows
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Educational Use
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: a2y-atsui >=0.9.6
 Requires-Dist: a2y-wxtools
 Requires-Dist: a2y-testparameters
 Requires-Dist: a2y-paratree
 Requires-Dist: a2y-handy
 Requires-Dist: a2y-matplot
 Requires-Dist: a2y-touch
@@ -27,7 +26,10 @@
 
 # Python Module: a2y_ats
 a2y_ats模块提供一个自动化测试框架。
 
 ## ChangeLog
 2024-05-07 尝试使用新版实现，修正一些发现的 bug。
 从版本 1.2.0 开始建议只在 Python3.8或以上版本中使用。
+
+2024-05-10 给 ATSFrame 加入 cells 和 get_cell 成员，以方便访问各个 cell。
+
```

