# Comparing `tmp/kbputils-0.0.5.tar.gz` & `tmp/kbputils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbputils-0.0.5.tar", last modified: Fri May  3 18:35:39 2024, max compression
+gzip compressed data, was "kbputils-0.0.6.tar", last modified: Fri May 10 15:51:21 2024, max compression
```

## Comparing `kbputils-0.0.5.tar` & `kbputils-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:35:39.086653 kbputils-0.0.5/
--rw-r--r--   0 matt      (1000) matt      (1000)     1305 2024-04-16 18:40:43.000000 kbputils-0.0.5/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)     2199 2024-05-03 18:35:39.086653 kbputils-0.0.5/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     1844 2024-04-16 19:00:17.000000 kbputils-0.0.5/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:35:39.083320 kbputils-0.0.5/kbputils/
--rw-r--r--   0 matt      (1000) matt      (1000)      154 2024-05-03 18:34:35.000000 kbputils-0.0.5/kbputils/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2563 2024-05-03 18:34:35.000000 kbputils-0.0.5/kbputils/cli.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14187 2024-05-03 18:34:35.000000 kbputils-0.0.5/kbputils/converters.py
--rw-r--r--   0 matt      (1000) matt      (1000)    18086 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/kbp.py
--rw-r--r--   0 matt      (1000) matt      (1000)      773 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/kbs.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6745 2024-04-16 18:40:43.000000 kbputils-0.0.5/kbputils/validators.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:35:39.086653 kbputils-0.0.5/kbputils.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     2199 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      362 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       55 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        4 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        9 2024-05-03 18:35:39.000000 kbputils-0.0.5/kbputils.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      627 2024-05-03 18:34:35.000000 kbputils-0.0.5/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-03 18:35:39.086653 kbputils-0.0.5/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:51:21.464118 kbputils-0.0.6/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1305 2024-04-16 18:40:43.000000 kbputils-0.0.6/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)     2718 2024-05-10 15:51:21.464118 kbputils-0.0.6/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     2363 2024-05-10 15:51:04.000000 kbputils-0.0.6/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:51:21.464118 kbputils-0.0.6/kbputils/
+-rw-r--r--   0 matt      (1000) matt      (1000)      154 2024-05-10 15:51:04.000000 kbputils-0.0.6/kbputils/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-16 18:40:43.000000 kbputils-0.0.6/kbputils/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2563 2024-05-03 18:34:35.000000 kbputils-0.0.6/kbputils/cli.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14246 2024-05-10 15:51:04.000000 kbputils-0.0.6/kbputils/converters.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    18656 2024-05-10 15:51:04.000000 kbputils-0.0.6/kbputils/kbp.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      773 2024-04-16 18:40:43.000000 kbputils-0.0.6/kbputils/kbs.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6745 2024-04-16 18:40:43.000000 kbputils-0.0.6/kbputils/validators.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:51:21.464118 kbputils-0.0.6/kbputils.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2718 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      362 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       55 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        4 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        9 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      627 2024-05-03 18:34:35.000000 kbputils-0.0.6/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-10 15:51:21.464118 kbputils-0.0.6/setup.cfg
```

### Comparing `kbputils-0.0.5/LICENSE` & `kbputils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.5/PKG-INFO` & `kbputils-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbputils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utilities to handle .kbp files created with Karaoke Builder Studio.
 Author-email: Matt M <code@itmightbekaraoke.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ass
@@ -16,43 +16,52 @@
 
 Current contents are:
 
 kbputils module to parse a file into a data structure:
 
     k = kbputils.KBPFile(filename)
 
-converters module which currently contains a basic converter to the .ass format:
+converters module which currently contains a converter to the .ass format:
 
-    converter = kbputils.converters.AssConverter(k) # A few options are available, but not many yet
+    converter = kbputils.converters.AssConverter(k) # Several options are available to tweak processing
     doc = converter.ass_document()  # generate an ass.Document from the ass module
     with open("outputfile.ass", "w", encoding='utf_8_sig') as f:
         doc.dump_file(f)
 
 There's also a CLI for it (command and syntax subject to change):
 
     $ KBPUtils --help
