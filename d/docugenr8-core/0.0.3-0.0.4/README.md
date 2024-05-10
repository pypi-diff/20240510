# Comparing `tmp/docugenr8_core-0.0.3.tar.gz` & `tmp/docugenr8_core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8_core-0.0.3.tar", last modified: Wed May  8 20:22:25 2024, max compression
+gzip compressed data, was "docugenr8_core-0.0.4.tar", last modified: Fri May 10 19:57:44 2024, max compression
```

## Comparing `docugenr8_core-0.0.3.tar` & `docugenr8_core-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.332346 docugenr8_core-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-08 20:22:25.328346 docugenr8_core-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:22:25.332346 docugenr8_core-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.324346 docugenr8_core-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.324346 docugenr8_core-0.0.3/src/docugenr8_core/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/build_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/font.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.328346 docugenr8_core-0.0.3/src/docugenr8_core/text_area/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/paragraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/textline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/word.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/src/docugenr8_core/text_area/words_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.328346 docugenr8_core-0.0.3/src/docugenr8_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-08 20:22:25.000000 docugenr8_core-0.0.3/src/docugenr8_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-08 20:22:25.000000 docugenr8_core-0.0.3/src/docugenr8_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:22:25.000000 docugenr8_core-0.0.3/src/docugenr8_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 20:22:25.000000 docugenr8_core-0.0.3/src/docugenr8_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 20:22:25.000000 docugenr8_core-0.0.3/src/docugenr8_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.328346 docugenr8_core-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/tests/test_1.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 20:21:54.000000 docugenr8_core-0.0.3/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.089646 docugenr8_core-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.093647 docugenr8_core-0.0.4/src/docugenr8_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/build_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/src/docugenr8_core/text_area/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/textarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/textline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/words_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/tests/test_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/version.txt
```

### Comparing `docugenr8_core-0.0.3/LICENSE` & `docugenr8_core-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/PKG-INFO` & `docugenr8_core-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: docugenr8-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fonttools
 Requires-Dist: docugenr8-shared<1.0.0,>=0.0.0
-Requires-Dist: docugenr8-pdf<1.0.0,>=0.0.0
 Provides-Extra: check
 Requires-Dist: ruff; extra == "check"
 Requires-Dist: mypy; extra == "check"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
```

### Comparing `docugenr8_core-0.0.3/pyproject.toml` & `docugenr8_core-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{ name = "Vladimir Jovanovic", email = "vladimirjo@protonmail.com" }]
 description = "Library for document creating"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = []
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
-dependencies = ["fonttools", "docugenr8-shared>=0.0.0,<1.0.0", "docugenr8-pdf>=0.0.0,<1.0.0"]
+dependencies = ["fonttools", "docugenr8-shared>=0.0.0,<1.0.0"]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = { file = "version.txt" }
 
 [project.optional-dependencies]
 check = ["ruff", "mypy"]
```

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/__init__.py` & `docugenr8_core-0.0.4/src/docugenr8_core/__init__.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/build_dto.py` & `docugenr8_core-0.0.4/src/docugenr8_core/build_dto.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/document.py` & `docugenr8_core-0.0.4/src/docugenr8_core/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,18 @@
         self.pages: list[Page] = []
         self.fonts: dict[str, Font] = {}
 
     def add_page(
         self,
         width: float,
         height: float,
-    ) -> None:
+    ) -> Page:
         page = Page(width, height)
         self.pages.append(page)
+        return page
 
     def add_font(
         self,
         font_name: str,
         path: str,
     ) -> None:
         font = Font(font_name, path)
```

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/font.py` & `docugenr8_core-0.0.4/src/docugenr8_core/font.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 TAB = 9
 NEW_LINE = 10
 SPACE = 32
 
 
 class Font:
-    def __init__(self, font_name: str, path: str) -> None:
+    def __init__(
+        self,
+        font_name: str,
+        path: str,
+    ) -> None:
         self.name = font_name
         self.raw_data = pathlib.Path(_resolve_file_path(path)).read_bytes()
         self.ttfont = ttLib.TTFont(BytesIO(self.raw_data), recalcTimestamp=False)
         self.cmap = self.ttfont.getBestCmap()
         self.em: float = self.ttfont["head"].unitsPerEm  # type: ignore
         self.ascent_per_em: float = self.ttfont["hhea"].ascent  # type: ignore
         self.descent_per_em: float = self.ttfont["hhea"].descent  # type: ignore
```

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/settings.py` & `docugenr8_core-0.0.4/src/docugenr8_core/settings.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/text_area/fragment.py` & `docugenr8_core-0.0.4/src/docugenr8_core/text_area/fragment.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/text_area/paragraph.py` & `docugenr8_core-0.0.4/src/docugenr8_core/text_area/paragraph.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/text_area/textarea.py` & `docugenr8_core-0.0.4/src/docugenr8_core/text_area/textarea.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,16 +243,18 @@
     def _add_words_front_to_textarea(self, words: deque[Word]) -> None:
         while len(words) > 0:
             word = words.popleft()
             self._paragraphs[0]._textlines[0]._append_word(word, 0)
         self._paragraphs[0]._adjust_words_between_textlines()
 
     def _get_next_word(self) -> Word | None:
-        """gets the next word from either next paragraph if there is one,
-        or from the words buffer
+        """Get next word.
+
+        Gets the next word from either next paragraph if there is one,
+        or from the words buffer.
         """
         textarea = self._get_next_textarea_with_words()
         if textarea is not None:
             return textarea._paragraphs[0]._textlines[0]._words[0]
         buffer = self._get_buffer()
         if len(buffer) == 0:
             return None
```

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/text_area/textline.py` & `docugenr8_core-0.0.4/src/docugenr8_core/text_area/textline.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/text_area/word.py` & `docugenr8_core-0.0.4/src/docugenr8_core/text_area/word.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core/text_area/words_creation.py` & `docugenr8_core-0.0.4/src/docugenr8_core/text_area/words_creation.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core.egg-info/PKG-INFO` & `docugenr8_core-0.0.4/src/docugenr8_core.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: docugenr8-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fonttools
 Requires-Dist: docugenr8-shared<1.0.0,>=0.0.0
-Requires-Dist: docugenr8-pdf<1.0.0,>=0.0.0
 Provides-Extra: check
 Requires-Dist: ruff; extra == "check"
 Requires-Dist: mypy; extra == "check"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
```

### Comparing `docugenr8_core-0.0.3/src/docugenr8_core.egg-info/SOURCES.txt` & `docugenr8_core-0.0.4/src/docugenr8_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.3/tests/test_1.py` & `docugenr8_core-0.0.4/tests/test_1.py`

 * *Files identical despite different names*

