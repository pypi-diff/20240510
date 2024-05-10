# Comparing `tmp/neon-skill-camera-1.0.1a1.tar.gz` & `tmp/neon-skill-camera-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-camera-1.0.1a1.tar", last modified: Tue Feb  6 01:09:33 2024, max compression
+gzip compressed data, was "neon-skill-camera-1.0.2a1.tar", last modified: Fri May 10 19:20:10 2024, max compression
```

## Comparing `neon-skill-camera-1.0.1a1.tar` & `neon-skill-camera-1.0.2a1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17038 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.563944 neon-skill-camera-1.0.1a1/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/DefaultDuration.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/LaunchCamera.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/NoCamera.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/NothingToShow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/PictureInsteadOfVideo.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/ServerNotSupported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/ShowLatest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/StartRecording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/hour.list
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/minute.list
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/second.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/Camera.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/ControlBar.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/ui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/images/capture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/images/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)   341166 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/sounds/clicking.wav
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.563944 neon-skill-camera-1.0.1a1/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/ShowLastIntent.intent
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/TakePicIntent.intent
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/TakeVidIntent.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/duration.entity
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.393653 neon-skill-camera-1.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-10 19:20:10.393653 neon-skill-camera-1.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17038 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.385654 neon-skill-camera-1.0.2a1/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.389654 neon-skill-camera-1.0.2a1/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/DefaultDuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/LaunchCamera.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/NoCamera.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/NothingToShow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/PictureInsteadOfVideo.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/ServerNotSupported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/ShowLatest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/StartRecording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/hour.list
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/minute.list
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/dialog/en-us/second.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.389654 neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-10 19:20:10.000000 neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 19:20:10.000000 neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:20:10.000000 neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 19:20:10.000000 neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 19:20:10.000000 neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 19:20:10.000000 neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:20:10.393653 neon-skill-camera-1.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.393653 neon-skill-camera-1.0.2a1/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/ui/Camera.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/ui/ControlBar.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.393653 neon-skill-camera-1.0.2a1/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/ui/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/ui/images/capture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/ui/images/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.393653 neon-skill-camera-1.0.2a1/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)   341166 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/ui/sounds/clicking.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.389654 neon-skill-camera-1.0.2a1/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:10.393653 neon-skill-camera-1.0.2a1/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/vocab/en-us/ShowLastIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/vocab/en-us/TakePicIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/vocab/en-us/TakeVidIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-10 19:20:06.000000 neon-skill-camera-1.0.2a1/vocab/en-us/duration.entity
```

### Comparing `neon-skill-camera-1.0.1a1/LICENSE.md` & `neon-skill-camera-1.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/PKG-INFO` & `neon-skill-camera-1.0.2a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-camera
-Version: 1.0.1a1
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-camera
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-camera-1.0.1a1/README.md` & `neon-skill-camera-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/__init__.py` & `neon-skill-camera-1.0.2a1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 import time
 from os.path import dirname, abspath
 import subprocess
 
 from neon_utils.file_utils import get_most_recent_file_in_dir
 from neon_utils.message_utils import request_from_mobile
 
-from mycroft.skills.core import intent_file_handler
-from mycroft.util.parse import extract_number
-from mycroft.util import play_wav
+from ovos_workshop.decorators import intent_handler
+from lingua_franca.parse import extract_number
+from ovos_utils.sound import play_audio
 from subprocess import DEVNULL, STDOUT
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_utils.gui import is_gui_installed
 from neon_utils.skills.neon_skill import NeonSkill
 from neon_utils.message_utils import get_message_user
@@ -129,15 +129,15 @@
         self.gui["save_path"] = self.pic_path
         if activity == "singleshot":
             self.gui["singleshot_mode"] = True
         if activity == "generic":
             self.gui["singleshot_mode"] = False
         self.gui.show_page("Camera.qml", override_idle=60)
 
-    @intent_file_handler('TakePicIntent.intent')
+    @intent_handler('TakePicIntent.intent')
     def handle_take_pic_intent(self, message):
         if ("picture" or "pic" or "photo") in message.data.get("utterance"):
             LOG.info("In picture")
             LOG.debug(message.data)
             today = datetime.datetime.today()
             user = get_message_user(message) or os.environ.get('USER', os.environ.get('USERNAME'))
             pic_path = os.path.join(self.pic_path, user)
@@ -160,30 +160,30 @@
                     self.speak_dialog("ServerNotSupported", private=True)
                 elif self.gui_enabled:
                     self.gui["singleshot_mode"] = False
                     self.handle_camera_activity("singleshot")
                     self.bus.emit(message.forward("neon.metric", {"name": "audio-response"}))
                 else:
                     if self.cam_dev is not None:
-                        play_wav(self.shutter_sound)
+                        play_audio(self.shutter_sound)
                         self.bus.emit(message.forward("neon.metric", {"name": "audio-response"}))
                         # LOG.debug(f"TIME: to_speak, {time.time()}, {message.data['utterance']}, {message.context}")
                         os.system(f"fswebcam -d {self.cam_dev} --delay 2 --skip 2 "
                                   f"-r 1280x720 --no-banner {newest_pic}")
                         time.sleep(1)
                         self.display_image(image=newest_pic)
                     else:
                         self.speak_dialog("NoCamera", private=True)
             except Exception as e:
                 LOG.error(e)
             # finally:
             #     if ("user" or "my") in message.data.get("utterance"):
             #         self.save_user_info(newest_pic, "picture")
 