-    usage: KBPUtils [-h] [--border | --no-border] [--float-font | --no-float-font] [--float-pos | --no-float-pos] [--target-x TARGET_X]
-                    [--target-y TARGET_Y] [--fade-in FADE_IN] [--fade-out FADE_OUT] [--transparency | --no-transparency] [--offset OFFSET]
-                    source_file [dest_file]
-    
+    usage: KBPUtils [-h] [--version] [--border | --no-border | -b] [--float-font | --no-float-font | -f] [--float-pos | --no-float-pos | -p]
+                [--target-x TARGET_X] [--target-y TARGET_Y] [--fade-in FADE_IN] [--fade-out FADE_OUT] [--transparency | --no-transparency | -t]
+                [--offset OFFSET] [--overflow {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}]
+                source_file [dest_file]
+
     Convert .kbp to .ass file
-    
+
     positional arguments:
       source_file
       dest_file
-    
+
     options:
       -h, --help            show this help message and exit
-      --border, --no-border
+      --version, -V         show program's version number and exit
+      --border, --no-border, -b
                             bool (default: True)
-      --float-font, --no-float-font
+      --float-font, --no-float-font, -f
                             bool (default: True)
-      --float-pos, --no-float-pos
+      --float-pos, --no-float-pos, -p
                             bool (default: False)
-      --target-x TARGET_X   int (default: 300)
-      --target-y TARGET_Y   int (default: 216)
-      --fade-in FADE_IN     int (default: 300)
-      --fade-out FADE_OUT   int (default: 200)
-      --transparency, --no-transparency
+      --target-x TARGET_X, -x TARGET_X
+                            int (default: 300)
+      --target-y TARGET_Y, -y TARGET_Y
+                            int (default: 216)
+      --fade-in FADE_IN, -i FADE_IN
+                            int (default: 300)
+      --fade-out FADE_OUT, -o FADE_OUT
+                            int (default: 200)
+      --transparency, --no-transparency, -t
                             bool (default: True)
-      --offset OFFSET       int | bool (default: True)
-    
+      --offset OFFSET, -s OFFSET
+                            int | bool (default: True)
+      --overflow {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}, -v {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}
+                            AssOverflow (default: EVEN_SPLIT)
+
```

### Comparing `kbputils-0.0.5/README.md` & `kbputils-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,43 +5,52 @@
 
 Current contents are:
 
 kbputils module to parse a file into a data structure:
 
     k = kbputils.KBPFile(filename)
 
-converters module which currently contains a basic converter to the .ass format:
+converters module which currently contains a converter to the .ass format:
 
-    converter = kbputils.converters.AssConverter(k) # A few options are available, but not many yet
+    converter = kbputils.converters.AssConverter(k) # Several options are available to tweak processing
     doc = converter.ass_document()  # generate an ass.Document from the ass module
     with open("outputfile.ass", "w", encoding='utf_8_sig') as f:
         doc.dump_file(f)
 
 There's also a CLI for it (command and syntax subject to change):
 
     $ KBPUtils --help
-    usage: KBPUtils [-h] [--border | --no-border] [--float-font | --no-float-font] [--float-pos | --no-float-pos] [--target-x TARGET_X]
-                    [--target-y TARGET_Y] [--fade-in FADE_IN] [--fade-out FADE_OUT] [--transparency | --no-transparency] [--offset OFFSET]
-                    source_file [dest_file]
-    
+    usage: KBPUtils [-h] [--version] [--border | --no-border | -b] [--float-font | --no-float-font | -f] [--float-pos | --no-float-pos | -p]
+                [--target-x TARGET_X] [--target-y TARGET_Y] [--fade-in FADE_IN] [--fade-out FADE_OUT] [--transparency | --no-transparency | -t]
+                [--offset OFFSET] [--overflow {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}]
+                source_file [dest_file]
+
     Convert .kbp to .ass file
-    
+
     positional arguments:
       source_file
       dest_file
-    
+
     options:
       -h, --help            show this help message and exit
-      --border, --no-border
+      --version, -V         show program's version number and exit
+      --border, --no-border, -b
                             bool (default: True)
-      --float-font, --no-float-font
+      --float-font, --no-float-font, -f
                             bool (default: True)
-      --float-pos, --no-float-pos
+      --float-pos, --no-float-pos, -p
                             bool (default: False)
-      --target-x TARGET_X   int (default: 300)
-      --target-y TARGET_Y   int (default: 216)
-      --fade-in FADE_IN     int (default: 300)
-      --fade-out FADE_OUT   int (default: 200)
-      --transparency, --no-transparency
+      --target-x TARGET_X, -x TARGET_X
+                            int (default: 300)
+      --target-y TARGET_Y, -y TARGET_Y
+                            int (default: 216)
+      --fade-in FADE_IN, -i FADE_IN
+                            int (default: 300)
+      --fade-out FADE_OUT, -o FADE_OUT
+                            int (default: 200)
+      --transparency, --no-transparency, -t
                             bool (default: True)
