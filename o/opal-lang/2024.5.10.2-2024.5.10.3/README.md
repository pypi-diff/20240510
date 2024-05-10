# Comparing `tmp/opal_lang-2024.5.10.2.tar.gz` & `tmp/opal_lang-2024.5.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal_lang-2024.5.10.2.tar", last modified: Fri May 10 19:09:48 2024, max compression
+gzip compressed data, was "opal_lang-2024.5.10.3.tar", last modified: Fri May 10 19:43:21 2024, max compression
```

## Comparing `opal_lang-2024.5.10.2.tar` & `opal_lang-2024.5.10.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:48.068425 opal_lang-2024.5.10.2/
--rw-rw-rw-   0        0        0     1087 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/LICENSE
--rw-rw-rw-   0        0        0    20114 2024-05-10 19:09:48.066425 opal_lang-2024.5.10.2/PKG-INFO
--rw-rw-rw-   0        0        0    19535 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/README.md
--rw-rw-rw-   0        0        0      788 2024-05-10 19:08:36.000000 opal_lang-2024.5.10.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 19:09:48.068425 opal_lang-2024.5.10.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:47.989408 opal_lang-2024.5.10.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:47.996409 opal_lang-2024.5.10.2/src/opal/
--rw-rw-rw-   0        0        0     2939 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/__init__.py
--rw-rw-rw-   0        0        0    12074 2024-05-10 19:06:26.000000 opal_lang-2024.5.10.2/src/opal/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:48.002410 opal_lang-2024.5.10.2/src/opal/components/
--rw-rw-rw-   0        0        0    96441 2024-05-10 19:08:47.000000 opal_lang-2024.5.10.2/src/opal/components/Compiler.py
--rw-rw-rw-   0        0        0    13383 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/components/Tokens.py
--rw-rw-rw-   0        0        0     3138 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/components/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:48.008412 opal_lang-2024.5.10.2/src/opal/examples/
--rw-rw-rw-   0        0        0    10096 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/examples/2048.opal
--rw-rw-rw-   0        0        0      688 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/examples/fibonacci.opal
--rw-rw-rw-   0        0        0     5598 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/examples/fireworks.opal
--rw-rw-rw-   0        0        0     4776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/examples/rain.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:48.028416 opal_lang-2024.5.10.2/src/opal/libs/
--rw-rw-rw-   0        0        0     8863 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/Array.py
--rw-rw-rw-   0        0        0     1910 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/Queue.py
--rw-rw-rw-   0        0        0     1680 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/Stack.py
--rw-rw-rw-   0        0        0     7650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/Vector.py
--rw-rw-rw-   0        0        0     1675 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/_internals.py
--rw-rw-rw-   0        0        0     6951 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/char.py
--rw-rw-rw-   0        0        0     5836 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/fastSort.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:48.031417 opal_lang-2024.5.10.2/src/opal/libs/graphics/
--rw-rw-rw-   0        0        0    14759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/graphics/Graphics.py
--rw-rw-rw-   0        0        0      743 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/graphics/icon.png
--rw-rw-rw-   0        0        0     2650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/helpers.opal
--rw-rw-rw-   0        0        0     9776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/merge.opal
--rw-rw-rw-   0        0        0     5759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/sort.opal
--rw-rw-rw-   0        0        0     2810 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/stableSort.opal
--rw-rw-rw-   0        0        0     7145 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/libs/std.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:48.035418 opal_lang-2024.5.10.2/src/opal/runner/
--rw-rw-rw-   0        0        0      772 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/runner/build.py
--rw-rw-rw-   0        0        0   270398 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.2/src/opal/runner/icon.ico
-drwxrwxrwx   0        0        0        0 2024-05-10 19:09:48.064424 opal_lang-2024.5.10.2/src/opal_lang.egg-info/
--rw-rw-rw-   0        0        0    20114 2024-05-10 19:09:47.000000 opal_lang-2024.5.10.2/src/opal_lang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2024-05-10 19:09:47.000000 opal_lang-2024.5.10.2/src/opal_lang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 19:09:47.000000 opal_lang-2024.5.10.2/src/opal_lang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-10 19:09:47.000000 opal_lang-2024.5.10.2/src/opal_lang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-10 19:09:47.000000 opal_lang-2024.5.10.2/src/opal_lang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.167282 opal_lang-2024.5.10.3/
+-rw-rw-rw-   0        0        0     1087 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/LICENSE
+-rw-rw-rw-   0        0        0    20114 2024-05-10 19:43:21.165281 opal_lang-2024.5.10.3/PKG-INFO
+-rw-rw-rw-   0        0        0    19535 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/README.md
+-rw-rw-rw-   0        0        0      788 2024-05-10 19:42:27.000000 opal_lang-2024.5.10.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 19:43:21.167282 opal_lang-2024.5.10.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.097265 opal_lang-2024.5.10.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.105267 opal_lang-2024.5.10.3/src/opal/
+-rw-rw-rw-   0        0        0     2939 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/__init__.py
+-rw-rw-rw-   0        0        0    12134 2024-05-10 19:41:58.000000 opal_lang-2024.5.10.3/src/opal/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.109268 opal_lang-2024.5.10.3/src/opal/components/
+-rw-rw-rw-   0        0        0    96441 2024-05-10 19:42:22.000000 opal_lang-2024.5.10.3/src/opal/components/Compiler.py
+-rw-rw-rw-   0        0        0    13383 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/components/Tokens.py
+-rw-rw-rw-   0        0        0     3138 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/components/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.116270 opal_lang-2024.5.10.3/src/opal/examples/
+-rw-rw-rw-   0        0        0    10096 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/examples/2048.opal
+-rw-rw-rw-   0        0        0      688 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/examples/fibonacci.opal
+-rw-rw-rw-   0        0        0     5598 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/examples/fireworks.opal
+-rw-rw-rw-   0        0        0     4776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/examples/rain.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.135273 opal_lang-2024.5.10.3/src/opal/libs/
+-rw-rw-rw-   0        0        0     8863 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/Array.py
+-rw-rw-rw-   0        0        0     1910 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/Queue.py
+-rw-rw-rw-   0        0        0     1680 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/Stack.py
+-rw-rw-rw-   0        0        0     7650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/Vector.py
+-rw-rw-rw-   0        0        0     1675 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/_internals.py
+-rw-rw-rw-   0        0        0     6951 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/char.py
+-rw-rw-rw-   0        0        0     5836 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/fastSort.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.138275 opal_lang-2024.5.10.3/src/opal/libs/graphics/
+-rw-rw-rw-   0        0        0    14759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/graphics/Graphics.py
+-rw-rw-rw-   0        0        0      743 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/graphics/icon.png
+-rw-rw-rw-   0        0        0     2650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/helpers.opal
+-rw-rw-rw-   0        0        0     9776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/merge.opal
+-rw-rw-rw-   0        0        0     5759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/sort.opal
+-rw-rw-rw-   0        0        0     2810 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/stableSort.opal
+-rw-rw-rw-   0        0        0     7145 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/libs/std.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.141276 opal_lang-2024.5.10.3/src/opal/runner/
+-rw-rw-rw-   0        0        0      772 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/runner/build.py
+-rw-rw-rw-   0        0        0   270398 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.3/src/opal/runner/icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-10 19:43:21.164281 opal_lang-2024.5.10.3/src/opal_lang.egg-info/
+-rw-rw-rw-   0        0        0    20114 2024-05-10 19:43:21.000000 opal_lang-2024.5.10.3/src/opal_lang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-05-10 19:43:21.000000 opal_lang-2024.5.10.3/src/opal_lang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 19:43:21.000000 opal_lang-2024.5.10.3/src/opal_lang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-10 19:43:21.000000 opal_lang-2024.5.10.3/src/opal_lang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-10 19:43:21.000000 opal_lang-2024.5.10.3/src/opal_lang.egg-info/top_level.txt
```

### Comparing `opal_lang-2024.5.10.2/LICENSE` & `opal_lang-2024.5.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/PKG-INFO` & `opal_lang-2024.5.10.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-lang
-Version: 2024.5.10.2
+Version: 2024.5.10.3
 Summary: A programming language based on Python and Cython
 Project-URL: Homepage, https://github.com/thatsOven/opal-lang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `opal_lang-2024.5.10.2/README.md` & `opal_lang-2024.5.10.3/README.md`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/pyproject.toml` & `opal_lang-2024.5.10.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "*" = ["*.opal", "*.ico", "*.png"]
 
 [project]
 name = "opal-lang"
