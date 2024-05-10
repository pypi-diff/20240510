# Comparing `tmp/mdxcanvas-0.1.4.tar.gz` & `tmp/mdxcanvas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxcanvas-0.1.4.tar", max compression
+gzip compressed data, was "mdxcanvas-0.1.5.tar", max compression
```

## Comparing `mdxcanvas-0.1.4.tar` & `mdxcanvas-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2024-01-31 20:08:12.653583 mdxcanvas-0.1.4/LICENSE
--rw-r--r--   0        0        0      156 2024-02-23 19:51:14.711484 mdxcanvas-0.1.4/mdxcanvas/__init__.py
--rw-r--r--   0        0        0    20789 2024-04-23 21:55:26.002491 mdxcanvas-0.1.4/mdxcanvas/canvas_creator.py
--rw-r--r--   0        0        0      914 2024-04-23 21:43:27.025380 mdxcanvas-0.1.4/mdxcanvas/deploy.py
--rw-r--r--   0        0        0     3393 2024-04-23 21:59:22.722245 mdxcanvas-0.1.4/mdxcanvas/document_schema.py
--rw-r--r--   0        0        0      873 2024-02-26 20:43:38.531257 mdxcanvas-0.1.4/mdxcanvas/extensions.py
--rw-r--r--   0        0        0     2689 2024-04-22 22:07:08.576782 mdxcanvas-0.1.4/mdxcanvas/jinja_parser.py
--rw-r--r--   0        0        0    25451 2024-04-23 21:57:23.356381 mdxcanvas-0.1.4/mdxcanvas/parser.py
--rw-r--r--   0        0        0      559 2024-04-22 22:07:08.577386 mdxcanvas-0.1.4/mdxcanvas/question_schema.py
--rw-r--r--   0        0        0     1878 2024-04-22 22:07:08.577697 mdxcanvas-0.1.4/mdxcanvas/templating.py
--rw-r--r--   0        0        0    15263 2024-04-23 21:58:15.572059 mdxcanvas-0.1.4/mdxcanvas/yaml_parser.py
--rw-r--r--   0        0        0      651 2024-04-23 21:59:31.615699 mdxcanvas-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 mdxcanvas-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 01:39:54.971696 mdxcanvas-0.1.5/LICENSE
+-rw-r--r--   0        0        0      156 2024-04-08 01:39:54.980858 mdxcanvas-0.1.5/mdxcanvas/__init__.py
+-rw-r--r--   0        0        0    20789 2024-05-08 23:33:02.372283 mdxcanvas-0.1.5/mdxcanvas/canvas_creator.py
+-rw-r--r--   0        0        0     1053 2024-05-09 01:17:42.872976 mdxcanvas-0.1.5/mdxcanvas/deploy.py
+-rw-r--r--   0        0        0     3393 2024-05-08 23:33:02.371732 mdxcanvas-0.1.5/mdxcanvas/document_schema.py
+-rw-r--r--   0        0        0      873 2024-04-08 01:39:54.981405 mdxcanvas-0.1.5/mdxcanvas/extensions.py
+-rw-r--r--   0        0        0     2689 2024-04-22 22:03:40.203135 mdxcanvas-0.1.5/mdxcanvas/jinja_parser.py
+-rw-r--r--   0        0        0    25451 2024-05-09 01:17:42.874201 mdxcanvas-0.1.5/mdxcanvas/parser.py
+-rw-r--r--   0        0        0      559 2024-04-12 20:46:23.699994 mdxcanvas-0.1.5/mdxcanvas/question_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-09 16:04:59.850313 mdxcanvas-0.1.5/mdxcanvas/templating.py
+-rw-r--r--   0        0        0    15263 2024-05-08 23:33:02.371585 mdxcanvas-0.1.5/mdxcanvas/yaml_parser.py
+-rw-r--r--   0        0        0      651 2024-05-09 01:06:24.390161 mdxcanvas-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 mdxcanvas-0.1.5/PKG-INFO
```

### Comparing `mdxcanvas-0.1.4/LICENSE` & `mdxcanvas-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/canvas_creator.py` & `mdxcanvas-0.1.5/mdxcanvas/canvas_creator.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/deploy.py` & `mdxcanvas-0.1.5/mdxcanvas/deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,20 @@
     parser.add_argument("filename", type=Path)
     parser.add_argument("--course-info", type=Path, default="canvas_course_info.json")
     args = parser.parse_args()
 
     with open(args.course_info) as f:
         course_settings = json.load(f)
 
+    api_token = os.environ.get("CANVAS_API_TOKEN")
+    if api_token is None:
+        raise ValueError("Please set the CANVAS_API_TOKEN environment variable")
+
     main(api_url=course_settings["CANVAS_API_URL"],
-         api_token=os.getenv("CANVAS_API_TOKEN"),
+         api_token=api_token,
          course_id=course_settings["CANVAS_COURSE_ID"],
          time_zone=course_settings["LOCAL_TIME_ZONE"],
          file_path=args.filename)
 
 
 if __name__ == '__main__':
     entry()
```

### Comparing `mdxcanvas-0.1.4/mdxcanvas/document_schema.py` & `mdxcanvas-0.1.5/mdxcanvas/document_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/extensions.py` & `mdxcanvas-0.1.5/mdxcanvas/extensions.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/jinja_parser.py` & `mdxcanvas-0.1.5/mdxcanvas/jinja_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/parser.py` & `mdxcanvas-0.1.5/mdxcanvas/parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/question_schema.py` & `mdxcanvas-0.1.5/mdxcanvas/question_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/templating.py` & `mdxcanvas-0.1.5/mdxcanvas/templating.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/mdxcanvas/yaml_parser.py` & `mdxcanvas-0.1.5/mdxcanvas/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.4/pyproject.toml` & `mdxcanvas-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdxcanvas"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Canvas LMS API wrapper for maintaining content in markdown"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Preston Raab <phr23@byu.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.1.2"
```

### Comparing `mdxcanvas-0.1.4/PKG-INFO` & `mdxcanvas-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mdxcanvas
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Canvas LMS API wrapper for maintaining content in markdown
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: CanvasAPI (>=3.2.0,<4.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: Markdown (>=3.1.1,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.0.1,<3.0.0)
 Requires-Dist: Pygments (>=2.17.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.0,<5.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
```

