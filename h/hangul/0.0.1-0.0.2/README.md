# Comparing `tmp/hangul-0.0.1.tar.gz` & `tmp/hangul-0.0.2.tar.gz`

## Comparing `hangul-0.0.1.tar` & `hangul-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 hangul-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/assemble.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/chosung_includes.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/combine_hangul_character.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/constants.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/convert_qwerty_to_hangul_alphabet.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/disassemble.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/disassemble_complete_hangul_character.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/hangul_includes.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/josa.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/remove_last_hangul_character.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/utils.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/internal/hangul.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 hangul-0.0.1/hangul/internal/utils.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_assemble.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_chosung_includes.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_combine_hangul_character.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_convert_qwerty_to_hangul_alphabet.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_disassemble.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_disassemble_complete_hangul_character.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_hangul_includes.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_josa.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_remove_last_hangul_character.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/test_utils.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 hangul-0.0.1/tests/internal/test_hangul.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hangul-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hangul-0.0.1/LICENSE
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hangul-0.0.1/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 hangul-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hangul-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 hangul-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/assemble.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/chosung_includes.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/combine_hangul_character.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/constants.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/convert_qwerty_to_hangul_alphabet.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/disassemble.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/disassemble_complete_hangul_character.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/hangul_includes.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/josa.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/remove_last_hangul_character.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/utils.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/internal/hangul.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 hangul-0.0.2/hangul/internal/utils.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_assemble.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_chosung_includes.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_combine_hangul_character.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_convert_qwerty_to_hangul_alphabet.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_disassemble.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_disassemble_complete_hangul_character.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_hangul_includes.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_josa.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_remove_last_hangul_character.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 hangul-0.0.2/tests/internal/test_hangul.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hangul-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hangul-0.0.2/LICENSE
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 hangul-0.0.2/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 hangul-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hangul-0.0.2/PKG-INFO
```

### Comparing `hangul-0.0.1/.github/workflows/ci.yaml` & `hangul-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/assemble.py` & `hangul-0.0.2/hangul/assemble.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/chosung_includes.py` & `hangul-0.0.2/hangul/chosung_includes.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/combine_hangul_character.py` & `hangul-0.0.2/hangul/combine_hangul_character.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/constants.py` & `hangul-0.0.2/hangul/constants.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/convert_qwerty_to_hangul_alphabet.py` & `hangul-0.0.2/hangul/convert_qwerty_to_hangul_alphabet.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/disassemble.py` & `hangul-0.0.2/hangul/disassemble.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/disassemble_complete_hangul_character.py` & `hangul-0.0.2/hangul/disassemble_complete_hangul_character.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/josa.py` & `hangul-0.0.2/hangul/josa.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/remove_last_hangul_character.py` & `hangul-0.0.2/hangul/remove_last_hangul_character.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/utils.py` & `hangul-0.0.2/hangul/utils.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/internal/hangul.py` & `hangul-0.0.2/hangul/internal/hangul.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/hangul/internal/utils.py` & `hangul-0.0.2/hangul/internal/utils.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_assemble.py` & `hangul-0.0.2/tests/test_assemble.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_chosung_includes.py` & `hangul-0.0.2/tests/test_chosung_includes.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_combine_hangul_character.py` & `hangul-0.0.2/tests/test_combine_hangul_character.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_convert_qwerty_to_hangul_alphabet.py` & `hangul-0.0.2/tests/test_convert_qwerty_to_hangul_alphabet.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_disassemble.py` & `hangul-0.0.2/tests/test_disassemble.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_disassemble_complete_hangul_character.py` & `hangul-0.0.2/tests/test_disassemble_complete_hangul_character.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_hangul_includes.py` & `hangul-0.0.2/tests/test_hangul_includes.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_josa.py` & `hangul-0.0.2/tests/test_josa.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_remove_last_hangul_character.py` & `hangul-0.0.2/tests/test_remove_last_hangul_character.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/test_utils.py` & `hangul-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/tests/internal/test_hangul.py` & `hangul-0.0.2/tests/internal/test_hangul.py`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/.gitignore` & `hangul-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/LICENSE` & `hangul-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hangul-0.0.1/pyproject.toml` & `hangul-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["hangul"]
 
 [project]
 name = "hangul"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "John Choi", email = "isnbh0@gmail.com" }]
 description = "A Python port of the es-hangul JavaScript library."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/isnbh0/py-hangul"
-Issues = "https://github.com/isnbh0/py-hangul/issues"
+Homepage = "https://github.com/isnbh0/hangul"
+Issues = "https://github.com/isnbh0/hangul/issues"
```

### Comparing `hangul-0.0.1/PKG-INFO` & `hangul-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: hangul
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python port of the es-hangul JavaScript library.
-Project-URL: Homepage, https://github.com/isnbh0/py-hangul
-Project-URL: Issues, https://github.com/isnbh0/py-hangul/issues
+Project-URL: Homepage, https://github.com/isnbh0/hangul
+Project-URL: Issues, https://github.com/isnbh0/hangul/issues
 Author-email: John Choi <isnbh0@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# pyhangul
+# hangul
 
 A port of [es-hangul](https://github.com/toss/es-hangul) into Python.
```

