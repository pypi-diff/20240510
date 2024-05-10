# Comparing `tmp/kbp2video-0.1.2.tar.gz` & `tmp/kbp2video-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbp2video-0.1.2.tar", last modified: Fri May  3 18:37:35 2024, max compression
+gzip compressed data, was "kbp2video-0.1.3.tar", last modified: Fri May 10 15:52:40 2024, max compression
```

## Comparing `kbp2video-0.1.2.tar` & `kbp2video-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:37:35.103513 kbp2video-0.1.2/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.2/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-03 18:37:35.103513 kbp2video-0.1.2/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.2/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:37:35.100180 kbp2video-0.1.2/kbp2video/
--rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-03 18:36:57.000000 kbp2video-0.1.2/kbp2video/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/_ffmpegcolor.py
--rw-r--r--   0 matt      (1000) matt      (1000)    75758 2024-05-03 18:36:57.000000 kbp2video-0.1.2/kbp2video/_gui.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/advanced_editor.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/utils.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:37:35.100180 kbp2video-0.1.2/kbp2video.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       53 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-03 18:36:57.000000 kbp2video-0.1.2/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-03 18:37:35.103513 kbp2video-0.1.2/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:52:40.877575 kbp2video-0.1.3/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.3/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-10 15:52:40.877575 kbp2video-0.1.3/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.3/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:52:40.874241 kbp2video-0.1.3/kbp2video/
+-rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-10 15:52:28.000000 kbp2video-0.1.3/kbp2video/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.3/kbp2video/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.3/kbp2video/_ffmpegcolor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    76003 2024-05-10 15:52:28.000000 kbp2video-0.1.3/kbp2video/_gui.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.3/kbp2video/advanced_editor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.3/kbp2video/utils.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:52:40.877575 kbp2video-0.1.3/kbp2video.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-10 15:52:40.000000 kbp2video-0.1.3/kbp2video.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-10 15:52:40.000000 kbp2video-0.1.3/kbp2video.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-10 15:52:40.000000 kbp2video-0.1.3/kbp2video.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-10 15:52:40.000000 kbp2video-0.1.3/kbp2video.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       53 2024-05-10 15:52:40.000000 kbp2video-0.1.3/kbp2video.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-10 15:52:40.000000 kbp2video-0.1.3/kbp2video.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-03 18:36:57.000000 kbp2video-0.1.3/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-10 15:52:40.877575 kbp2video-0.1.3/setup.cfg
```

### Comparing `kbp2video-0.1.2/LICENSE` & `kbp2video-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.2/kbp2video/_ffmpegcolor.py` & `kbp2video-0.1.3/kbp2video/_ffmpegcolor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.2/kbp2video/_gui.py` & `kbp2video-0.1.3/kbp2video/_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import ffmpeg
 from ._ffmpegcolor import ffmpeg_color
 import enum
 import kbputils
 import io
 import shutil
 from . import __version__
+import traceback
 
 class TrackTableColumn(enum.Enum):
     KBP_ASS = 0
     Audio = 1
     Background = 2
     Advanced = 3
 
@@ -1220,15 +1221,15 @@
                     data = kbp_obj.ass_data(**kbputils_options)
                 except:
                     QMetaObject.invokeMethod(
                         self,
                         'info', 
                         Qt.AutoConnection,
                         Q_ARG(str, "Failed to process kbp"),
-                        Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{' '.join(sys.exc_info())}"))
+                        Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{traceback.format_exc()}"))
                     continue
             elif kbp.endswith(".ass"): # kbp_obj is either a KBPASSWrapper with a .ass file, or a manually entered string with .ass
                 if any(x in kbp for x in ":;,'=\""):
                     print("Already .ass file, but needs new filename for ffmpeg")
                     QFile(kbp).copy(assfile)
                 else:
                     print("Using existing .ass file")
@@ -1519,14 +1520,20 @@
             "MainWindow", "&Convert to Video", None))
         self.convertAssButton.setText(QCoreApplication.translate(
             "MainWindow", "Subtitle onl&y", None))
     # retranslateUi
 
 
 def run(argv=sys.argv, ffmpeg_path=None):
+    if '--help' in argv or '-h' in argv:
+        print("kbp2video [[--help | -h] | [--version | -V]] [Qt6 options]")
+        sys.exit(0)
+    elif '--version' in argv or '-V' in argv:
+        print(__version__)
+        sys.exit(0)
     # Look better on Windows
     QApplication.setStyle("Fusion")
     app = QApplication(argv)
     orig_path = os.environ['PATH']
     if ffmpeg_path:
         os.environ['PATH'] = os.pathsep.join([ffmpeg_path, os.environ['PATH']])
     if not shutil.which("ffmpeg"):
```

### Comparing `kbp2video-0.1.2/kbp2video/advanced_editor.py` & `kbp2video-0.1.3/kbp2video/advanced_editor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.2/kbp2video/utils.py` & `kbp2video-0.1.3/kbp2video/utils.py`

 * *Files identical despite different names*