-    @intent_file_handler('ShowLastIntent.intent')
+    @intent_handler('ShowLastIntent.intent')
     def handle_show_last_intent(self, message):
         if "picture" in message.data.get("utterance"):
             if request_from_mobile(message):
                 pass
                 # TODO
                 # self.speak("MOBILE-INTENT LATEST_PICTURE")
                 # self.mobile_skill_intent("show_pic", {}, message)
@@ -236,25 +236,25 @@
         except Exception as e:
             LOG.error(e)
             self.speak_dialog("NothingToShow", {"kind": "videos"}, private=True)
 
     def display_image(self, image, secs=15, notify=True):
         # notification sound
         if notify:
-            play_wav(self.notify_sound)
+            play_audio(self.notify_sound)
 
         # method of displaying image
         # if self.configuration_available["devVars"]["devType"] in ("pi", "neonPi"):
         #     os.system("sudo /home/pi/ngi_code/scripts/splash/splash_start " + image + " " + str(secs))
         if is_gui_installed():
             self.gui.show_image(image, fill="PreserveAspectFit")
         else:
             os.system("timeout " + str(secs) + " eog " + image)
 
-    @intent_file_handler('TakeVidIntent.intent')
+    @intent_handler('TakeVidIntent.intent')
     def handle_take_vid_intent(self, message):
         if "video" in message.data.get("utterance"):
             try:
                 duration = message.data["duration"]
                 heard_duration = True
             except KeyError:
                 duration = "5 seconds"
@@ -293,25 +293,25 @@
                     self.speak_dialog("ServerNotSupported", private=True)
                 elif self.cam_dev:
                     if heard_duration:
                         self.speak_dialog("StartRecording", {"duration": duration}, private=True)
                     else:
                         self.speak_dialog("DefaultDuration", {"duration": duration}, private=True)
                     self.vidid += 1
-                    play_wav(self.record_sound)
+                    play_audio(self.record_sound)
                     vid_path = os.path.join(self.vid_path, get_message_user(message))
                     if not os.path.exists(vid_path):
                         LOG.debug(f"Creating video path: {vid_path}")
                         os.makedirs(vid_path)
 
                     path = vid_path + "v" + str(self.vidid) + ".avi" if not\
                         ("user" or "my") in message.data.get("utterance") else \
                         vid_path + "user_video_v" + str(self.vidid) + ".avi"
                     os.system(f"streamer -f rgb24 -i {self.cam_dev} -t 00:00:{secs} -o {path}.avi")
-                    play_wav(self.notify_sound)
+                    play_audio(self.notify_sound)
                     # if ("user" or "my") in message.data.get("utterance"):
                     #     self.save_user_info(path, 'video')
 
                     if playback:
                         time.sleep(1)
                         subprocess.Popen(["mpv", path], stdout=DEVNULL, stderr=STDOUT)
                 else:
```

### Comparing `neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/PKG-INFO` & `neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-camera
-Version: 1.0.1a1
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-camera
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/SOURCES.txt` & `neon-skill-camera-1.0.2a1/neon_skill_camera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/setup.py` & `neon-skill-camera-1.0.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/skill.json` & `neon-skill-camera-1.0.2a1/skill.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060607%*

 * *Differences: {"'requirements'": "{'python': {insert: [(1, 'ovos-lingua-franca~=0.4'), (3, "*

 * *                   "'ovos-workshop~=0.0.15')]}}"}*

```diff
@@ -23,15 +23,17 @@
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "neon-utils~=1.0",
-            "ovos-utils~=0.0, >=0.0.28"
+            "ovos-lingua-franca~=0.4",
+            "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Take pictures and videos.",
     "skillname": "skill-camera",
     "summary": "Take pictures and videos.",
```

### Comparing `neon-skill-camera-1.0.1a1/ui/Camera.qml` & `neon-skill-camera-1.0.2a1/ui/Camera.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/ui/ControlBar.qml` & `neon-skill-camera-1.0.2a1/ui/ControlBar.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/ui/images/back.svg` & `neon-skill-camera-1.0.2a1/ui/images/back.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/ui/images/capture.svg` & `neon-skill-camera-1.0.2a1/ui/images/capture.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/ui/images/close.svg` & `neon-skill-camera-1.0.2a1/ui/images/close.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/ui/sounds/clicking.wav` & `neon-skill-camera-1.0.2a1/ui/sounds/clicking.wav`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1a1/version.py` & `neon-skill-camera-1.0.2a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a1"
+__version__ = "1.0.2a1"
```

### Comparing `neon-skill-camera-1.0.1a1/vocab/en-us/ShowLastIntent.intent` & `neon-skill-camera-1.0.2a1/vocab/en-us/ShowLastIntent.intent`

 * *Files identical despite different names*

