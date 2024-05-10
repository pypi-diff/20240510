# Comparing `tmp/ipyslides-3.8.2.tar.gz` & `tmp/ipyslides-3.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.8.2.tar", last modified: Wed May  8 19:16:04 2024, max compression
+gzip compressed data, was "ipyslides-3.8.4.tar", last modified: Fri May 10 10:29:36 2024, max compression
```

## Comparing `ipyslides-3.8.2.tar` & `ipyslides-3.8.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 19:16:04.375400 ipyslides-3.8.2/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.2/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-08 19:16:04.375400 ipyslides-3.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 19:16:04.241017 ipyslides-3.8.2/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.2/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-08 19:15:05.000000 ipyslides-3.8.2/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:16:04.359138 ipyslides-3.8.2/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.2/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    39824 2024-05-08 19:13:02.000000 ipyslides-3.8.2/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     5950 2024-05-08 17:44:13.000000 ipyslides-3.8.2/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.2/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.8.2/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.8.2/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-03 23:26:00.000000 ipyslides-3.8.2/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.8.2/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:16:04.372324 ipyslides-3.8.2/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.8.2/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.2/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.2/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.2/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.2/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    22017 2024-05-08 19:00:25.000000 ipyslides-3.8.2/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28852 2024-05-08 00:37:24.000000 ipyslides-3.8.2/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28513 2024-05-08 18:39:39.000000 ipyslides-3.8.2/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15593 2024-05-08 00:49:46.000000 ipyslides-3.8.2/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.2/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    48786 2024-05-08 18:32:24.000000 ipyslides-3.8.2/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.2/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.2/ipyslides/source.py
--rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.8.2/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.2/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.2/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:16:04.308645 ipyslides-3.8.2/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-08 19:16:03.000000 ipyslides-3.8.2/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-08 19:16:03.000000 ipyslides-3.8.2/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 19:16:03.000000 ipyslides-3.8.2/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-08 19:16:03.000000 ipyslides-3.8.2/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 19:16:03.000000 ipyslides-3.8.2/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 19:16:04.375400 ipyslides-3.8.2/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:29:36.331344 ipyslides-3.8.4/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.4/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-10 10:29:36.329716 ipyslides-3.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:29:36.242355 ipyslides-3.8.4/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.4/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-10 10:28:41.000000 ipyslides-3.8.4/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:29:36.324666 ipyslides-3.8.4/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.4/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    39305 2024-05-10 10:28:28.000000 ipyslides-3.8.4/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     5950 2024-05-10 08:28:06.000000 ipyslides-3.8.4/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.4/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.8.4/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.4/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.4/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    12158 2024-05-10 07:35:58.000000 ipyslides-3.8.4/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:29:36.327673 ipyslides-3.8.4/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12840 2024-05-10 10:09:39.000000 ipyslides-3.8.4/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.4/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.4/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.4/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.4/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    21451 2024-05-10 05:55:37.000000 ipyslides-3.8.4/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28852 2024-05-08 00:37:24.000000 ipyslides-3.8.4/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28513 2024-05-08 18:39:39.000000 ipyslides-3.8.4/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    15376 2024-05-10 05:56:13.000000 ipyslides-3.8.4/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.4/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47812 2024-05-10 09:58:54.000000 ipyslides-3.8.4/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.4/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.4/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.8.4/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.4/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.4/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:29:36.294764 ipyslides-3.8.4/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-10 10:29:35.000000 ipyslides-3.8.4/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-10 10:29:35.000000 ipyslides-3.8.4/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:29:35.000000 ipyslides-3.8.4/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-10 10:29:35.000000 ipyslides-3.8.4/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 10:29:35.000000 ipyslides-3.8.4/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:29:36.331344 ipyslides-3.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.4/setup.py
```

### Comparing `ipyslides-3.8.2/LICENSE` & `ipyslides-3.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/PKG-INFO` & `ipyslides-3.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.2
+Version: 3.8.4
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.2/README.md` & `ipyslides-3.8.4/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/_layout_css.py` & `ipyslides-3.8.4/ipyslides/_base/_layout_css.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
                     "animation-delay": "60s",  # Beet at 60 seconds if left on slide
                 },
                 ".Slide-Number" : { # slide number
                     "position": "absolute !important",
                     "right": "0 !important",
                     "bottom": "0 !important",
                     "backdrop-filter": "blur(8px)",
+                    "padding": "0 6px !important",
                 },
                 ".Progress-Box": {
                     "margin": "0 !important",
                     "padding": "0 !important",
                     "position": "absolute !important",
                     "left":"0 !important",
                     "bottom": "0 !important",
@@ -343,42 +344,42 @@
                         },
                     },
                     ".Toc-Btn, .Menu-Btn, .Screenshot-Btn": {
                         "min-width": "28px",
                         "width": "28px", # need this too
                     },  # Avoid overflow in small screens
                     ".Footer": {
+                        "overflow": "hidden !important",
                         ".widget-html-content": {
                             "display": "flex",
                             "align-items": "center",
                             "justify-content": "flex-start",
                         },
                         "p": {
                             "font-size": "14px !important",
                         },
                     },
                 },
             },
             ".Controls": {
                 "position": "absolute",
-                "right": "16px !important",
-                "bottom": "0px !important",
+                "right": "8px !important",
+                "bottom": "12px !important",
                 "z-index": "4",  # below matplotlib fullsreen
                 "padding": "0 !important",
                 "justify-content": " flex-end !important",
                 "align-items": "center !important",
-                "margin-bottom": "16px !important",
                 "color": " var(--accent-color) !important",
                 ".widget-button > i": {
                     "color": "var(--accent-color) !important",
                 },
                 ".Arrows": {
                     "opacity": "0.4",
                     "font-size": "36px",
-                    "padding": "4px",
+                    "padding": "2px",
                     "^:hover, ^:focus": {"opacity": 1},
                 },
                 ".ProgBox": {
                     "width": "16px",
                     "padding": "0px 8px",
                     "opacity": 0,
                     "overflow": "hidden",
@@ -396,28 +397,28 @@
                 "position":"absolute",
                 "left": "0",
                 "bottom": "24px", # just above navbar
                 "display": "table-column-group !important", # This to avoid collapsing divs
                 "background": "var(--secondary-bg)",
                 "backdrop-filter": " blur(50px)",
                 "margin": "4px",
-                "min-width": "30% !important",
+                "min-width": "50% !important",
                 "box-sizing": "border-box !important",
                 "z-index": "8",
                 "border-radius": "4px",
                 "transition": "height 400ms ease-in-out",
-                "@container slides (max-width: 650px)": {"min-width": "60% !important"},
+                "@container slides (max-width: 650px)": {"min-width": "80% !important"},
                 ".custom-html": {
                     "display": "flex",
                     "flex-direction": "row",
                     "flex-wrap": "nowrap",
                     "justify-content": "space-between !important",
                     "height": "auto",
                     "width": "auto",
-                    "font-size": "14px !important",
+                    "font-size": "16px !important", # A liitle larger
                     "box-sizing": "border-box !important",
                 },
             },
             ".CaptureHtml *": {
                 "font-size": "0.9em",
                 "line-height": "0.9em  !important",
             },
@@ -546,24 +547,24 @@
                 'rect.tl-frame__body': { # Due to lack of dark mode in widget
                     'fill':'var(--primary-bg)',
                     'stroke':'var(--secondary-bg)',
                 },
             },
             ".Arrows": {
                 ".fa.fa-chevron-left": Icon(
-                    "chevron", color=accent_color, size="36px", rotation=180
+                    "chevron", color=accent_color, size="32px", rotation=180
                 ).css,
                 ".fa.fa-chevron-right": Icon(
-                    "chevron", color=accent_color, size="36px", rotation=0
+                    "chevron", color=accent_color, size="32px", rotation=0
                 ).css,
                 ".fa.fa-chevron-up": Icon(
-                    "chevron", color=accent_color, size="36px", rotation=-90
+                    "chevron", color=accent_color, size="32px", rotation=-90
                 ).css,  # Why SVG rotation is clockwise?
                 ".fa.fa-chevron-down": Icon(
-                    "chevron", color=accent_color, size="36px", rotation=90
+                    "chevron", color=accent_color, size="32px", rotation=90
                 ).css,
             },
             ".Settings-Btn": {
                 ".fa.fa-plus": Icon("settings", color=accent_color, size=_icons_size).css,
                 ".fa.fa-minus": Icon("close", color=accent_color, size=_icons_size).css,
             },
             ".Toc-Btn": {
@@ -726,35 +727,22 @@
                 "padding-bottom": "8px !important",
                 "padding-right": "8px !important",
             },  # Jupyter-Lab make space in input cell
             "<.cell-output-ipywidget-background": {  # VSCode issue */
                 "background": "var(--theme-background,inherit) !important",
                 "margin": "8px 0px",
             },
