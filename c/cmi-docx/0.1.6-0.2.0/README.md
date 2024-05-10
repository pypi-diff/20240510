# Comparing `tmp/cmi_docx-0.1.6.tar.gz` & `tmp/cmi_docx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmi_docx-0.1.6.tar", max compression
+gzip compressed data, was "cmi_docx-0.2.0.tar", max compression
```

## Comparing `cmi_docx-0.1.6.tar` & `cmi_docx-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    26526 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/LICENSE
--rw-r--r--   0        0        0     1899 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/README.md
--rw-r--r--   0        0        0     1557 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      295 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/src/cmi_docx/__init__.py
--rw-r--r--   0        0        0     4983 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/src/cmi_docx/document.py
--rw-r--r--   0        0        0     6029 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/src/cmi_docx/paragraph.py
--rw-r--r--   0        0        0     6833 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/src/cmi_docx/run.py
--rw-r--r--   0        0        0     2684 2024-04-17 20:08:53.674223 cmi_docx-0.1.6/src/cmi_docx/table.py
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 cmi_docx-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1899 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/README.md
+-rw-r--r--   0        0        0     1565 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      374 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/src/cmi_docx/__init__.py
+-rw-r--r--   0        0        0     4969 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/src/cmi_docx/document.py
+-rw-r--r--   0        0        0     6080 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/src/cmi_docx/paragraph.py
+-rw-r--r--   0        0        0     6335 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/src/cmi_docx/run.py
+-rw-r--r--   0        0        0     1111 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/src/cmi_docx/styles.py
+-rw-r--r--   0        0        0     2684 2024-05-10 18:01:54.173677 cmi_docx-0.2.0/src/cmi_docx/table.py
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 cmi_docx-0.2.0/PKG-INFO
```

### Comparing `cmi_docx-0.1.6/LICENSE` & `cmi_docx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.6/README.md` & `cmi_docx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.6/pyproject.toml` & `cmi_docx-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmi_docx"
-version = "0.1.6"
+version = "0.2.0"
 description = ".docx utilities"
 authors = ["Reinder Vos de Wael <reinder.vosdewael@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "cmi_docx", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -12,15 +12,15 @@
 python-docx = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 mypy = "^1.9.0"
 pre-commit = "^3.7.0"
 pytest-cov = "^5.0.0"
-ruff = "^0.3.4"
+ruff = ">=0.3.4,<0.5.0"
 
 [tool.poetry.group.docs.dependencies]
 pdoc = "^14.4.0"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
```

### Comparing `cmi_docx-0.1.6/src/cmi_docx/document.py` & `cmi_docx-0.2.0/src/cmi_docx/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Extends a python-docx Word document with additional functionality."""
 
 import pathlib
-from typing import Any
 
 from docx import document
 from docx.text import paragraph as docx_paragraph
 
-from cmi_docx import paragraph, run
+from cmi_docx import paragraph, run, styles
 
 
 class ExtendDocument:
     """Extends a python-docx Word document with additional functionality."""
 
     def __init__(self, document: document.Document) -> None:
         """Initializes a DocxSearch object for finding text."""
@@ -42,15 +41,15 @@
         return [
             finder
             for para in self.all_paragraphs
             for finder in paragraph.ExtendParagraph(para).find_in_runs(needle)
         ]
 
     def replace(
-        self, needle: str, replace: str, style: dict[str, Any] | None = None
+        self, needle: str, replace: str, style: styles.RunStyle | None = None
     ) -> None:
         """Finds and replaces text in a Word document.
 
         Args:
             needle: The text to find.
             replace: The text to replace.
             style: The style to apply to the replacement text.
```

### Comparing `cmi_docx-0.1.6/src/cmi_docx/paragraph.py` & `cmi_docx-0.2.0/src/cmi_docx/paragraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Module for extending python-docx Paragraph objects."""
 
 import bisect
 import dataclasses
 import itertools
 import re
-from typing import Any
 
 from docx.enum import text
 from docx.text import paragraph as docx_paragraph
 from docx.text import run as docx_run
 
-from cmi_docx import run
+from cmi_docx import run, styles
 
 
 @dataclasses.dataclass
 class FindParagraph:
     """Data class for maintaing find results in paragraphs.
 
     Attributes:
@@ -95,15 +94,15 @@
                     run_indices=(start_run, end_run),
                     character_indices=(start_index, end_index),
                 )
             )
         return run_finds
 
     def replace(
-        self, needle: str, replace: str, style: dict[str, Any] | None = None
+        self, needle: str, replace: str, style: styles.RunStyle | None = None
     ) -> None:
         """Finds and replaces text in a Word paragraph.
 
         Args:
             needle: The text to find.
             replace: The text to replace.
             style: The style to apply to the replacement text.
@@ -112,15 +111,15 @@
         run_finder.sort(
             key=lambda x: (x.run_indices[0], x.character_indices[0]), reverse=True
         )
 
         for run_find in run_finder:
             run_find.replace(replace, style)
 
-    def insert_run(self, index: int, text: str, style: dict[str, Any]) -> docx_run.Run:
+    def insert_run(self, index: int, text: str, style: styles.RunStyle) -> docx_run.Run:
         """Inserts a run into a paragraph.
 
         Args:
             index: The index to insert the run at.
             text: The text of the run.
             style: The style of the run, see run.ExtendRun.format for more details.
 
