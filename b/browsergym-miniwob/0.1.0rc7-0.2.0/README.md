# Comparing `tmp/browsergym_miniwob-0.1.0rc7.tar.gz` & `tmp/browsergym_miniwob-0.2.0.tar.gz`

## Comparing `browsergym_miniwob-0.1.0rc7.tar` & `browsergym_miniwob-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/requirements.txt
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/src/browsergym/miniwob/__init__.py
--rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/src/browsergym/miniwob/all.py
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/src/browsergym/miniwob/base.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/tests/test_base.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/tests/test_click-scroll-list.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/tests/test_use-colorwheel-2.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/tests/utils.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/.gitignore
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/pyproject.toml
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 browsergym_miniwob-0.1.0rc7/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/src/browsergym/miniwob/__init__.py
+-rw-r--r--   0        0        0    19080 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/src/browsergym/miniwob/all.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/src/browsergym/miniwob/base.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/tests/test_base.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/tests/test_click-menu-2.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/tests/test_click-scroll-list.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/tests/test_use-colorwheel-2.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/.gitignore
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.0/PKG-INFO
```

### Comparing `browsergym_miniwob-0.1.0rc7/src/browsergym/miniwob/__init__.py` & `browsergym_miniwob-0.2.0/src/browsergym/miniwob/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0rc7"
+__version__ = "0.2.0"
 
 from browsergym.core.registration import register_task
 
 from . import all
 
 ALL_MINIWOB_TASKS = [
     all.AscendingNumbersTask,
@@ -133,9 +133,9 @@
 ]
 
 # register the Miniwob benchmark
 for task in ALL_MINIWOB_TASKS:
     register_task(
         task.get_task_id(),
         task,
-        kwargs={"viewport": {"width": 500, "height": 320}, "slow_mo": 100},
+        nondeterministic=task.nondeterministic,
     )
```

### Comparing `browsergym_miniwob-0.1.0rc7/src/browsergym/miniwob/all.py` & `browsergym_miniwob-0.2.0/src/browsergym/miniwob/all.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,47 @@
     subdomain = "click-menu"
 
 
 class ClickMenu2Task(AbstractMiniwobTask):
     desc = "Find a specific item from a menu."
     subdomain = "click-menu-2"
 
+    def setup(self, page: playwright.sync_api.Page) -> tuple[str, dict]:
+        goal, info = super().setup(page)
+
+        if self.remove_human_display:
+            get_utterance_func = "getUtterance_legacy"
+        else:
+            get_utterance_func = "getUtterance"
+
+        # this task requires specific treatment to recover the text goal
+        page.evaluate(
+            f"core.{get_utterance_func} = function () "
+            + r"""{
+    query_div = document.getElementById('query');
+    if (query_div.children.length > 0) {
+        utterance = '';
+        utterance = utterance + query_div.childNodes[0].textContent.replace(/\s+/g, ' ').trim();
+        utterance = utterance + ' "' + query_div.children[0].getAttribute('class').split(' ')[1] + '"';
+        utterance = utterance + ' ' + query_div.childNodes[2].textContent.replace(/\s+/g, ' ').trim();
+    }
+    else {
+        utterance = query_div.textContent.replace(/\s+/g, ' ').trim();
+    }
+    return utterance;
+};
+'';
+"""
+        )
+
+        # re-extract the goal
+        goal = self._get_goal()
+
+        return goal, info
+
 
 class ClickOptionTask(AbstractMiniwobTask):
     desc = "Click option boxes."
     subdomain = "click-option"
 
 
 class ClickPieTask(AbstractMiniwobTask):
@@ -606,16 +639,16 @@
     subdomain = "use-colorwheel"
 
 
 class UseColorwheel2Task(AbstractMiniwobTask):
     desc = "Use a color wheel given specific random color."
     subdomain = "use-colorwheel-2"
 
-    def setup(self, seed: int, page: playwright.sync_api.Page) -> tuple[str, dict]:
-        goal, info = super().setup(seed, page)
+    def setup(self, page: playwright.sync_api.Page) -> tuple[str, dict]:
+        goal, info = super().setup(page)
 
         if self.remove_human_display:
             get_utterance_func = "getUtterance_legacy"
         else:
             get_utterance_func = "getUtterance"
 
         # this task requires specific treatment to recover the text goal
```

### Comparing `browsergym_miniwob-0.1.0rc7/src/browsergym/miniwob/base.py` & `browsergym_miniwob-0.2.0/src/browsergym/miniwob/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,33 +7,43 @@
 
 class AbstractMiniwobTask(AbstractBrowserTask):
     """
     Abstract class for all Miniwob++ tasks
 
     """
 
-    nondeterministic = False
+    # gym metadata (default value, can be overloaded per task)
+    nondeterministic: bool = False
 
     @classmethod
     def get_task_id(cls):
         return f"miniwob.{cls.subdomain}"
 
     def __init__(
         self,
+        seed: int,
         base_url: Optional[str] = None,
         episode_max_time: int = 1000000,
         remove_human_display: bool = True,
     ) -> None:
         """
         Args:
+            seed: random seed.
             base_url: str (optional), the base Miniwob URL where the task's HTML file is to be found. If not provided, the MINIWOB_URL environment variable will be used.
             episode_max_time: int, episode max time in milliseconds. Default: 1000000 ms.
             remove_human_display: bool, whether or not to remove the human display (goal, time left, last reward etc.) from the DOM. Default: True.
 
         """