-version = "2024.5.10.2"
+version = "2024.5.10.3"
 description = "A programming language based on Python and Cython"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `opal_lang-2024.5.10.2/src/opal/__init__.py` & `opal_lang-2024.5.10.3/src/opal/__init__.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/__main__.py` & `opal_lang-2024.5.10.3/src/opal/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import os, sys, shutil, numpy, subprocess
-from timeit              import default_timer
-from pathlib             import Path
-from setuptools          import setup
-from Cython.Build        import cythonize
-from Cython.Compiler     import Options
+import os, sys, shutil, numpy, subprocess, traceback
+from timeit          import default_timer
+from pathlib         import Path
+from setuptools      import setup
+from Cython.Build    import cythonize
+from Cython.Compiler import Options
 
 from opal.components.Compiler import *
 
 RELEASE_COLLECT = ["__future__", "typeguard", "pygame", "unittest", "numpy", "json"]
 PY_STDLIB       = set(sys.stdlib_module_names) | {"opal"} - {"antigravity"} # fun, but i don't wanna open the xkcd page every time i compile something
 NO_INSTALL      = set(RELEASE_COLLECT) | PY_STDLIB
 
@@ -46,15 +46,16 @@
             name         = os.path.basename(file).split(".")[0],
             include_dirs = [numpy.get_include()], 
             ext_modules  = cythonize(file, compiler_directives = {
                 "language_level": "3"
             }),
             zip_safe = False
         )
-    except:
+    except Exception:
+        print(traceback.format_exc())
         ok = False
     else:
         ok = True
 
     sys.argv = oldArgs
 
     return ok
@@ -85,15 +86,15 @@
         if (not compiler.module) or noModule:
             if len(sys.argv) == 3:
                 filename = f"{endName}.py"
             else:
                 filename = sys.argv[3]
                 name = os.path.basename(filename).split(".")[0]
 
-            with open(filename, "w") as py:
+            with open(filename, "w", encoding = "utf-8") as py:
                 py.write(f"from os import environ\nenviron['_OPAL_RUN_AS_MAIN_']=''\nimport {name}\ndel environ['_OPAL_RUN_AS_MAIN_']")
         return filename
 
 def compileOne(libs, file, compiler):
     time = default_timer()
 
     filename = os.path.join(libs, file)
```

