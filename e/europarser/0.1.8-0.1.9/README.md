# Comparing `tmp/europarser-0.1.8.tar.gz` & `tmp/europarser-0.1.9.tar.gz`

## Comparing `europarser-0.1.8.tar` & `europarser-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 europarser-0.1.8/.dockerignore
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 europarser-0.1.8/Dockerfile
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 europarser-0.1.8/README_en.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 europarser-0.1.8/docker_log.conf
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 europarser-0.1.8/log.conf
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.8/pyinstaller.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 europarser-0.1.8/start_europarser.sh
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 europarser-0.1.8/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 europarser-0.1.8/.github/workflows/hatch-build-and-publish.yml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/__init__.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/daniel_light.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/endpoint.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/lang_detect.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/main.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/models.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/pipeline.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/pivot.py
--rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/api.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/utils.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/basic.min.css
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/dropzone.min.css
--rw-r--r--   0        0        0   114649 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/dropzone.min.js
--rw-r--r--   0        0        0    39237 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/favicon.ico
--rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/templates/main.html
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_csv.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_excel.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_gephi.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_iramuteq.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_json.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_markdown.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_stats.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_txm.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/transformer.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 europarser-0.1.8/tests/api_tester.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 europarser-0.1.8/.gitignore
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 europarser-0.1.8/.hgignore
--rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 europarser-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 europarser-0.1.8/README.md
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 europarser-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 europarser-0.1.9/.dockerignore
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 europarser-0.1.9/Dockerfile
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 europarser-0.1.9/README_en.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 europarser-0.1.9/docker_log.conf
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 europarser-0.1.9/log.conf
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.9/pyinstaller.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 europarser-0.1.9/start_europarser.sh
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 europarser-0.1.9/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 europarser-0.1.9/.github/workflows/hatch-build-and-publish.yml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/daniel_light.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/endpoint.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/lang_detect.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/main.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/models.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/pipeline.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/pivot.py
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/api.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/utils.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/static/basic.min.css
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/static/dropzone.min.css
+-rw-r--r--   0        0        0   114649 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/static/dropzone.min.js
+-rw-r--r--   0        0        0    39237 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/static/favicon.ico
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/api/templates/main.html
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_csv.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_excel.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_gephi.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_iramuteq.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_json.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_markdown.py
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_stats.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/to_txm.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 europarser-0.1.9/src/europarser/transformers/transformer.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 europarser-0.1.9/tests/api_tester.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 europarser-0.1.9/.gitignore
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 europarser-0.1.9/.hgignore
+-rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 europarser-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 europarser-0.1.9/README.md
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 europarser-0.1.9/PKG-INFO
```

### Comparing `europarser-0.1.8/Dockerfile` & `europarser-0.1.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/README_en.md` & `europarser-0.1.9/README_en.md`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/docker_log.conf` & `europarser-0.1.9/docker_log.conf`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/log.conf` & `europarser-0.1.9/log.conf`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/pyinstaller.py` & `europarser-0.1.9/pyinstaller.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/start_europarser.sh` & `europarser-0.1.9/start_europarser.sh`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/.github/workflows/docker-publish.yml` & `europarser-0.1.9/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/.github/workflows/hatch-build-and-publish.yml` & `europarser-0.1.9/.github/workflows/hatch-build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/daniel_light.py` & `europarser-0.1.9/src/europarser/daniel_light.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/endpoint.py` & `europarser-0.1.9/src/europarser/endpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,36 @@
 parser.add_argument("--support-journals", help="Minimal support for journals", type=int)
 parser.add_argument("--support-dates", help="Minimal support for dates", type=int)
 parser.add_argument("--support", help="Minimal support for all", type=int)
 parser.add_argument("--filter-keywords", help="Filter keywords", type=bool, default=False)
 parser.add_argument("--filter-lang", help="Filter language", type=bool, default=False)
 
 parser.add_argument("--api", help="Run as API", action="store_true")
-parser.add_argument("--host", default="127.0.0.1", help="Host to bind to")
-parser.add_argument("--port", default=8000, help="Port to bind to", type=int)
+parser.add_argument("--host", help="Host to bind to", type=str, optional=True)
+parser.add_argument("--port", help="Port to bind to", type=int, optional=True)
+parser.add_argument(
+    "--expose",
+    help="Expose the API (shorthand for --host 0.0.0.0 --port 8000), dosent override --host or --port if specified",
+    action="store_true"
+)
+
 
 parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
 
 def main():
     args = parser.parse_args()
 