+        super().__init__(seed)
+
+        # task properties, will be used to set up the browsergym environment
+        self.viewport = {"width": 500, "height": 320}
+        self.slow_mo = 100  # ms
+        self.timeout = 5000  # ms
+
         assert episode_max_time > 0
 
         # if not provided, try to get Miniwob URL from environment variable
         if base_url is None:
             if "MINIWOB_URL" in os.environ:
                 base_url = os.environ["MINIWOB_URL"]
             else:
@@ -41,15 +51,15 @@
                     f"Please provide a Miniwob base URL (or setup one using the environment variable MINIWOB_URL)."
                 )
 
         self.url = base_url + self.subdomain + ".html"
         self.episode_max_time = episode_max_time
         self.remove_human_display = remove_human_display
 
-    def setup(self, seed: int, page: playwright.sync_api.Page) -> tuple[str, dict]:
+    def setup(self, page: playwright.sync_api.Page) -> tuple[str, dict]:
         self.page = page
 
         # navigate to the task's url
         self.page.goto(self.url)
 
         # remove human display if requested (goal, time left, last reward etc.)
         if self.remove_human_display:
@@ -114,15 +124,15 @@
         # start the task
         self.page.evaluate(
             r"""
 Math.seedrandom({seed});
 core.EPISODE_MAX_TIME = {episode_max_time};
 core.startEpisodeReal();
 """.format(
-                seed=seed,
+                seed=self.random.randint(0, 1000000),
                 episode_max_time=self.episode_max_time,
             )
         )
 
         # wait for the Miniwob task to have status ready
         self.page.wait_for_function(r"""() => WOB_TASK_READY""")
```

### Comparing `browsergym_miniwob-0.1.0rc7/tests/test_base.py` & `browsergym_miniwob-0.2.0/tests/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 def test_validate_teardown(task_cls):
     pw = browsergym.core._get_global_playwright()
 
     browser = pw.chromium.launch(headless=__HEADLESS, slow_mo=__SLOW_MO)
     context = browser.new_context()
     page = context.new_page()
 
-    task = task_cls()
-    task.setup(seed=42, page=page)
+    task = task_cls(seed=42)
+    task.setup(page=page)
 
     reward, done, msg, info = task.validate(page, [])
 
     assert done is False
 
     task.teardown()
 
@@ -47,16 +47,16 @@
 def test_episode_max_time(task_cls):
     pw = browsergym.core._get_global_playwright()
 
     browser = pw.chromium.launch(headless=__HEADLESS, slow_mo=__SLOW_MO)
     context = browser.new_context()
     page = context.new_page()
 
-    task = task_cls(episode_max_time=0.2)
-    task.setup(seed=42, page=page)
+    task = task_cls(seed=42, episode_max_time=0.2)
+    task.setup(page=page)
 
     time.sleep(0.5)
 
     reward, done, msg, info = task.validate(page, [])
 
     assert done is True
     assert reward == 0
@@ -74,16 +74,16 @@
     browser = pw.chromium.launch(headless=__HEADLESS, slow_mo=__SLOW_MO)
 
     # remove display
 
     context = browser.new_context()
     page = context.new_page()
 
-    task = task_cls(remove_human_display=True)
-    task.setup(seed=42, page=page)
+    task = task_cls(seed=42, remove_human_display=True)
+    task.setup(page=page)
 
     for element_id in ["reward-display", "click-canvas", "sync-task-cover"]:
         element_in_dom = page.evaluate(f"!!document.getElementById('{element_id}')")
         assert not element_in_dom
 
     assert page.evaluate(f"document.getElementById('query').innerHTML") == ""
 
@@ -96,16 +96,16 @@
     context.close()
 
     # keep display
 
     context = browser.new_context()
     page = context.new_page()
 
-    task = task_cls(remove_human_display=False)
-    task.setup(seed=42, page=page)
+    task = task_cls(seed=42, remove_human_display=False)
+    task.setup(page=page)
 
     for element_id in ["reward-display", "click-canvas", "sync-task-cover"]:
         element_in_dom = page.evaluate(f"!!document.getElementById('{element_id}')")
         assert element_in_dom
 
     assert page.evaluate(f"document.getElementById('query').innerHTML") != ""
```

### Comparing `browsergym_miniwob-0.1.0rc7/tests/test_click-scroll-list.py` & `browsergym_miniwob-0.2.0/tests/test_click-scroll-list.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.1.0rc7/tests/test_use-colorwheel-2.py` & `browsergym_miniwob-0.2.0/tests/test_use-colorwheel-2.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.1.0rc7/tests/utils.py` & `browsergym_miniwob-0.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.1.0rc7/README.md` & `browsergym_miniwob-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.1.0rc7/pyproject.toml` & `browsergym_miniwob-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.1.0rc7/PKG-INFO` & `browsergym_miniwob-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-miniwob
-Version: 0.1.0rc7
+Version: 0.2.0
 Summary: MiniWoB++ benchmark for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Rim Assouel, Maxime Gasse, Tom Marty
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
 Description-Content-Type: text/markdown
 
 # Miniwob benchmark for BrowserGym
 
 This package provides `browsergym.miniwob`, which is an unofficial port of the [MiniWoB++](https://miniwob.farama.org/) benchmark for BrowserGym.
 
 ## Setup
```

