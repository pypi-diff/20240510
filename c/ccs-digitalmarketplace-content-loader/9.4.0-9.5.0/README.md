# Comparing `tmp/ccs-digitalmarketplace-content-loader-9.4.0.tar.gz` & `tmp/ccs-digitalmarketplace-content-loader-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-content-loader-9.4.0.tar", last modified: Thu Sep 28 08:18:11 2023, max compression
+gzip compressed data, was "ccs-digitalmarketplace-content-loader-9.5.0.tar", last modified: Mon Oct  9 14:05:25 2023, max compression
```

## Comparing `ccs-digitalmarketplace-content-loader-9.4.0.tar` & `ccs-digitalmarketplace-content-loader-9.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 08:18:11.986880 ccs-digitalmarketplace-content-loader-9.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-09-28 08:18:11.986880 ccs-digitalmarketplace-content-loader-9.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 08:18:11.986880 ccs-digitalmarketplace-content-loader-9.4.0/ccs_digitalmarketplace_content_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-09-28 08:18:11.000000 ccs-digitalmarketplace-content-loader-9.4.0/ccs_digitalmarketplace_content_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-09-28 08:18:11.000000 ccs-digitalmarketplace-content-loader-9.4.0/ccs_digitalmarketplace_content_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 08:18:11.000000 ccs-digitalmarketplace-content-loader-9.4.0/ccs_digitalmarketplace_content_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-09-28 08:18:11.000000 ccs-digitalmarketplace-content-loader-9.4.0/ccs_digitalmarketplace_content_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-28 08:18:11.000000 ccs-digitalmarketplace-content-loader-9.4.0/ccs_digitalmarketplace_content_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 08:18:11.986880 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27372 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/content_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    23277 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/govuk_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    34583 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-09-28 08:18:11.986880 ccs-digitalmarketplace-content-loader-9.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-09-28 08:18:01.000000 ccs-digitalmarketplace-content-loader-9.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 14:05:25.104076 ccs-digitalmarketplace-content-loader-9.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-09 14:05:25.104076 ccs-digitalmarketplace-content-loader-9.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 14:05:25.100076 ccs-digitalmarketplace-content-loader-9.5.0/ccs_digitalmarketplace_content_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-09 14:05:25.000000 ccs-digitalmarketplace-content-loader-9.5.0/ccs_digitalmarketplace_content_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2023-10-09 14:05:25.000000 ccs-digitalmarketplace-content-loader-9.5.0/ccs_digitalmarketplace_content_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 14:05:25.000000 ccs-digitalmarketplace-content-loader-9.5.0/ccs_digitalmarketplace_content_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-09 14:05:25.000000 ccs-digitalmarketplace-content-loader-9.5.0/ccs_digitalmarketplace_content_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-09 14:05:25.000000 ccs-digitalmarketplace-content-loader-9.5.0/ccs_digitalmarketplace_content_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 14:05:25.104076 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27372 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/content_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23277 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/govuk_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34583 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-09 14:05:25.104076 ccs-digitalmarketplace-content-loader-9.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-10-09 14:05:12.000000 ccs-digitalmarketplace-content-loader-9.5.0/setup.py
```

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/LICENCE` & `ccs-digitalmarketplace-content-loader-9.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/README.md` & `ccs-digitalmarketplace-content-loader-9.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/ccs_digitalmarketplace_content_loader.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-content-loader-9.5.0/ccs_digitalmarketplace_content_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/content_loader.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/content_loader.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/converters.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/converters.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/formats.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/formats.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/govuk_frontend.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/govuk_frontend.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/html.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/html.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/markdown.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/markdown.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/messages.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/messages.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/metadata.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/metadata.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/questions.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/questions.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/dmcontent/utils.py` & `ccs-digitalmarketplace-content-loader-9.5.0/dmcontent/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,26 +100,39 @@
     For multiquestions that are serialized to separate top-level keys we set the follow-up value
     to `None`, so that it's replaced if the question was previously answered with a follow-up.
 
     """
 
     data = data.copy()
 
+    fields = {
+        "pop": set(),
+        "keep": set(),
+    }
+
     for question in question_or_section.questions:
         for followup_id, values in question.get('followup', {}).items():
             question_data = data.get(question.id)
             if not isinstance(question_data, list):
                 question_data = [question_data]
 
             if not set(question_data) & set(values):
-                for field in question_or_section.get_question(followup_id).form_fields:
-                    if nested:
-                        data.pop(field, None)
-                    else:
-                        data[field] = None
+                fields_key = "pop"
+            else:
+                fields_key = "keep"
+
+            for field in question_or_section.get_question(followup_id).form_fields:
+                fields[fields_key].add(field)
+
+    for field in fields["pop"]:
+        if field not in fields["keep"]:
+            if nested:
+                data.pop(field, None)
+            else:
+                data[field] = None
 
     return data
 
 
 def get_option_value(option):
     """
     An option in a Checkboxes or CheckboxTree question is a dict, but we need to treat their
```

### Comparing `ccs-digitalmarketplace-content-loader-9.4.0/setup.py` & `ccs-digitalmarketplace-content-loader-9.5.0/setup.py`

 * *Files identical despite different names*

