# Comparing `tmp/imy-0.3.0.tar.gz` & `tmp/imy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.3.0.tar", max compression
+gzip compressed data, was "imy-0.3.1.tar", max compression
```

## Comparing `imy-0.3.0.tar` & `imy-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.0/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.0/imy/__init__.py
--rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.0/imy/assets.py
--rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.0/imy/async_utils.py
--rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.0/imy/config.py
--rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.0/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     6498 2024-04-28 15:53:31.243915 imy-0.3.0/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    17433 2024-05-06 15:16:53.871680 imy-0.3.0/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.0/imy/inject.py
--rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.0/imy/logs.py
--rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.0/imy/package_metadata.py
--rw-r--r--   0        0        0      753 2024-05-06 18:22:57.896321 imy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.1/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.1/imy/__init__.py
+-rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.1/imy/assets.py
+-rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.1/imy/async_utils.py
+-rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.1/imy/config.py
+-rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.1/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     6498 2024-04-28 15:53:31.243915 imy-0.3.1/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    18387 2024-05-10 11:07:00.691935 imy-0.3.1/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.1/imy/inject.py
+-rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.1/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.1/imy/package_metadata.py
+-rw-r--r--   0        0        0      753 2024-05-10 11:08:02.772084 imy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.1/PKG-INFO
```

### Comparing `imy-0.3.0/LICENSE` & `imy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/assets.py` & `imy-0.3.1/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/async_utils.py` & `imy-0.3.1/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/config.py` & `imy-0.3.1/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/docstrings/__init__.py` & `imy-0.3.1/imy/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/docstrings/data_models.py` & `imy-0.3.1/imy/docstrings/data_models.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/docstrings/parsers.py` & `imy-0.3.1/imy/docstrings/parsers.py`

 * *Files 7% similar despite different names*

```diff
@@ -379,14 +379,17 @@
     )
 
 
 def _parse_class_docstring_with_inheritance(
     cls: type,
     *,
     key_sections: Iterable[str],
+    merge_key_section: Callable[
+        [str, dict[str, str], dict[str, str]], dict[str, str]
+    ] = lambda name, parent, child: {**parent, **child},
 ) -> data_models.Docstring:
     """
     Parses the docstring of a class in the same format as `parse_docstring`, but
     accounts for inheritance: Key-Value sections of all classes are merged, in a
     way that preserves child docs over parent docs.
     """
 
@@ -403,25 +406,29 @@
     base_docs: list[data_models.Docstring] = []
 
     for base in cls.__bases__:
         base_docs.append(
             _parse_class_docstring_with_inheritance(
                 base,
                 key_sections=key_sections,
+                merge_key_section=merge_key_section,
             )
         )
 
     # Merge the docstrings
     result_sections: dict[str, dict[str, str]] = {}
     all_in_order = base_docs + [parsed_docs]
 
-    for docs in all_in_order:
-        for section_name, section in docs.key_sections.items():
-            result_section = result_sections.setdefault(section_name, {})
-            result_section.update(section)
+    for cur_docs in all_in_order:
+        for section_name, cur_section in cur_docs.key_sections.items():
+            result_section = result_sections.get(section_name, {})
+            result_section = merge_key_section(
+                section_name, result_section, cur_section
+            )
+            result_sections[section_name] = result_section
 
     parsed_docs.key_sections = result_sections
 
     # Done
     return parsed_docs
 
 
@@ -489,21 +496,37 @@
             if dataclass_field.default is not dataclasses.MISSING:
                 doc_field.default = repr(dataclass_field.default)
 
             # Default factory?
             elif dataclass_field.default_factory is not dataclasses.MISSING:
                 doc_field.default = repr(dataclass_field.default_factory())
 
+    # Prepare a function for merging key sections
+    def merge_key_section(
+        name: str,
+        parent: dict[str, str],
+        child: dict[str, str],
+    ) -> dict[str, str]:
+        # Metadata is special: The parent doesn't matter, the child always wins.
+        # This is to avoid unexpected situations, where a class would be e.g.
+        # private, just because the parent is private.
+        if name == "metadata":
+            return child
+
+        # Otherwise merge the two. Child values override parent values.
+        return {**parent, **child}
+
     # Parse the docstring
     docs = _parse_class_docstring_with_inheritance(
         cls,
         key_sections=[
             "attributes",
             "metadata",
         ],
+        merge_key_section=merge_key_section,
     )
 
     # Add any information learned about fields from the docstring
     for field_name, field_details in docs.key_sections["attributes"].items():
         try:
             result_field = fields_by_name[field_name]
         except KeyError:
```

### Comparing `imy-0.3.0/imy/inject.py` & `imy-0.3.1/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/logs.py` & `imy-0.3.1/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/imy/package_metadata.py` & `imy-0.3.1/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.0/pyproject.toml` & `imy-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.3.0"
+version = "0.3.1"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.3.0/PKG-INFO` & `imy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