-            ".InView-Btn": {
-                "display": "none !important",
-            },
             "<.jp-LinkedOutputView > .jp-OutputArea > .jp-OutputArea-child": {
                 "height": "100% !important", # This needs to in same selector order to not effect slide content
-                ".SlidesWrapper, .DisplayBox": {
+                ".SlidesWrapper": {
                     "min-width": "100% !important",
                     "width": "100% !important",
                     "min-height": "100% !important",
                     "height": "100% !important",
                     "box-sizing": "border-box !important",
-                    ".InView-Btn": {
-                        "display": "block !important",
-                        "position": "absolute",
-                        "top": "0",
-                        "left": "0",
-                        "z-index": "10",
-                        "color": "white !important",
-                        "background": "green !important",
-                        "font-size": "14px !important",  # Avoid this button font scaling
-                    },
                     ".Width-Slider": {
                         "display": "none !important",
                     },
                 },
             },
             "<#ipython-main-app .SlidesWrapper .output_scroll": {  # For classic Notebook output
                 "height": "unset !important",
```

### Comparing `ipyslides-3.8.2/ipyslides/_base/_widgets.py` & `ipyslides-3.8.4/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/base.py` & `ipyslides-3.8.4/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/export_html.py` & `ipyslides-3.8.4/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/export_template.py` & `ipyslides-3.8.4/ipyslides/_base/export_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
 section .SlideBox > .Footer { 
     background: var(--primary-bg); /* no important here */
     padding: 0 !important; margin: 0 !important; 
     position:absolute;
     left:0;
     width: 100%;
     bottom: 0;
+    overflow: hidden !important;
 }
 section .SlideBox > .Footer.NavHidden {
     background: none; /* no important here */
 }
 section .SlideBox > .Footer > p {
     font-size: 14px !important;
     padding: 4px !important;
```

### Comparing `ipyslides-3.8.2/ipyslides/_base/icons.py` & `ipyslides-3.8.4/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/intro.py` & `ipyslides-3.8.4/ipyslides/_base/intro.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 | {_key('E')}                                 | {_icons["code"]}                                  | {key_maps["E"]}        |
 | {_key('L')}                                 | {_icons["laser"]}, {_icons["circle"]}             | {key_maps["L"]}        |
 | {_key('K')}                                 |                                                   | {key_maps["K"]}        |
 """ 
 
 more_instructions = f"""{get_logo('2em', 'IPySlides')}
 ::: note-tip
-    In JupyterLab, right click on the slides and select `Create New View for Output` and follow next there to optimize display.
+    In JupyterLab, right click on the slides and select `Create New View for Output` for optimized display.
 
 **Key Bindings**{{.success}} {_Icon("pencil", color="var(--accent-color)", rotation=45)}
 
 Having slides in focus, you can use follwoing keys/combinations:
 
 {key_combs}
 ::: note
```

### Comparing `ipyslides-3.8.2/ipyslides/_base/js/interaction.js` & `ipyslides-3.8.4/ipyslides/_base/js/interaction.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -156,17 +156,32 @@
                     sync: true
                 })
             }, interval)
         } else if (sync === "OFF") {
             clearInterval(model.syncIntervalID);
         }
 
