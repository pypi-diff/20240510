# Comparing `tmp/reasonify_headless-0.0.2.1.tar.gz` & `tmp/reasonify_headless-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.0.2.1.tar", last modified: Fri Mar 29 15:09:46 2024, max compression
+gzip compressed data, was "reasonify_headless-0.0.2.2.tar", last modified: Fri May 10 04:05:53 2024, max compression
```

## Comparing `reasonify_headless-0.0.2.1.tar` & `reasonify_headless-0.0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1080 2024-03-29 15:09:46.230219 reasonify_headless-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0       48 2024-03-25 14:26:26.453867 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0      292 2024-03-25 15:04:55.582491 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/core/__init__.py
--rw-r--r--   0        0        0     1209 2024-03-26 00:02:57.861753 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/core/step2.py
--rw-r--r--   0        0        0     1393 2024-03-26 00:33:20.953112 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/core/step3.py
--rw-r--r--   0        0        0     1274 2024-03-26 05:15:49.768522 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/core/step4.py
--rw-r--r--   0        0        0      177 2024-03-24 14:16:00.867731 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/models/tool.py
--rw-r--r--   0        0        0      403 2024-03-25 11:32:08.766310 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/showTools.j2
--rw-r--r--   0        0        0     1677 2024-03-28 04:46:45.440890 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step2.j2
--rw-r--r--   0        0        0      177 2024-03-26 01:07:53.525616 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step2schema.ts
--rw-r--r--   0        0        0     1242 2024-03-28 04:50:40.795708 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step3.j2
--rw-r--r--   0        0        0      567 2024-03-28 05:00:02.253057 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step3schema.ts
--rw-r--r--   0        0        0     1137 2024-03-29 15:06:27.426080 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step4a.j2
--rw-r--r--   0        0        0     1010 2024-03-29 14:51:23.953890 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step4b.j2
--rw-r--r--   0        0        0      285 2024-03-23 04:02:17.167768 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step4bschema.ts
--rw-r--r--   0        0        0     1797 2024-03-26 01:06:37.522415 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0     1493 2024-03-29 14:37:14.879972 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/utils/globals.py
--rw-r--r--   0        0        0       79 2024-03-16 05:46:45.084890 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/utils/resolve.py
--rw-r--r--   0        0        0      204 2024-03-25 02:21:06.206815 reasonify_headless-0.0.2.1/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 reasonify_headless-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1154 2024-05-10 04:05:53.939738 reasonify_headless-0.0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-03-25 14:26:26.453867 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-01 15:41:30.934449 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/__init__.py
+-rw-r--r--   0        0        0     1209 2024-04-01 15:39:10.607693 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step2.py
+-rw-r--r--   0        0        0     1410 2024-05-10 03:39:16.452275 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step3.py
+-rw-r--r--   0        0        0     1274 2024-03-26 05:15:49.768522 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step4.py
+-rw-r--r--   0        0        0      177 2024-05-10 03:28:17.853720 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/models/tool.py
+-rw-r--r--   0        0        0      403 2024-03-25 11:32:08.766310 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/showTools.j2
+-rw-r--r--   0        0        0     1677 2024-03-28 04:46:45.440890 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step2.j2
+-rw-r--r--   0        0        0      177 2024-03-30 10:40:21.464187 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step2schema.ts
+-rw-r--r--   0        0        0     1242 2024-03-28 04:50:40.795708 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step3.j2
+-rw-r--r--   0        0        0      582 2024-03-30 10:40:21.464187 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step3schema.ts
+-rw-r--r--   0        0        0     1137 2024-03-29 15:06:27.426080 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4a.j2
+-rw-r--r--   0        0        0     1010 2024-03-29 14:51:23.953890 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4b.j2
+-rw-r--r--   0        0        0      299 2024-03-30 10:40:21.464187 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4bschema.ts
+-rw-r--r--   0        0        0     1797 2024-05-10 03:24:31.466362 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0     1503 2024-03-30 11:05:27.898676 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/globals.py
+-rw-r--r--   0        0        0       79 2024-03-16 05:46:45.084890 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/resolve.py
+-rw-r--r--   0        0        0      204 2024-03-25 02:21:06.206815 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 reasonify_headless-0.0.2.2/PKG-INFO
```

### Comparing `reasonify_headless-0.0.2.1/pyproject.toml` & `reasonify_headless-0.0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 description = "headless implementation for the Reasonify Agent"
 dynamic = []
 requires-python = ">=3.10"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
-    "promplate~=0.3.3.4",
+    "promplate~=0.3.4.4",
     "python-box~=7.1.1",
     "promptools[validation]~=0.1.3.2",
 ]
-version = "0.0.2.1"
+version = "0.0.2.2"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -30,21 +30,22 @@
 
 [tool.pdm.version]
 source = "file"
 path = "reasonify-headless/version.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=24.3.0",
+    "black>=24.4.2",
     "isort>=5.13.2",
-    "ruff>=0.3.3",
+    "ruff>=0.4.4",
     "watchfiles>=0.21.0",
-    "promplate-pyodide~=0.0.3",
+    "promplate-pyodide~=0.0.3.2",
     "micropip~=0.6.0",
-    "pyodide-py~=0.25.0",
+    "pyodide-py~=0.25.1",
+    "webtypy~=0.1.7",
 ]
 
 [tool.pdm.scripts.fmt]
 composite = [
     "ruff check --fix --exit-zero",
     "isort .",
     "black .",
@@ -55,7 +56,10 @@
     "watchfiles",
     "pdm build --no-sdist -d static/whl",
     "reasonify-headless",
 ]
 
 [tool.black]
 line-length = 120
+
+[tool.pyright]
+reportMissingModuleSource = false
```

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/core/step2.py` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step2.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/core/step3.py` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step3.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class Step3Schema(TypedDict):
     note: str
     actions: list[Action]
 
     # from parents
-    tools: list[Tool]
+    tools: NotRequired[list[Tool]]
 
 
 @step3.mid_process
 def parse(context):
     c = Context(context)
     parsed = c.extract_json({}, Step3Schema)
 
@@ -45,11 +45,11 @@
 @step3.end_process
 async def run_tools(context):
     c = cast(Step3Schema, Context(context))
     if not c["actions"]:
         raise Jump(step3)  # fail to generate actions
 
     for action in c["actions"]:
-        for tool in cast(list[Tool], c["tools"]):
+        for tool in cast(list[Tool], c.get("tools")):
             if tool["id"] == action["tool_id"]:
                 action["tool"] = tool
                 action["result"] = await resolve(tool["run"](**action["payload"]))
```

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/core/step4.py` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step4.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step2.j2` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step2.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step3.j2` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step3.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step4a.j2` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4a.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/templates/step4b.j2` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4b.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/context.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.0.2.1/reasonify-headless/reasonify/utils/globals.py` & `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,12 +40,12 @@
 def make_context(context: Context | None = None):
     if context is None:
         return ChainMap(*static_layers, defaultdict(SilentBox))
     return ChainMap(dict(SilentBox(context)), *static_layers, defaultdict(SilentBox))
 
 
 class DotTemplate(Template):
-    def render(self, context):
+    def render(self, context=None):
         return super().render(make_context(context))
 
-    async def arender(self, context):
+    async def arender(self, context=None):
         return await super().arender(make_context(context))
```

