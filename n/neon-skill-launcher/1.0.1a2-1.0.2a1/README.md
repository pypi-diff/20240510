# Comparing `tmp/neon-skill-launcher-1.0.1a2.tar.gz` & `tmp/neon-skill-launcher-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-launcher-1.0.1a2.tar", last modified: Wed Apr  3 19:00:04 2024, max compression
+gzip compressed data, was "neon-skill-launcher-1.0.2a1.tar", last modified: Fri May 10 17:34:20 2024, max compression
```

## Comparing `neon-skill-launcher-1.0.1a2.tar` & `neon-skill-launcher-1.0.2a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.805920 neon-skill-launcher-1.0.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.805920 neon-skill-launcher-1.0.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/launch_program.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/launch_website.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/mobile_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/on.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/website_not_found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/regex/website.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/browse.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/launch.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/launch_program.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.916202 neon-skill-launcher-1.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-10 17:34:20.916202 neon-skill-launcher-1.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.912202 neon-skill-launcher-1.0.2a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.912202 neon-skill-launcher-1.0.2a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.912202 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/launch_program.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/launch_website.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/mobile_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/on.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/dialog/website_not_found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.912202 neon-skill-launcher-1.0.2a1/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/regex/website.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.916202 neon-skill-launcher-1.0.2a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/vocab/browse.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/vocab/launch.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/locale/en-us/vocab/launch_program.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.916202 neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-10 17:34:20.000000 neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-10 17:34:20.000000 neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:34:20.000000 neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 17:34:20.000000 neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-10 17:34:20.000000 neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 17:34:20.000000 neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:34:20.916202 neon-skill-launcher-1.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:20.916202 neon-skill-launcher-1.0.2a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-10 17:34:17.000000 neon-skill-launcher-1.0.2a1/version.py
```

### Comparing `neon-skill-launcher-1.0.1a2/LICENSE.md` & `neon-skill-launcher-1.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a2/PKG-INFO` & `neon-skill-launcher-1.0.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-launcher
-Version: 1.0.1a2
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-launcher
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-launcher-1.0.1a2/README.md` & `neon-skill-launcher-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a2/__init__.py` & `neon-skill-launcher-1.0.2a1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 from ovos_utils import classproperty
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_utils.log import LOG
 from ovos_utils.gui import is_gui_installed
 from neon_utils.message_utils import request_from_mobile
 from neon_utils.skills.neon_skill import NeonSkill
 from neon_utils.web_utils import scrape_page_for_links as scrape
-
-from mycroft.skills import intent_handler, intent_file_handler
+from ovos_workshop.decorators import intent_handler
 
 
 class LauncherSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
         self.valid_domains = ('com', 'net', 'org', 'edu', 'gov', 'ai', 'us',
                               'tech')
@@ -58,15 +57,15 @@
                                    requires_internet=True,
                                    requires_network=True,
                                    requires_gui=True,
                                    no_internet_fallback=False,
                                    no_network_fallback=False,
                                    no_gui_fallback=False)
 
-    @intent_file_handler("launch_program.intent")
+    @intent_handler("launch_program.intent")
     def handle_launch_program(self, message):
         """
         Handle a request to launch a specific program
         """
         if not self.neon_in_request(message):
             return
         if message.context.get("mobile"):
```

### Comparing `neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/PKG-INFO` & `neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-launcher
-Version: 1.0.1a2
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-launcher
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/SOURCES.txt` & `neon-skill-launcher-1.0.2a1/neon_skill_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a2/setup.py` & `neon-skill-launcher-1.0.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a2/skill.json` & `neon-skill-launcher-1.0.2a1/skill.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984848484848485%*

 * *Differences: {"'requirements'": "{'python': {insert: [(0, 'adapt-parser<2.0,>=0.5'), (4, "*

 * *                   "'ovos-workshop~=0.0.15')]}}"}*

```diff
@@ -26,17 +26,19 @@
         "x86_64",
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
+            "adapt-parser<2.0,>=0.5",
             "neon-utils[network]~=1.0",
             "ovos-bus-client~=0.0.3",
-            "ovos-utils~=0.0, >=0.0.28"
+            "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Browse the web by voice",
     "skillname": "skill-launcher",
     "summary": "Browse the web by voice",
```

### Comparing `neon-skill-launcher-1.0.1a2/test/test_skill.py` & `neon-skill-launcher-1.0.2a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a2/version.py` & `neon-skill-launcher-1.0.2a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a2"
+__version__ = "1.0.2a1"
```