+    } else if (msg === "CloseView") { // deletes node without closing comm to kernl
+        if (box) { // may be nothing there left already
+            box.remove();
+        }
     }
 };
 
+function keepThisViewOnly(box) {
+    let klass = box.className.match(/Slides\-\d+/)[0];
+    let slides = document.getElementsByClassName(klass); // only this uid slides, not in other notebooks
+
+    for (let slide of Array.from(slides)) {
+        if (slide !== box) { // onlt keep this view
+            slide.remove(); // deletes node, but keeps comm live
+        }
+    }
+}
+
 function handleChangeFS(box, model) {
     if (box === document.fullscreenElement) {
         model.set("msg_topy", "FS")
     } else {
         model.set("msg_topy", "!FS")
     };
     model.save_changes();
@@ -261,14 +276,17 @@
 
         // Touch Events are experimental
         touchSwiper(box, model);
 
         // handle scale of slides size
         handleScale(box);
 
+        // Remove other views without closing comm
+        keepThisViewOnly(box);
+
         // Sends a message if fullscreen is changed by some other mechanism
         box.onfullscreenchange = () => {
             handleChangeFS(box, model)
         };
 
         // If voila, turn on full viewport
         let loc = window.location.toString()
```

### Comparing `ipyslides-3.8.2/ipyslides/_base/js/notes.js` & `ipyslides-3.8.4/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/navigation.py` & `ipyslides-3.8.4/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/notes.py` & `ipyslides-3.8.4/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/screenshot.py` & `ipyslides-3.8.4/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/settings.py` & `ipyslides-3.8.4/ipyslides/_base/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         self.btn_laser = self.widgets.toggles.laser
         self.btn_draw = self.widgets.toggles.draw
         self.btn_menu = self.widgets.toggles.menu
         self.box = self.widgets.panelbox
 
         self.widgets.buttons.toc.on_click(self._toggle_tocbox)
         self.widgets.buttons.info.on_click(self._show_info)
-        self.widgets.buttons._inview.on_click(self.__keep_new_output_only)
         self.widgets.htmls.toast.observe(self._toast_on_value_change, names=["value"])
         self.theme_dd.observe(self._update_theme, names=["value"])
         self.fontsize_slider.observe(self._update_theme, names=["value"])
         self.width_slider.observe(self._update_size, names=["value"])
         self.btn_window.observe(self._toggle_viewport, names=["value"])
         self.btn_fscreen.observe(self._toggle_fullscreen, names=["value"])
         self.btn_fscreen.observe(self._on_icon_change, names=["icon"])
@@ -64,23 +63,14 @@
         self.widgets.checks.navgui.observe(self._toggle_nav_gui, names=["value"])
         self.widgets.checks.proxy.observe(self._toggle_proxy_buttons, names=["value"])
         self._update_theme()  # Trigger Theme and Javascript in it
         self.set_code_theme()  # Trigger CSS in it, must
         self.set_layout(center=True)  # Trigger this as well
         self._update_size(change=None)  # Trigger this as well
 
-    def __keep_new_output_only(self, btn):
-        self.widgets.navbox.children = [
-            w for w in self.widgets.navbox.children if w is not btn
-        ]
-        dh = getattr(self._slides._display_box, "_DH", None)  # Get display handler
-        self._slides._display_box = self._slides.alert("Slides → Linked Output View").as_widget()  # Swap display box by info, still widget to be closable
-        if dh is not None:
-            dh.update(self._slides._display_box) 
-
     def _close_quick_menu(self):
         "Need for actions on all buttons inside menu."
         if self.btn_menu.value:
             self.btn_menu.value = False
     
     def _toast_on_value_change(self, change):
         if change.new:
@@ -396,15 +386,15 @@
             msg = "THEME:jupyterlab"
         else:
             msg = 'THEME:dark' if "Dark" in self.theme_dd.value else 'THEME:light'
         self.widgets.iw.msg_tojs = msg # changes theme of board
 
     def _toggle_tocbox(self, btn):
         if self.widgets.tocbox.layout.height == "0":
-            self.widgets.tocbox.layout.height = f"min(calc(100% - 32px), {max(128, len(self.widgets.tocbox.children)*32)}px)"
+            self.widgets.tocbox.layout.height = f"min(calc(100% - 32px), {max(150, len(self.widgets.tocbox.children)*36)}px)"
             self.widgets.tocbox.layout.border = "1px solid var(--hover-bg)"
             self.widgets.tocbox.layout.padding = "4px"
             self.widgets.buttons.toc.icon = "minus"
         else:
             self.widgets.tocbox.layout.height = "0"
             self.widgets.tocbox.layout.border = "none"
             self.widgets.tocbox.layout.padding = "0"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ipyslides-3.8.2/ipyslides/_base/slide.py` & `ipyslides-3.8.4/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/styles.py` & `ipyslides-3.8.4/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/_base/widgets.py` & `ipyslides-3.8.4/ipyslides/_base/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     capture =  Button(icon='camera',layout= Layout(width='auto',height='auto'),
                 tooltip='Take Screen short in full screen. Order of multiple shots in a slide is preserved! [S]',
                 ).add_class('Screenshot-Btn').add_class('Menu-Item')
     pdf     = Button(description='Save PDF',layout= Layout(width='auto',height='auto'))
     png     = Button(description='Save PNG',layout= Layout(width='auto',height='auto'))
     cap_all = Button(description='Capture All',layout= Layout(width='auto',height='auto'))
     export  = Button(description="Export to HTML",layout= Layout(width='auto',height='auto'))
-    _inview = Button(description='Click to Optimize Experience in JupyterLab',layout= Layout(width='auto',height='auto')).add_class('InView-Btn') # For testing if inside LinkedView
     
 @dataclass(frozen=True)
 class _Toggles:
     """
     Instantiate under `Widgets` class only.
     """
     window  = ipw.ToggleButton(icon='plus',value = False, tooltip ='Fill Viewport [V]').add_class('FullWindow-Btn').add_class('Menu-Item')
@@ -119,15 +118,15 @@
 
 @dataclass(frozen=True)
 class _Sliders:
     """
     Instantiate under `Widgets` class only.
     """
     progress = ipw.SelectionSlider(options=[('0',0)], value=0, continuous_update=False,readout=True)
-    width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 55,continuous_update=False).add_class('Width-Slider') 
+    width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 60,continuous_update=False).add_class('Width-Slider') 
     fontsize = ipw.IntSlider(**describe('Font Size'),min=8,max=64,step=1, value = 20,continuous_update=False, tooltip="If you need more larger/smaller font size, use `Slides.settings.set_font_size`")
 
 @dataclass(frozen=True)
 class _Dropdowns:
     """
     Instantiate under `Widgets` class only.
     """