-    if args.api or all([args.host, args.port]):
+    if args.api or all([args.host, args.port]) or args.expose:
         import uvicorn
         from .api import app
 
-        uvicorn.run(app, host=args.host, port=args.port)
+        if args.expose:
+            args.host = args.host or "0.0.0.0"
+
+        uvicorn.run(app, host=args.host or "127.0.0.1", port=args.port or 8000)
         exit(0)
 
     if args.cli:
         if not all([args.folder, args.output]):
             print("You need to specify a input folder and outputs")
             parser.print_help()
             exit(1)
```

### Comparing `europarser-0.1.8/src/europarser/main.py` & `europarser-0.1.9/src/europarser/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from pathlib import Path
 from typing import Optional
 
 from . import pipeline
 from .models import FileToTransform, TransformerOutput, Params, Output
 
 
-def main(folder: Path, outputs: list[Output], params: Optional[Params] = None) -> None:
+def main(folder: Path | str, outputs: list[Output], params: Optional[Params] = None) -> None:
     if params is None:
         params = Params()
 
+    if isinstance(folder, str):
+        folder = Path(folder)
+    elif not isinstance(folder, Path):
+        raise ValueError(f"folder must be a Path or a string, not {type(folder)}")
+
     # parse all files
     files = []
     for file in folder.iterdir():
+        if file.suffix.lower() != ".html":
+            print(f"Skipping {file.name} (not an HTML file)")
+            continue
         if file.is_file():
             with open(file, 'r', encoding='utf-8') as f:
                 files.append(FileToTransform(name=file.name, file=f.read()))
     print(f"Processing {len(files)} files...")
 
     # process result
     results: list[TransformerOutput] = pipeline(files, outputs, params=params)
```

### Comparing `europarser-0.1.8/src/europarser/models.py` & `europarser-0.1.9/src/europarser/models.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/pipeline.py` & `europarser-0.1.9/src/europarser/pipeline.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/pivot.py` & `europarser-0.1.9/src/europarser/pivot.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/utils.py` & `europarser-0.1.9/src/europarser/utils.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/api/api.py` & `europarser-0.1.9/src/europarser/api/api.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/api/utils.py` & `europarser-0.1.9/src/europarser/api/utils.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/api/static/basic.min.css` & `europarser-0.1.9/src/europarser/api/static/basic.min.css`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/api/static/dropzone.min.css` & `europarser-0.1.9/src/europarser/api/static/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/api/static/dropzone.min.js` & `europarser-0.1.9/src/europarser/api/static/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/api/static/favicon.ico` & `europarser-0.1.9/src/europarser/api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/api/templates/main.html` & `europarser-0.1.9/src/europarser/api/templates/main.html`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_csv.py` & `europarser-0.1.9/src/europarser/transformers/to_csv.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_excel.py` & `europarser-0.1.9/src/europarser/transformers/to_excel.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_gephi.py` & `europarser-0.1.9/src/europarser/transformers/to_gephi.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_iramuteq.py` & `europarser-0.1.9/src/europarser/transformers/to_iramuteq.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_json.py` & `europarser-0.1.9/src/europarser/transformers/to_json.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_markdown.py` & `europarser-0.1.9/src/europarser/transformers/to_markdown.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_stats.py` & `europarser-0.1.9/src/europarser/transformers/to_stats.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/to_txm.py` & `europarser-0.1.9/src/europarser/transformers/to_txm.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/src/europarser/transformers/transformer.py` & `europarser-0.1.9/src/europarser/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/tests/api_tester.py` & `europarser-0.1.9/tests/api_tester.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/.gitignore` & `europarser-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/LICENSE.txt` & `europarser-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/README.md` & `europarser-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/pyproject.toml` & `europarser-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.8/PKG-INFO` & `europarser-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: europarser
-Version: 0.1.8
+Version: 0.1.9
 Project-URL: Documentation, https://github.com/CERES-sorbonne/europarser#readme
 Project-URL: Issues, https://github.com/CERES-sorbonne/europarser/issues
 Project-URL: Source, https://github.com/CERES-sorbonne/europarser
 Author-email: Marceau <pypi@marceau-h.fr>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