-      --offset OFFSET       int | bool (default: True)
-    
+      --offset OFFSET, -s OFFSET
+                            int | bool (default: True)
+      --overflow {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}, -v {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}
+                            AssOverflow (default: EVEN_SPLIT)
+
```

### Comparing `kbputils-0.0.5/kbputils/cli.py` & `kbputils-0.0.6/kbputils/cli.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.5/kbputils/converters.py` & `kbputils-0.0.6/kbputils/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,18 +270,19 @@
         self._calc_style_alignments()
         for page in self.kbpFile.pages:
             for num, line in enumerate(page.lines):
                 if line.isempty():
                     continue
                 pos = self.get_pos(line, num)
                 line_margins = self.get_line_margins(line, pos)
+                line_style = styles[line.style]
                 result.events.append(ass.Dialogue(
                     start=datetime.timedelta(milliseconds = line.start * 10 + self.options.offset),
                     end=datetime.timedelta(milliseconds = line.end * 10 + self.options.offset),
-                    style=AssConverter.ass_style_name(kbp.KBPStyleCollection.alpha2key(line.style), styles[line.style].name),
+                    style=AssConverter.ass_style_name(line_style.style_no, line_style.name), # Undefined styles get default style number
                     effect="karaoke",
                     text=self.kbp2asstext(line, pos),
                     margin_l=line_margins[0],
                     margin_r=line_margins[1],
                     ))
         for idx in styles:
             style = styles[idx]
```

### Comparing `kbputils-0.0.5/kbputils/kbp.py` & `kbputils-0.0.6/kbputils/kbp.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 
     def isempty(self):
         return not self.syllables or (len(self.syllables) == 1 and self.syllables[0].isempty())
 
 @validators.validated_instantiation
 class KBPStyle(typing.NamedTuple):
     name: str
+    style_no: int
     textcolor: str | int
     outlinecolor: str | int
     textwipecolor: str | int
     outlinewipecolor: str | int
     fontname: str
     fontsize: int
     fontstyle: str
@@ -251,14 +252,15 @@
     # non-wiped values for compatibility with other formats
     def make_fixed(style):
         if style.fixed:
             return style
         else:
             return style._replace(
                 name = style.name + "_fixed",
+                style_no = -style.style_no,
                 textwipecolor = style.textcolor,
                 outlinewipecolor = style.outlinecolor,
                 fixed = True)
 
 class KBPStyleCollection(dict):
     __slots__ = ()
 
@@ -272,18 +274,29 @@
             return string.ascii_uppercase.index(alpha)+1
         elif alpha in list(string.ascii_lowercase):
             return -string.ascii_lowercase.index(alpha)-1
 
     def __missing__(self, key):
         if key in list(string.ascii_letters):
             return self[KBPStyleCollection.alpha2key(key)]
+
         # Auto-vivify fixed styles
         elif isinstance(key, int) and -key in self.keys():
             self[key] = self[-key].make_fixed()
             return self[key]
+
+        # Undefined styles should return the default style
+        # The caller can determine this happened if needed by
+        # comparing style.style_no with the requested index
+        # A converter can choose on its side whether it wants
+        # the undefined style to be considered a new one or 
+        # reuse the name of the default
+        elif isinstance(key, int) and (1 <= abs(key) <= 26):
+            return self[1] if key > 0 else self[-1]
+
         else:
             raise KeyError(key)
 
     # Hopefully the checks in the next several methods will be enough to keep bad data out...
     @validators.validated_types
     @staticmethod
     def __assert_valid_item(key: int, value: KBPStyle):
@@ -334,15 +347,16 @@
         for n, line in enumerate(style_lines):
             line = line.lstrip()
             if line == "" and style_no is not None:
                 style_no = None
                 fields = {}
             elif style_no is None and line.startswith("Style"):
                 tmp = line.split(",")
-                style_no = int(tmp[0][5:])
+                style_no = int(tmp[0][5:]) + 1
+                fields['style_no'] = style_no
                 tmp = [tmp[1], *(int(x) for x in tmp[2:])]
                 fields.update(dict(zip(("name", "textcolor", "outlinecolor", "textwipecolor", "outlinewipecolor"),tmp)))
                 tmp = style_lines[n+1].lstrip().split(",")
                 tmp[1] = int(tmp[1])
                 tmp[3] = int(tmp[3])
                 fields.update(dict(zip(("fontname", "fontsize", "fontstyle", "charset"),tmp)))
                 tmp = style_lines[n+2].lstrip().split(",")
