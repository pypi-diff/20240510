# Comparing `tmp/mxlm-0.0.8.tar.gz` & `tmp/mxlm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxlm-0.0.8.tar", last modified: Thu May  9 09:33:30 2024, max compression
+gzip compressed data, was "mxlm-0.0.9.tar", last modified: Fri May 10 09:41:25 2024, max compression
```

## Comparing `mxlm-0.0.8.tar` & `mxlm-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-09 09:33:30.784721 mxlm-0.0.8/
--rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.8/MANIFEST.in
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-05-09 09:33:30.784721 mxlm-0.0.8/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)     1078 2024-04-10 04:01:47.000000 mxlm-0.0.8/README.md
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-09 09:33:30.780721 mxlm-0.0.8/mxlm/
--rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-05-09 09:33:10.000000 mxlm-0.0.8/mxlm/__info__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      308 2024-05-09 09:25:14.000000 mxlm-0.0.8/mxlm/__init__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     6134 2024-04-30 07:49:05.000000 mxlm-0.0.8/mxlm/chat_api.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2397 2024-04-10 03:59:44.000000 mxlm-0.0.8/mxlm/chatmd_utils.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2266 2024-04-30 07:52:39.000000 mxlm-0.0.8/mxlm/dialog_format_conversion.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      613 2024-05-08 10:07:35.000000 mxlm-0.0.8/mxlm/mxlm_utils.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      475 2024-05-09 09:23:49.000000 mxlm-0.0.8/mxlm/random_utils.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     1031 2024-05-09 09:23:49.000000 mxlm-0.0.8/mxlm/richtext.py
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-09 09:33:30.784721 mxlm-0.0.8/mxlm.egg-info/
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-05-09 09:33:30.000000 mxlm-0.0.8/mxlm.egg-info/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      348 2024-05-09 09:33:30.000000 mxlm-0.0.8/mxlm.egg-info/SOURCES.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-05-09 09:33:30.000000 mxlm-0.0.8/mxlm.egg-info/dependency_links.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-05-09 09:33:30.000000 mxlm-0.0.8/mxlm.egg-info/requires.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-05-09 09:33:30.000000 mxlm-0.0.8/mxlm.egg-info/top_level.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.8/requirements.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-05-09 09:33:30.784721 mxlm-0.0.8/setup.cfg
--rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.8/setup.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-10 09:41:25.433117 mxlm-0.0.9/
+-rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.9/MANIFEST.in
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-05-10 09:41:25.433117 mxlm-0.0.9/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)     1078 2024-04-10 04:01:47.000000 mxlm-0.0.9/README.md
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-10 09:41:25.429117 mxlm-0.0.9/mxlm/
+-rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-05-10 09:41:04.000000 mxlm-0.0.9/mxlm/__info__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      308 2024-05-09 09:25:14.000000 mxlm-0.0.9/mxlm/__init__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     6134 2024-04-30 07:49:05.000000 mxlm-0.0.9/mxlm/chat_api.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2397 2024-04-10 03:59:44.000000 mxlm-0.0.9/mxlm/chatmd_utils.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2266 2024-04-30 07:52:39.000000 mxlm-0.0.9/mxlm/dialog_format_conversion.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      781 2024-05-10 09:40:08.000000 mxlm-0.0.9/mxlm/mxlm_utils.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      475 2024-05-09 09:23:49.000000 mxlm-0.0.9/mxlm/random_utils.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     1031 2024-05-09 09:23:49.000000 mxlm-0.0.9/mxlm/richtext.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-10 09:41:25.433117 mxlm-0.0.9/mxlm.egg-info/
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-05-10 09:41:25.000000 mxlm-0.0.9/mxlm.egg-info/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      348 2024-05-10 09:41:25.000000 mxlm-0.0.9/mxlm.egg-info/SOURCES.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-05-10 09:41:25.000000 mxlm-0.0.9/mxlm.egg-info/dependency_links.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-05-10 09:41:25.000000 mxlm-0.0.9/mxlm.egg-info/requires.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-05-10 09:41:25.000000 mxlm-0.0.9/mxlm.egg-info/top_level.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.9/requirements.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-05-10 09:41:25.433117 mxlm-0.0.9/setup.cfg
+-rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.9/setup.py
```

### Comparing `mxlm-0.0.8/README.md` & `mxlm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.8/mxlm/__info__.py` & `mxlm-0.0.9/mxlm/__info__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __description__ = "Language Model Utils"
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `mxlm-0.0.8/mxlm/chat_api.py` & `mxlm-0.0.9/mxlm/chat_api.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.8/mxlm/chatmd_utils.py` & `mxlm-0.0.9/mxlm/chatmd_utils.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.8/mxlm/dialog_format_conversion.py` & `mxlm-0.0.9/mxlm/dialog_format_conversion.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.8/mxlm/mxlm_utils.py` & `mxlm-0.0.9/mxlm/mxlm_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 """
 Created on Fri Mar 29 16:15:58 2024
 
 @author: yl
 """
 
 
-def df_to_html(df, *args, max_width=400, **argkws):
+def df_to_html(df, *args, max_width=400, HTML_WIDTH_PER_CHAR=8, **argkws):
     """
     Pretty print DataFrame to html
     """
+    import html
+    import pprint
+
     if hasattr(df, "to_frame"):
         df = df.to_frame()
+
     argkws.setdefault(
         "formatters",
         {
             col: lambda x: f'<div style="max-width:{max_width}px;"><span style="white-space: pre-wrap; font-family: Monospace;">%s</span></div>'
-            % x
+            % html.escape(
+                pprint.pformat(x, indent=0, width=max_width // HTML_WIDTH_PER_CHAR)
+            )
             for col in df.columns
         },
     )
     argkws.setdefault("escape", False)
     return df.to_html(*args, **argkws)
```

### Comparing `mxlm-0.0.8/mxlm/richtext.py` & `mxlm-0.0.9/mxlm/richtext.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.8/setup.py` & `mxlm-0.0.9/setup.py`

 * *Files identical despite different names*

