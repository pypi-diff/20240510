# Comparing `tmp/neon-skill-communication-0.1.1a3.tar.gz` & `tmp/neon-skill-communication-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-communication-0.1.1a3.tar", last modified: Thu Feb  1 21:51:42 2024, max compression
+gzip compressed data, was "neon-skill-communication-0.1.1a4.tar", last modified: Fri May 10 17:36:35 2024, max compression
```

## Comparing `neon-skill-communication-0.1.1a3.tar` & `neon-skill-communication-0.1.1a4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:51:42.100124 neon-skill-communication-0.1.1a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-01 21:51:42.100124 neon-skill-communication-0.1.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13462 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:51:42.096124 neon-skill-communication-0.1.1a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:51:42.096124 neon-skill-communication-0.1.1a3/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:51:42.100124 neon-skill-communication-0.1.1a3/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/locale/en-us/dialog/cant_call.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/locale/en-us/dialog/cant_send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/locale/en-us/dialog/one_moment.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:51:42.100124 neon-skill-communication-0.1.1a3/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/locale/en-us/vocab/call.intent
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/locale/en-us/vocab/draft.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/locale/en-us/vocab/message.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/locale/en-us/vocab/neon.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:51:42.100124 neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-01 21:51:42.000000 neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-01 21:51:42.000000 neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 21:51:42.000000 neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-01 21:51:42.000000 neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-01 21:51:42.000000 neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-01 21:51:42.000000 neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 21:51:42.100124 neon-skill-communication-0.1.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:51:42.100124 neon-skill-communication-0.1.1a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-01 21:51:38.000000 neon-skill-communication-0.1.1a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:35.255783 neon-skill-communication-0.1.1a4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 17:36:35.255783 neon-skill-communication-0.1.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13446 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:35.251783 neon-skill-communication-0.1.1a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:35.251783 neon-skill-communication-0.1.1a4/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:35.251783 neon-skill-communication-0.1.1a4/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/locale/en-us/dialog/cant_call.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/locale/en-us/dialog/cant_send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/locale/en-us/dialog/one_moment.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:35.251783 neon-skill-communication-0.1.1a4/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/locale/en-us/vocab/call.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/locale/en-us/vocab/draft.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/locale/en-us/vocab/message.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/locale/en-us/vocab/neon.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:35.255783 neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 17:36:35.000000 neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-10 17:36:35.000000 neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:36:35.000000 neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-10 17:36:35.000000 neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 17:36:35.000000 neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 17:36:35.000000 neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:36:35.255783 neon-skill-communication-0.1.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:35.255783 neon-skill-communication-0.1.1a4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-10 17:36:32.000000 neon-skill-communication-0.1.1a4/version.py
```

### Comparing `neon-skill-communication-0.1.1a3/LICENSE.md` & `neon-skill-communication-0.1.1a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a3/PKG-INFO` & `neon-skill-communication-0.1.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-communication
-Version: 0.1.1a3
+Version: 0.1.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-communication
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-communication-0.1.1a3/README.md` & `neon-skill-communication-0.1.1a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a3/__init__.py` & `neon-skill-communication-0.1.1a4/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from threading import Lock
 from adapt.intent import IntentBuilder
 from ovos_utils.log import LOG
 from ovos_utils import classproperty
 from ovos_utils.process_utils import RuntimeRequirements
 from neon_utils.skills.neon_skill import NeonSkill
 from neon_utils.signal_utils import check_for_signal
-from mycroft.skills import intent_handler, intent_file_handler
+from ovos_workshop.decorators import intent_handler
 
 
 class CommunicationSkill(NeonSkill):
     def __init__(self, **kwargs):
         super(CommunicationSkill, self).__init__(**kwargs)
         self.query_replies = {}
         self.query_extensions = {}
@@ -57,15 +57,15 @@
 
     def initialize(self):
         self.add_event("communication:request.call.response",
                        self.handle_place_call_response)
         self.add_event("communication:request.message.response",
                        self.handle_send_message_response)
 
-    @intent_file_handler("call.intent")
+    @intent_handler("call.intent")
     def handle_place_call(self, message):
         if self.neon_in_request(message):
             # TODO: Move hesitation to user preference DM
             if check_for_signal('CORE_useHesitation', -1):
                 self.speak_dialog("one_moment")
             utt = message.data.get("utterance")
             request = message.data.get("contact")
```

### Comparing `neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/PKG-INFO` & `neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-communication
-Version: 0.1.1a3
+Version: 0.1.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-communication
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-communication-0.1.1a3/neon_skill_communication.egg-info/SOURCES.txt` & `neon-skill-communication-0.1.1a4/neon_skill_communication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a3/setup.py` & `neon-skill-communication-0.1.1a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a3/skill.json` & `neon-skill-communication-0.1.1a4/skill.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060607%*

 * *Differences: {"'requirements'": "{'python': {insert: [(0, 'adapt-parser<2.0,>=0.5'), (3, "*

 * *                   "'ovos-workshop~=0.0.15')]}}"}*

```diff
@@ -19,16 +19,18 @@
         "x86_64",
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
+            "adapt-parser<2.0,>=0.5",
             "neon-utils~=1.0",
-            "ovos-utils~=0.0, >=0.0.28"
+            "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Skill for the Common Message Skill framework.",
     "skillname": "skill-communication",
     "summary": "Skill for the Common Message Skill framework.",
```

### Comparing `neon-skill-communication-0.1.1a3/test/test_skill.py` & `neon-skill-communication-0.1.1a4/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a3/version.py` & `neon-skill-communication-0.1.1a4/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a3"
+__version__ = "0.1.1a4"
```