@@ -350,15 +364,15 @@
                 fields.update(dict(zip(("outlines", "shadows", "wipestyle", "allcaps", "fixed"),(tmp[:4],tmp[4:6],tmp[6],tmp[7],False))))
                 result = KBPStyle(**fields)
                 if palette:
                     result = result.resolve_colors(palette)
                 # Adding 1 to style for 2 reasons:
                 # - Style 0/A is shown in the KBS UI as 01
                 # - It allows indexing fixed styles as negative numbers
-                styles[style_no+1] = result
+                styles[style_no] = result
             # else second/third line of styles already processed
         return styles
     
     
     def key2alpha(key: int):
         if key < 0:
             return string.ascii_lowercase[-key-1]
```

### Comparing `kbputils-0.0.5/kbputils/kbs.py` & `kbputils-0.0.6/kbputils/kbs.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.5/kbputils/validators.py` & `kbputils-0.0.6/kbputils/validators.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.5/kbputils.egg-info/PKG-INFO` & `kbputils-0.0.6/kbputils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbputils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utilities to handle .kbp files created with Karaoke Builder Studio.
 Author-email: Matt M <code@itmightbekaraoke.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ass
@@ -16,43 +16,52 @@
 
 Current contents are:
 
 kbputils module to parse a file into a data structure:
 
     k = kbputils.KBPFile(filename)
 
-converters module which currently contains a basic converter to the .ass format:
+converters module which currently contains a converter to the .ass format:
 
-    converter = kbputils.converters.AssConverter(k) # A few options are available, but not many yet
+    converter = kbputils.converters.AssConverter(k) # Several options are available to tweak processing
     doc = converter.ass_document()  # generate an ass.Document from the ass module
     with open("outputfile.ass", "w", encoding='utf_8_sig') as f:
         doc.dump_file(f)
 
 There's also a CLI for it (command and syntax subject to change):
 
     $ KBPUtils --help
-    usage: KBPUtils [-h] [--border | --no-border] [--float-font | --no-float-font] [--float-pos | --no-float-pos] [--target-x TARGET_X]
-                    [--target-y TARGET_Y] [--fade-in FADE_IN] [--fade-out FADE_OUT] [--transparency | --no-transparency] [--offset OFFSET]
-                    source_file [dest_file]
-    
+    usage: KBPUtils [-h] [--version] [--border | --no-border | -b] [--float-font | --no-float-font | -f] [--float-pos | --no-float-pos | -p]
+                [--target-x TARGET_X] [--target-y TARGET_Y] [--fade-in FADE_IN] [--fade-out FADE_OUT] [--transparency | --no-transparency | -t]
+                [--offset OFFSET] [--overflow {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}]
+                source_file [dest_file]
+
     Convert .kbp to .ass file
-    
+
     positional arguments:
       source_file
       dest_file
-    
+
     options:
       -h, --help            show this help message and exit
-      --border, --no-border
+      --version, -V         show program's version number and exit
+      --border, --no-border, -b
                             bool (default: True)
-      --float-font, --no-float-font
+      --float-font, --no-float-font, -f
                             bool (default: True)
-      --float-pos, --no-float-pos
+      --float-pos, --no-float-pos, -p
                             bool (default: False)
-      --target-x TARGET_X   int (default: 300)
-      --target-y TARGET_Y   int (default: 216)
-      --fade-in FADE_IN     int (default: 300)
-      --fade-out FADE_OUT   int (default: 200)
-      --transparency, --no-transparency
+      --target-x TARGET_X, -x TARGET_X
+                            int (default: 300)
+      --target-y TARGET_Y, -y TARGET_Y
+                            int (default: 216)
+      --fade-in FADE_IN, -i FADE_IN
+                            int (default: 300)
+      --fade-out FADE_OUT, -o FADE_OUT
+                            int (default: 200)
+      --transparency, --no-transparency, -t
                             bool (default: True)
-      --offset OFFSET       int | bool (default: True)
-    
+      --offset OFFSET, -s OFFSET
+                            int | bool (default: True)
+      --overflow {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}, -v {NO_WRAP,EVEN_SPLIT,TOP_SPLIT,BOTTOM_SPLIT}
+                            AssOverflow (default: EVEN_SPLIT)
+
```

### Comparing `kbputils-0.0.5/pyproject.toml` & `kbputils-0.0.6/pyproject.toml`

 * *Files identical despite different names*

