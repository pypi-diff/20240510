# Comparing `tmp/bookmarks_converter-0.3.4.tar.gz` & `tmp/bookmarks_converter-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookmarks_converter-0.3.4.tar", max compression
+gzip compressed data, was "bookmarks_converter-0.3.5.tar", max compression
```

## Comparing `bookmarks_converter-0.3.4.tar` & `bookmarks_converter-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-10-13 13:47:35.525127 bookmarks_converter-0.3.4/LICENSE
--rw-r--r--   0        0        0     4670 2023-10-13 13:47:35.525127 bookmarks_converter-0.3.4/README.md
--rw-r--r--   0        0        0     1378 2023-10-13 13:47:35.529127 bookmarks_converter-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       37 2023-10-13 13:47:35.529127 bookmarks_converter-0.3.4/src/bookmarks_converter/__init__.py
--rw-r--r--   0        0        0       87 2023-10-13 13:47:35.529127 bookmarks_converter-0.3.4/src/bookmarks_converter/__main__.py
--rw-r--r--   0        0        0     2723 2023-10-13 13:47:35.529127 bookmarks_converter-0.3.4/src/bookmarks_converter/cli.py
--rw-r--r--   0        0        0    16191 2023-10-13 13:47:35.529127 bookmarks_converter-0.3.4/src/bookmarks_converter/core.py
--rw-r--r--   0        0        0    13498 2023-10-13 13:47:35.529127 bookmarks_converter-0.3.4/src/bookmarks_converter/models.py
--rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 bookmarks_converter-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-10 09:29:17.696418 bookmarks_converter-0.3.5/LICENSE
+-rw-r--r--   0        0        0     4670 2024-05-10 09:29:17.696418 bookmarks_converter-0.3.5/README.md
+-rw-r--r--   0        0        0     1378 2024-05-10 09:29:17.700418 bookmarks_converter-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-05-10 09:29:17.700418 bookmarks_converter-0.3.5/src/bookmarks_converter/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-10 09:29:17.700418 bookmarks_converter-0.3.5/src/bookmarks_converter/__main__.py
+-rw-r--r--   0        0        0     2723 2024-05-10 09:29:17.700418 bookmarks_converter-0.3.5/src/bookmarks_converter/cli.py
+-rw-r--r--   0        0        0    16191 2024-05-10 09:29:17.700418 bookmarks_converter-0.3.5/src/bookmarks_converter/core.py
+-rw-r--r--   0        0        0    13502 2024-05-10 09:29:17.700418 bookmarks_converter-0.3.5/src/bookmarks_converter/models.py
+-rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 bookmarks_converter-0.3.5/PKG-INFO
```

### Comparing `bookmarks_converter-0.3.4/LICENSE` & `bookmarks_converter-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bookmarks_converter-0.3.4/README.md` & `bookmarks_converter-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bookmarks_converter-0.3.4/pyproject.toml` & `bookmarks_converter-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookmarks-converter"
-version = "0.3.4"
+version = "0.3.5"
 description = "Parse db/html/json bookmarks file from (Chrome - Firefox - Custom source) and convert it to db/html/json format."
 authors = ["Adam Saleh <radam9@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/radam9/bookmarks-converter"
 repository = "https://github.com/radam9/bookmarks-converter"
 keywords = [
```

### Comparing `bookmarks_converter-0.3.4/src/bookmarks_converter/cli.py` & `bookmarks_converter-0.3.5/src/bookmarks_converter/cli.py`

 * *Files identical despite different names*

### Comparing `bookmarks_converter-0.3.4/src/bookmarks_converter/core.py` & `bookmarks_converter-0.3.5/src/bookmarks_converter/core.py`

 * *Files identical despite different names*

### Comparing `bookmarks_converter-0.3.4/src/bookmarks_converter/models.py` & `bookmarks_converter-0.3.5/src/bookmarks_converter/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             "icon": self.icon,
             "iconuri": self.icon_uri,
             "tags": self.tags,
         }
         return url
 
     def _check_instance_type(self, type_):
-        """"Check that the type of the instance matches the type of executed method"""
+        """ "Check that the type of the instance matches the type of executed method"""
         if self.type != type_:
             raise TypeError(f"The item you are converting is not a {type_}")
 
     def __iter__(self):
         """Iterating over an Object iterates over its contents."""
         return iter(self.children)
 
@@ -283,17 +283,17 @@
     Parameters:
     -----------
     The class expects a mix of parameters similar to the attributes, they vary
     depending on the element type (folder/url)"""
 
     def __init__(self, **kwargs):
         # Chrome has added a new field in their json file `meta_info`.
-        # This field is a dictionary with key/value pairs.
-        # ignore this field for the time being as it only contains `last_visited_desktop` key.
-        if "last_visited_desktop" in kwargs:
+        # This field is a dictionary with key/value pairs, and doesn't have an `id` field.
+        # ignore this field for the time being as it contains meta information.
+        if "id" not in kwargs:
             return
 
         # check the version of the passed json file depending on unique elements
         # that exist in each source.
         if "name" in kwargs:
             self.source = "Chrome"
         elif "typeCode" in kwargs:
```

### Comparing `bookmarks_converter-0.3.4/PKG-INFO` & `bookmarks_converter-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookmarks-converter
-Version: 0.3.4
+Version: 0.3.5
 Summary: Parse db/html/json bookmarks file from (Chrome - Firefox - Custom source) and convert it to db/html/json format.
 Home-page: https://github.com/radam9/bookmarks-converter
 License: MIT
 Keywords: bookmarks,bookmarks converter,bookmarks-converter,bookmarks-parser,bookmarks parser
 Author: Adam Saleh
 Author-email: radam9@gmail.com
 Requires-Python: >=3.9,<4.0
```

