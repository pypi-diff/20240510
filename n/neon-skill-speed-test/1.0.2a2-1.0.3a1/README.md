# Comparing `tmp/neon-skill-speed_test-1.0.2a2.tar.gz` & `tmp/neon-skill-speed_test-1.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-speed_test-1.0.2a2.tar", last modified: Tue Apr  2 20:54:34 2024, max compression
+gzip compressed data, was "neon-skill-speed_test-1.0.3a1.tar", last modified: Fri May 10 17:32:06 2024, max compression
```

## Comparing `neon-skill-speed_test-1.0.2a2.tar` & `neon-skill-speed_test-1.0.3a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/notify_testing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/results.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/start_test.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/intent/run_speed_test.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:32:06.187602 neon-skill-speed_test-1.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-10 17:32:06.187602 neon-skill-speed_test-1.0.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:32:06.183602 neon-skill-speed_test-1.0.3a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:32:06.183602 neon-skill-speed_test-1.0.3a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:32:06.187602 neon-skill-speed_test-1.0.3a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/locale/en-us/dialog/notify_testing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/locale/en-us/dialog/results.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/locale/en-us/dialog/start_test.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:32:06.187602 neon-skill-speed_test-1.0.3a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/locale/en-us/intent/run_speed_test.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:32:06.187602 neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-10 17:32:06.000000 neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 17:32:06.000000 neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:32:06.000000 neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-10 17:32:06.000000 neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-10 17:32:06.000000 neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 17:32:06.000000 neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:32:06.187602 neon-skill-speed_test-1.0.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:32:06.187602 neon-skill-speed_test-1.0.3a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-10 17:32:03.000000 neon-skill-speed_test-1.0.3a1/version.py
```

### Comparing `neon-skill-speed_test-1.0.2a2/LICENSE.md` & `neon-skill-speed_test-1.0.3a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a2/PKG-INFO` & `neon-skill-speed_test-1.0.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speed_test
-Version: 1.0.2a2
+Version: 1.0.3a1
 Home-page: https://github.com/NeonGeckoCom/skill-speed_test
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-speed_test-1.0.2a2/README.md` & `neon-skill-speed_test-1.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a2/__init__.py` & `neon-skill-speed_test-1.0.3a1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 import speedtest
 
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from neon_utils.skills.neon_skill import NeonSkill
-
-from mycroft.skills import intent_file_handler
+from ovos_workshop.decorators import intent_handler
 
 
 class SpeedTestSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
         self._test = None
         try:
@@ -61,15 +60,15 @@
                                    requires_internet=True,
                                    requires_network=True,
                                    requires_gui=False,
                                    no_internet_fallback=False,
                                    no_network_fallback=False,
                                    no_gui_fallback=True)
 
-    @intent_file_handler("run_speed_test.intent")
+    @intent_handler("run_speed_test.intent")
     def handle_run_speed_test(self, message):
         self.speak_dialog("start_test")
         self.bus.emit(message.forward(
             "ovos.notification.api.set.controlled",
             {"sender": self.skill_id,
              "text": self.translate("notify_testing")}))
         self.test.download()
```

### Comparing `neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/PKG-INFO` & `neon-skill-speed_test-1.0.3a1/neon_skill_speed_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speed-test
-Version: 1.0.2a2
+Version: 1.0.3a1
 Home-page: https://github.com/NeonGeckoCom/skill-speed_test
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-speed_test-1.0.2a2/setup.py` & `neon-skill-speed_test-1.0.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a2/skill.json` & `neon-skill-speed_test-1.0.3a1/skill.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'requirements'": "{'python': {insert: [(3, 'ovos-workshop~=0.0.15')]}}"}*

```diff
@@ -29,14 +29,15 @@
         "arm"
     ],
     "requirements": {
         "python": [
             "neon-utils~=1.0",
             "ovos-bus-client~=0.0.3",
             "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15",
             "speedtest-cli~=2.1"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Skill used to test your internet speed",
     "skillname": "skill-speed_test",
```

### Comparing `neon-skill-speed_test-1.0.2a2/test/test_skill.py` & `neon-skill-speed_test-1.0.3a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a2/version.py` & `neon-skill-speed_test-1.0.3a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.2a2"
+__version__ = "1.0.3a1"
```