### Comparing `opal_lang-2024.5.10.2/src/opal/components/Compiler.py` & `opal_lang-2024.5.10.3/src/opal/components/Compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from importlib import import_module
 from traceback import format_exception
 import os
 
 from opal.components.utils  import *
 from opal.components.Tokens import *
 
-VERSION = (2024, 5, 10, 2)
+VERSION = (2024, 5, 10, 3)
 SET_OPS = ("+=", "-=", "**=", "//=", "*=", "/=", "%=", "&=", "|=", "^=", ">>=", "<<=", "@=", "=")
 CYTHON_TYPES = (
     "short", "int", "long", "long long", "float", "bint",
     "double", "long double", "list", "object", "str", 
     "tuple", "dict", "range", "bytes", "bytearray", "complex"
 )
 CYTHON_FN_TYPES = CYTHON_TYPES + ("void", "bool")
```

### Comparing `opal_lang-2024.5.10.2/src/opal/components/Tokens.py` & `opal_lang-2024.5.10.3/src/opal/components/Tokens.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/components/utils.py` & `opal_lang-2024.5.10.3/src/opal/components/utils.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/examples/2048.opal` & `opal_lang-2024.5.10.3/src/opal/examples/2048.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/examples/fibonacci.opal` & `opal_lang-2024.5.10.3/src/opal/examples/fibonacci.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/examples/fireworks.opal` & `opal_lang-2024.5.10.3/src/opal/examples/fireworks.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/examples/rain.opal` & `opal_lang-2024.5.10.3/src/opal/examples/rain.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/Array.py` & `opal_lang-2024.5.10.3/src/opal/libs/Array.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/Queue.py` & `opal_lang-2024.5.10.3/src/opal/libs/Queue.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/Stack.py` & `opal_lang-2024.5.10.3/src/opal/libs/Stack.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/Vector.py` & `opal_lang-2024.5.10.3/src/opal/libs/Vector.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/_internals.py` & `opal_lang-2024.5.10.3/src/opal/libs/_internals.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/char.py` & `opal_lang-2024.5.10.3/src/opal/libs/char.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/fastSort.opal` & `opal_lang-2024.5.10.3/src/opal/libs/fastSort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/graphics/Graphics.py` & `opal_lang-2024.5.10.3/src/opal/libs/graphics/Graphics.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/graphics/icon.png` & `opal_lang-2024.5.10.3/src/opal/libs/graphics/icon.png`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/helpers.opal` & `opal_lang-2024.5.10.3/src/opal/libs/helpers.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/merge.opal` & `opal_lang-2024.5.10.3/src/opal/libs/merge.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/sort.opal` & `opal_lang-2024.5.10.3/src/opal/libs/sort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/stableSort.opal` & `opal_lang-2024.5.10.3/src/opal/libs/stableSort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/libs/std.opal` & `opal_lang-2024.5.10.3/src/opal/libs/std.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/runner/build.py` & `opal_lang-2024.5.10.3/src/opal/runner/build.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal/runner/icon.ico` & `opal_lang-2024.5.10.3/src/opal/runner/icon.ico`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.2/src/opal_lang.egg-info/PKG-INFO` & `opal_lang-2024.5.10.3/src/opal_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-lang
-Version: 2024.5.10.2
+Version: 2024.5.10.3
 Summary: A programming language based on Python and Cython
 Project-URL: Homepage, https://github.com/thatsOven/opal-lang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `opal_lang-2024.5.10.2/src/opal_lang.egg-info/SOURCES.txt` & `opal_lang-2024.5.10.3/src/opal_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

