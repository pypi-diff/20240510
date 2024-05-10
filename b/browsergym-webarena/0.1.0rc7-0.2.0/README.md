# Comparing `tmp/browsergym_webarena-0.1.0rc7.tar.gz` & `tmp/browsergym_webarena-0.2.0.tar.gz`

## Comparing `browsergym_webarena-0.1.0rc7.tar` & `browsergym_webarena-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/requirements.txt
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/src/browsergym/webarena/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/src/browsergym/webarena/config.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/src/browsergym/webarena/instance.py
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/src/browsergym/webarena/task.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/tests/test_env_general.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/tests/test_instance.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/tests/utils.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/.gitignore
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/README.md
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/pyproject.toml
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 browsergym_webarena-0.1.0rc7/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/src/browsergym/webarena/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/src/browsergym/webarena/config.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/src/browsergym/webarena/instance.py
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/src/browsergym/webarena/task.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/tests/test_env_general.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/tests/test_instance.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/.gitignore
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/README.md
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 browsergym_webarena-0.2.0/PKG-INFO
```

### Comparing `browsergym_webarena-0.1.0rc7/src/browsergym/webarena/instance.py` & `browsergym_webarena-0.2.0/src/browsergym/webarena/instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,7 +95,16 @@
                 username = self.credentials[site]["username"]
                 password = self.credentials[site]["password"]
 
                 page.goto(url)
                 page.get_by_label("Username").fill(username)
                 page.get_by_label("Password").fill(password)
                 page.get_by_role("button", name="Sign in").click()
+
+            case "wikipedia":
+                page.goto(url)
+
+            case "map":
+                page.goto(url)
+
+            case _:
+                raise ValueError
```

### Comparing `browsergym_webarena-0.1.0rc7/src/browsergym/webarena/task.py` & `browsergym_webarena-0.2.0/src/browsergym/webarena/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,27 @@
     """
     Base class for all WebArena tasks.
 
     """
 
     def __init__(
         self,
+        seed: int,
         task_id: Optional[int] = None,
         intent_template_id: Optional[int] = None,
         with_na_hint: bool = False,
         with_homepage_hint: bool = False,
     ) -> None:
+        super().__init__(seed)
+
+        # task properties, will be used to set up the browsergym environment
+        self.viewport = {"width": 1280, "height": 720}
+        self.slow_mo = 1000  # ms
+        self.timeout = 10000  # ms
+
         self.webarena_instance = WebArenaInstance()
         self.config_file: str = None
         self.with_na_hint = with_na_hint
         self.with_homepage_hint = with_homepage_hint
 
         # one and only one of task id and template id must be provided
         if (task_id is None) == (intent_template_id is None):
@@ -70,20 +78,18 @@
             if not task_configs:
                 raise ValueError(
                     f"Could not find any task config with task_id={intent_template_id}."
                 )
 
         self.task_configs = task_configs
 
-    def setup(self, seed: int, page: playwright.sync_api.Page) -> tuple[str, dict]:
+    def setup(self, page: playwright.sync_api.Page) -> tuple[str, dict]:
         # import webarena on instanciation
         from webarena.evaluation_harness.evaluators import evaluator_router
 
-        self.random = np.random.RandomState(seed)
-
         # pick a task at random
         self.config = self.random.choice(self.task_configs)
 
         # hack: dynamically build a config file to read from
         with tempfile.NamedTemporaryFile(mode="w+", delete=False) as f:
             json.dump(self.config, f)
             f.flush()
```

### Comparing `browsergym_webarena-0.1.0rc7/tests/test_env_general.py` & `browsergym_webarena-0.2.0/tests/test_env_general.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.1.0rc7/tests/test_instance.py` & `browsergym_webarena-0.2.0/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.1.0rc7/tests/utils.py` & `browsergym_webarena-0.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.1.0rc7/README.md` & `browsergym_webarena-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.1.0rc7/pyproject.toml` & `browsergym_webarena-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.1.0rc7/PKG-INFO` & `browsergym_webarena-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-webarena
-Version: 0.1.0rc7
+Version: 0.2.0
 Summary: WebArena benchmark for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Maxime Gasse, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
-Requires-Dist: browsergym-core==0.1.0rc7
+Requires-Dist: browsergym-core==0.2.0
 Requires-Dist: libwebarena==0.0.2
 Description-Content-Type: text/markdown
 
 # WebArena benchmark for BrowserGym
 
 This package provides `browsergym.webarena`, which is an unofficial port of the [WebArena](https://webarena.dev/) benchmark for BrowserGym.
```