@@ -182,15 +181,14 @@
                 self.buttons.toc, 
                 self.buttons.source,  
             ]).add_class('Menu-Box'),
             HBox([self.htmls.footer]), # should be in Box to avoid overflow
         ],layout=Layout(height='28px')).add_class('NavBox')
         
         self.navbox = VBox([
-            self.buttons._inview,
             self.footerbox,
         ]).add_class('NavWrapper')   #class is must
 
         _many_btns = [self.buttons.setting, self.toggles.window, self.toggles.fscreen, self.toggles.laser, self.toggles.zoom, self.buttons.refresh, self.toggles.draw]
         
         self.panelbox = VBox([
             self.htmls.glass,
```

### Comparing `ipyslides-3.8.2/ipyslides/_demo.py` & `ipyslides-3.8.4/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/core.py` & `ipyslides-3.8.4/ipyslides/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,14 @@
         self.progress_slider.observe(self._update_content, names=["index"])
         self.widgets.buttons.refresh.on_click(self._update_dynamic_content)
         self.widgets.buttons.source.on_click(self._jump_to_source_cell)
 
         # All Box of Slides
         self._box = self.widgets.mainbox.add_class(self.uid)
         self._setup()  # Load some initial data and fixing
-        self._display_box = None  # Initialize
         
     @contextmanager
     def _set_running(self, slide):
         "Context manager to set running slide and turns back to previous."
         if slide and not isinstance(
             slide, Slide
         ):  # None is acceptable to hold running slide in other function
@@ -526,38 +525,20 @@
         if not self.is_jupyter_session():
             raise Exception("Python/IPython REPL cannot show slides. Use IPython notebook instead.")
 
         clear_output(wait = True) # Avoids jump buttons and other things in same cell created by scripts producing slides
         self._unregister_postrun_cell() # no need to scroll button where showing itself
         self._update_toc()  # Update toc before displaying app to include all sections
         self._update_dynamic_content()  # Update dynamic content before displaying app
-        self.close_view()  # Close previous views
-        self.__reset_navbox()  # Important to add inview button for each new view
-        self._display_box = ipw.VBox(children=[self._box]).add_class(
-            "DisplayBox"
-        )  # Initialize display box again
-        h = display(self._display_box, display_id=True)  # Display slides
-        self._display_box._DH = (
-            h  # This is important for Jupyter Lab to optimize experience
-        )
+        display(self.widgets.mainbox)  # Display slides
+        
 
     def close_view(self):
         "Close slides/cell view, but keep slides in memory than can be shown again."
-        if hasattr(self, "_display_box") and self._display_box is not None:
-            self._display_box.close()  # Clear display that removes CSS things there
-            self.__reset_navbox()  # Important to add inview button for next view
-
-    def __reset_navbox(self):
-        "Reset navbox to add inview button for Jupyter Lab"
-        others = [
-            w
-            for w in self.widgets.navbox.children
-            if w is not self.widgets.buttons._inview
-        ]
-        self.widgets.navbox.children = [self.widgets.buttons._inview, *others]
+        self.widgets.iw.msg_tojs = "CloseView"
 
     @property
     def _slideindex(self):
         "Get current slide index"
         return self.progress_slider.index
 
     @_slideindex.setter
```

### Comparing `ipyslides-3.8.2/ipyslides/formatters.py` & `ipyslides-3.8.4/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/source.py` & `ipyslides-3.8.4/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/utils.py` & `ipyslides-3.8.4/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/writer.py` & `ipyslides-3.8.4/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides/xmd.py` & `ipyslides-3.8.4/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.8.4/ipyslides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.2
+Version: 3.8.4
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.2/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.8.4/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.2/setup.py` & `ipyslides-3.8.4/setup.py`

 * *Files identical despite different names*