@@ -133,15 +132,15 @@
             new_run = self.paragraph._element._new_r()
             new_run.text = text
             if index < 0:
                 self.paragraph.runs[index]._element.addnext(new_run)
             else:
                 self.paragraph.runs[index]._element.addprevious(new_run)
 
-        run.ExtendRun(self.paragraph.runs[index]).format(**style)
+        run.ExtendRun(self.paragraph.runs[index]).format(style)
         return self.paragraph.runs[index]
 
     def format(
         self,
         *,
         bold: bool | None = None,
         italics: bool | None = None,
@@ -174,12 +173,14 @@
             self.paragraph.paragraph_format.space_before = space_before
 
         if space_after is not None:
             self.paragraph.paragraph_format.space_after = space_after
 
         for paragraph_run in self.paragraph.runs:
             run.ExtendRun(paragraph_run).format(
-                bold=bold,
-                italics=italics,
-                font_size=font_size,
-                font_rgb=font_rgb,
+                styles.RunStyle(
+                    bold=bold,
+                    italic=italics,
+                    font_size=font_size,
+                    font_rgb=font_rgb,
+                )
             )
```

### Comparing `cmi_docx-0.1.6/src/cmi_docx/run.py` & `cmi_docx-0.2.0/src/cmi_docx/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for extending python-docx Run objects."""
 
-from typing import Any
-
 from docx import shared
 from docx.text import paragraph as docx_paragraph
 
+from cmi_docx import styles
+
 
 class FindRun:
     """Data class for maintaing find results in runs.
 
     Attributes:
         paragraph: The paragraph containing the text.
         run_indices: The run indices of the text needle's start and end.
@@ -36,15 +36,15 @@
         self._replacement_done = False
 
     @property
     def runs(self) -> list[docx_paragraph.Run]:
         """Returns the runs containing the text."""
         return self.paragraph.runs[self.run_indices[0] : self.run_indices[1] + 1]
 
-    def replace(self, replace: str, style: dict[str, Any] | None = None) -> None:
+    def replace(self, replace: str, style: styles.RunStyle | None = None) -> None:
         """Replaces the text in the runs with the replacement text.
 
         Args:
             replace: The text to replace.
             style: The style to apply to the replacement text. If None, the
                 replacement text will have the same style as the first character of the
                 original text.
@@ -75,15 +75,15 @@
             )
         else:
             self.runs[0].text = self.runs[0].text[:start] + replace
             for run in self.runs[1:-1]:
                 run.clear()
             self.runs[-1].text = self.runs[-1].text[end:]
 
-    def _replace_with_style(self, replace: str, style: dict[str, Any]) -> None:
+    def _replace_with_style(self, replace: str, style: styles.RunStyle) -> None:
         """Replaces the text in the runs with the replacement text and style.
 
         Args:
             replace: The text to replace.
             style: The style to apply to the replacement text.
         """
         start = self.character_indices[0]
@@ -91,21 +91,21 @@
 
         pre, post = self.runs[0].text[:start], self.runs[0].text[end:]
         self.runs[0].text = pre
 
         new_run = self.paragraph._element._new_r()
         new_run.text = replace
         self.paragraph.runs[self.run_indices[0]]._element.addnext(new_run)
-        ExtendRun(self.paragraph.runs[self.run_indices[0] + 1]).format(**style)
+        ExtendRun(self.paragraph.runs[self.run_indices[0] + 1]).format(style)
 
         post_run = self.paragraph._element._new_r()
         post_run.text = post
         self.paragraph.runs[self.run_indices[0] + 1]._element.addnext(post_run)
         pre_style = ExtendRun(self.paragraph.runs[self.run_indices[0]]).get_format()
-        ExtendRun(self.paragraph.runs[self.run_indices[0] + 2]).format(**pre_style)
+        ExtendRun(self.paragraph.runs[self.run_indices[0] + 2]).format(pre_style)
 
     def __lt__(self, other: "FindRun") -> bool:
         """Sorts FindRun in order of appearance in the paragraph.
 
         Makes FindRun objects sortable.
 
         Args:
@@ -131,63 +131,47 @@
         """Initializes an ExtendRun object.
 
         Args:
             run: The run to extend.
         """
         self.run = run
 
-    def format(
-        self,
-        *,
-        bold: bool | None = None,
-        italics: bool | None = None,
-        underline: bool | None = None,
-        superscript: bool | None = None,
-        subscript: bool | None = None,
-        font_size: int | None = None,
-        font_rgb: tuple[int, int, int] | None = None,
-    ) -> None:
+    def format(self, style: styles.RunStyle) -> None:
         """Formats a run in a Word document.
 
         Args:
-            bold: Whether to bold the run.
-            italics: Whether to italicize the run.
-            underline: Whether to underline the run.
-            superscript: Whether to superscript the run.
-            subscript: Whether to subscript the run.
-            font_size: The font size of the run.
-            font_rgb: The font color of the run.
+            style: The style to apply to the run.
         """
-        if superscript and subscript:
+        if style.superscript and style.subscript:
             msg = "Cannot have superscript and subscript at the same time."
             raise ValueError(msg)
 
-        if bold is not None:
-            self.run.bold = bold
-        if italics is not None:
-            self.run.italic = italics
-        if underline is not None:
-            self.run.underline = underline
-        if superscript is not None:
-            self.run.font.superscript = superscript
-        if subscript is not None:
-            self.run.font.subscript = subscript
-        if font_size is not None:
-            self.run.font.size = font_size
-        if font_rgb is not None:
-            self.run.font.color.rgb = shared.RGBColor(*font_rgb)
+        if style.bold is not None:
+            self.run.bold = style.bold
+        if style.italic is not None:
+            self.run.italic = style.italic
+        if style.underline is not None:
+            self.run.underline = style.underline
+        if style.superscript is not None:
+            self.run.font.superscript = style.superscript
+        if style.subscript is not None:
+            self.run.font.subscript = style.subscript
+        if style.font_size is not None:
+            self.run.font.size = style.font_size
+        if style.font_rgb is not None:
+            self.run.font.color.rgb = shared.RGBColor(*style.font_rgb)
 
-    def get_format(self) -> dict[str, Any]:
+    def get_format(self) -> styles.RunStyle:
         """Returns the formatting of the run.
 
         Returns:
             The formatting of the run.
         """
-        return {
-            "bold": self.run.bold,
-            "italics": self.run.italic,
-            "underline": self.run.underline,
-            "superscript": self.run.font.superscript,
-            "subscript": self.run.font.subscript,
-            "font_size": self.run.font.size,
-            "font_rgb": self.run.font.color.rgb,
-        }
+        return styles.RunStyle(
+            bold=self.run.bold,
+            italic=self.run.italic,
+            underline=self.run.underline,
+            superscript=self.run.font.superscript,
+            subscript=self.run.font.subscript,
+            font_size=self.run.font.size,
+            font_rgb=self.run.font.color.rgb,
+        )
```

### Comparing `cmi_docx-0.1.6/src/cmi_docx/table.py` & `cmi_docx-0.2.0/src/cmi_docx/table.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.6/PKG-INFO` & `cmi_docx-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmi_docx
-Version: 0.1.6
+Version: 0.2.0
 Summary: .docx utilities
 License: LGPL-2.1
 Author: Reinder Vos de Wael
 Author-email: reinder.vosdewael@childmind.org
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

